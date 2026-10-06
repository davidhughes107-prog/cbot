# VSware chatbot test runner

`bot_test.py` runs the 30-question test set in `vsware_bot_test_set.xlsx` against the
HubSpot Customer Agent with no one at the keyboard. For each question it:

1. Opens the chat bubble on your public web page in a fresh, private browser window,
   so every question starts a new conversation.
2. Types the question and waits up to 60 seconds for the bot's reply. If nothing comes
   back, it records `NO ANSWER`.
3. Asks Claude to score the reply 0, 1 or 2 against the "Expected answer / behaviour"
   column, using the rubric from the workbook's "Read me" sheet.
4. Adds a new pair of columns to the **Runs** sheet: the bot's answers and the scores.
   Hover over a score to see Claude's one-sentence reason.
5. Prints a summary: total out of 60, Timetable subtotal, hand-off subtotal, and every
   row that scored 0, with its reason.

Earlier runs are never changed. Each time you run the script it adds a new column pair.
The TOTAL, "Timetable only" and "Hand-off rows only" formulas are copied into the new
columns, so they keep working.

---

## Why it uses the chat bubble, not the HubSpot API

HubSpot's Conversations API can read conversations and post replies **as an agent**.
It can't start a new conversation **as a website visitor** on live chat, and that's
what testing the bot needs. The only API route is a "Custom Channel". That needs a HubSpot
developer app and HubSpot's beta "Deploy Customer Agent to Custom Channels" option. It
would also test a different channel from the one your customers use.

So the script drives the real chat bubble on your web page, exactly as a visitor would.
As a result, **you don't need a HubSpot token.** You only need the address of a page
where the chat bubble appears.

---

## One-time setup (Windows)

### 1. Install Python

1. Go to <https://www.python.org/downloads/> and click the big "Download Python" button.
2. Run the installer. **On the first screen, tick "Add python.exe to PATH"**, then click
   "Install Now".
3. To check it worked, open the Start menu, type `cmd`, and open **Command Prompt**.
   Type the following and press Enter:

   ```
   python --version
   ```

   You should see something like `Python 3.13.1`.

### 2. Put the files in one folder

Make a folder, for example `C:\BotTest`, and put these files in it:

- `bot_test.py`
- `bot_test_config.example.json`
- `requirements.txt`
- `vsware_bot_test_set.xlsx`

In Command Prompt, go to that folder and install the add-ons the script needs (this is
needed only once):

```
cd C:\BotTest
python -m pip install -r requirements.txt
python -m playwright install chromium
```

The last command downloads a private copy of the Chromium browser for the script to use.
It doesn't touch your normal browser.

### 3. Get an Anthropic API key (used for scoring)

1. Sign in at <https://console.anthropic.com/>, open **API Keys**, and click
   **Create Key**. Copy the key (it starts with `sk-ant-`).
2. Save it on your computer so the script can find it. In Command Prompt, run:

   ```
   setx ANTHROPIC_API_KEY "sk-ant-paste-your-key-here"
   ```

3. **Close Command Prompt and open a new one.** `setx` only applies to windows opened
   after you run it.

The key is stored in your Windows user settings, not in any file in the folder, so it
can't be shared by accident.

Scoring a full 30-question run costs well under $1.

### 4. Create your config file

1. In the folder, copy `bot_test_config.example.json` and rename the copy to
   `bot_test_config.json`.
2. Open it in Notepad and set `widget_url` to the address of a page where the chat
   bubble appears.

| Setting           | What it does                                                                                                                                         |
|-------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| `xlsx_path`       | Name of the test workbook. Leave it as is if the workbook is in the same folder.                                                                      |
| `widget_url`      | The page that shows the HubSpot chat bubble.                                                                                                          |
| `questions`       | Leave it as `[]` to run all 30. To run only some, list their numbers, for example `[27, 28, 29, 30]` for the hand-off rows.                           |
| `timeout_seconds` | How long to wait for each reply before recording `NO ANSWER`.                                                                                         |
| `headless`        | `true` runs the browser invisibly. Set it to `false` to watch the browser type each question, which helps if something goes wrong.                   |
| `scoring_model`   | The Claude model that does the scoring.                                                                                                               |

---

## Running it

Close the workbook in Excel first. The script can't save while Excel has it open, and
if it is open the script will wait and ask you to close it.

Open Command Prompt and run:

```
cd C:\BotTest
python bot_test.py
```

The full set takes roughly 20–30 minutes, mostly waiting for the bot. You'll see each
question and its score as it goes, and a summary at the end, for example:

```
============================================================
TOTAL            44 / 60
Timetable rows   20 / 24
Hand-off rows    5 / 8

Rows that scored 0:
  Q30: Our SMS credit top-up is giving an error.
       The bot gave top-up steps instead of handing off to support.
============================================================
```

### Other useful commands

Re-run only the hand-off rows. This overrides the config's `questions` setting:

```
python bot_test.py --questions 27-30
```

You can also list numbers, for example `--questions 1,4,9`.

Ask the questions and score them, but don't write anything into the workbook:

```
python bot_test.py --dry-run
```

Check that scoring works without touching the bot or the workbook. This scores three
built-in sample answers:

```
python bot_test.py --test-scoring
```

### What the script leaves in the folder

- `vsware_bot_test_set.xlsx`: updated with the new run columns.
- `backups\`: a copy of the workbook taken just before each save, in case anything
  goes wrong.
- `bot_test_logs\`: a raw record of every answer and score from each run. It is
  written as the run goes, so you keep the results even if the run is interrupted.

---

## Reading the results

- The new columns get a header like `Run 2026-10-06 (auto)` in row 1. A partial run
  shows which questions it covered, for example `(auto, Q27,28,29,30)`, and the other
  rows stay blank.
- The script fills the empty "Run 2" and "Run 3" columns that are already in the sheet
  first. After that, it adds new columns to the right with the same formatting and
  total formulas.
- The scores are Claude's judgement. Read the reasons, especially for any row that
  scored 1, and overwrite a score by hand if you disagree. The totals update
  automatically.
- If Claude couldn't score a row, its score cell is left empty and the summary lists it
  under "Not scored", so you can score it yourself.

---

## Troubleshooting

**`NO ANSWER` on every question.** Set `"headless": false` and watch what happens.
Common causes:

- The page needs a cookie banner accepted before the chat loads.
- The chat bubble isn't on that page.
- The bot asks for an email address before answering. If so, turn off email capture
  in the Customer Agent's channel settings while testing.

**Answers include extra text** such as "Was this helpful?" or the bot's name. Add
patterns to remove to the config, for example:

```json
"ignore_lines": ["^VSware Assistant$", "^Rate this answer.*$"]
```

Each pattern is a regular expression, matched against one whole line, ignoring case.

**Answers are cut short.** The script decides the bot has finished once no new text
has appeared for 6 seconds. If the bot pauses longer between messages, add
`"reply_settle_seconds": 10` to the config.

**`ANTHROPIC_API_KEY is not set`.** Repeat step 3, and make sure you opened a **new**
Command Prompt afterwards.

**`Model 'claude-sonnet-5' was not found`.** Set `scoring_model` in the config to a
current model, for example `claude-sonnet-5-5`.
