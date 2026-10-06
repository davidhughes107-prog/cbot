# VSware Help Centre: the next 60 article drafts from support calls

**How to use this document.** Each article below is drafted from the steps support agents actually gave on the phone between March and September 2026. It uses the format the chatbot and the help-centre search read best: a title phrased as the user's question, the answer first, numbered steps with no screenshots required, then the phrases callers use so search finds it.

**Summary.** 56 of the 60 articles replace or merge with an existing help-centre article, named under each title.
4 are new, with no existing article covering the topic: 12, 20, 36 and 43.
59 articles carry an Editor note (only 56 has none): conflicts with the existing article, vague source steps, or overlap with another topic. Steps marked *(from existing article)* come from the current help centre, not from a call.

---

## 1. How do I import or refresh subject options in Timetable Construction?

**Asked 8 times.** Replaces or merges with: *Importing Generated Option Blocks into your Timetable Construction file*.

**Short answer:** Generate the option blocks and class lists first, then use **Actions > Refresh Options** in Stage 5 of Timetable Construction. You can repeat it whenever the options change.

**Steps**

1. Generate the option blocks and class lists in Options. Nothing can be imported without them.
2. Go to **Timetable Construction**, then **Actions** and select the timetable you are working on. *(from existing article)*
3. Go to Stage 5, **Class Data**, and select the year the option blocks are for. *(from existing article)*
4. Click **Actions > Refresh Options**.
5. If more than one solution exists, select the correct one when prompted.
6. If the options change later, repeat **Refresh Options**.

**Note:** if you remove a subject option, that student's preference is left blank. The student doesn't have to submit their choices again.

**Editor note:** two of the calls asked whether a block solution can be rearranged and whether subjects or teachers can be pinned to fixed blocks. The agent's steps don't answer either. Pinning is covered in *Timetable - Fixing/pinning Lessons on the Grid*. Topics 19 and 35 overlap with this one; consider merging all three.

**Use this when a school says**
- "can we import the options before the allocations are final"
- "can we still change the options after they're in the timetable"
- "how do I get the option blocks into timetable construction"
- "I changed the options, how do I update the timetable"

---

## 2. Why does it say "no active teaching groups" when I set up a State CBA for SPHE, CSPE or PE?

**Asked 7 times.** Replaces or merges with: *Junior Cycle and short course Subject Codes*.

**Short answer:** The teaching groups have the wrong subject code. Change every short-course teaching group to the correct code: SPHE 901, CSPE 900, PE 97.

**Steps**

1. Go to **Admin > Current Timetable > Teaching Groups** and select the year group.
2. Search for the subject by name or by teacher.
3. Scroll across the row to the **Edit** button and click it.
4. Change the subject code to the correct one (for example 901 for SPHE) and click **Save**/**Update**.
5. Repeat for every teaching group in each short-course subject.

**If the code doesn't exist yet (for example PE, 97)**

6. Go to **Settings > Subjects > Add Subject**.
7. Enter the subject name (for example PE Short Course), set the short code and short name to PE, choose a colour, and set the subject code to 97.
8. Save. You don't need to fill in required hours.
9. Go back to **Teaching Groups** and edit every PE class to use code 97.

**Editor note:** the existing *Add/Edit Subjects* article uses **Actions > New Subject** and says a subject code can't be edited later. Confirm the three codes against PPOD. Topics 7 and 30 describe the same fix; consider merging.

**Use this when a school says**
- "it says there are no active teaching groups with students for this year and subject"
- "I can't create the SPHE CBA"
- "teachers can't enter CBA results, it says no teaching group is linked"
- "the PE short course won't come up for the CBA"

---

## 3. Why can't I publish the timetable until I add a new term?

**Asked 7 times.** Replaces or merges with: *Publishing your Timetable* (Step 1) and *Setting Up the Calendar - Term Dates and Day Types*.

**Short answer:** The upcoming academic year needs a term with start and end dates before you can publish into it. Add the term, then publish.

**Steps**

1. Click the academic year selector in the top left corner.
2. Click the edit pencil.
3. Select the latest term and click **Add term**.
4. Enter a term name, for example 2026/2027.
5. Enter the start and end dates for the year.
6. Enter a term code, for example Full Year.
7. **Save**.
8. Publish the timetable file.

Add the term before you publish. Otherwise the school attendance calendar will not be auto-populated. *(from existing article)*

**Editor note:** the existing articles reach the edit pencil through **Settings > (Timings >) Academic years** instead of the top-left selector, and use "FY" as the example code. One call reported that the 2026/27 year was missing from the publish drop-down. The agent's steps add a term; they don't create a year. The existing article says the next academic year is created by the PPOD rollover and schools must not create it manually. Confirm what to tell a school whose next year is missing.

**Use this when a school says**
- "it won't let me publish the timetable"
- "26-27 isn't showing in the publish drop-down"
- "how do I set up the new academic year before publishing"
- "it says I need to add a term"

---

## 4. How do I create parent accounts for incoming first years and let them pay fees in the app?

**Asked 6 times.** Replaces or merges with: *How to create access for a group of parents* and *Onboarding Parents to VSware*.

**Short answer:** Move into next year, generate accounts for the incoming first-year group, then give parents the fee permission.

**Steps**

1. Use the year selector in the top left to switch to the next academic year, and open its settings cog. Choose **Just Me**. *(from existing article)*
2. Go to **Settings > System Settings > Account Generation**.
3. Select the incoming first-year class group. Check the exact group name under **Classes** first (for example First Year JCSP).
4. Set the username/password format and generate the parental accounts. Leave **Overwrite Usernames & Passwords Already Set** as **No**. *(from existing article)*
5. To enable fee payments, go to **Settings > Users and Groups** *(from existing article)* > **Available Permissions**. Leave the first category as it is, select **Contact** in the second, filter by "fee", and drag the fee payment permission into the **Contact** column.
6. Switch back to the current year to confirm the fees there. Fee permission changes carry over between years.
7. Check that the Stripe integration status shows as complete, so payments will work.

**Editor note:** the existing article calls this **Generate Parental Accounts**, and says VSware generates usernames only; parents set their own passwords. Confirm the label and the "password format" wording.

**Use this when a school says**
- "how do I set up the incoming first-year parents so they can pay fees"
- "I've entered the household details, how do I generate the usernames"
- "should we create the first-year parent logins now or wait for the timetable"

---

## 5. How do I publish next year's timetable and auto-populate the school calendar?

**Asked 5 times.** Replaces or merges with: *Publishing your Timetable*.

**Short answer:** Publish into the next academic year with **Actions > Publish Timetable**. The auto-populate option fills the calendar using your day types. The timetable stays visible only to you until you move all users forward.

**Steps**

1. In Timetable Construction, go to Screen 8, **View** *(from existing article)*. Click **Actions > Publish Timetable** and choose the next academic year.
2. To see what auto-populate will do, open **Settings** (the gear icon in the top blue bar) > **School Settings > School Attendance Calendar**. Each day type (for example Monday) has its own colour.
3. If you need them, create custom day types such as Holiday or School Closure Day.
4. Publish. If the publish button seems stuck, refresh and try again.
5. If a message says no match was found for a class, select **Do not match** for those classes and submit.
6. Wait for the system to confirm the publish was successful.
7. The published timetable is visible only to you until you select **All Users**. To do that, go to **Settings > Academic Year > gear icon > All Users**. *(from existing article)*

**Editor note:** the existing article describes the choices for unmatched classes as **Match** or **Deactivate**, not "Do not match". Confirm the label. Topics 9, 23, 24 and 37 also cover publishing; consider one publishing article with sections.

**Use this when a school says**
- "how do I publish next year's timetable so the office can see it"
- "what does auto-populate school calendar do"
- "the publish button is stuck"
- "it says no match found for a class"

---

## 6. How do I add a new class group and put students into it?

**Asked 4 times.** Replaces or merges with: *Adding an Extra Base Class*.

**Short answer:** The class group code must start with a letter, so use a single letter. Then drag students into the group in Current Timetable.

**Steps**

1. In Timetable Construction, go to **Class Data > Actions > Add Base Class**. *(from existing article)*
2. Enter a single letter as the class group code (for example A, B, C or D). It must start with a letter, not a number. Don't combine it with the class name.
3. **Save**. *(from existing article)*
4. To add students, go to **Admin > Current Timetable**.
5. Open **Class List Manager**, select the year and **Class Groups** *(from existing article)*, then click and drag students into the class group.

**Editor note:** the agent's steps don't say where the class group is created. Steps 1 and 3 come from the existing article, which also says a new base class should only be added when pupil numbers increase. One call was about a class not appearing on a teacher's timetable; that is covered by top-20 article 12.

**Use this when a school says**
- "it says the class group code must start with a letter"
- "how do I set up tutor groups for the incoming first years"
- "how do I put students into the new class group"

---

## 7. How do I fix a subject code that shows the wrong subject name?

**Asked 4 times.** Replaces or merges with: *Add/Edit Subjects*.

**Short answer:** If your school doesn't use the wrongly named subject, rename that subject instead of creating a new one. Then update the teaching groups that need it.

**Steps**

1. If your school doesn't use the subject entry with that code, edit it and rename it to the correct subject. To do that, go to **Settings > Subjects** and click the edit pencil. *(from existing article)*
2. Go to **Admin > Current Timetable > Teaching Groups**.
3. Select the year group.
4. Type part of the subject name in the name box.
5. Click **Edit** on the teaching group and change its name or code. Save.
6. Repeat for any other year group (for example third year) that needs the code for CBAs.

**Editor note:** this call gave the path as "Admin > Timetable > Teaching Group"; I have used the form other calls used. One call asked how to get PPOD's PE code (97) into VSware. That fix is in topics 2 and 30; consider merging all three.

**Use this when a school says**
- "the subject shows as Culture and Tourism instead of Classics"
- "the wrong subject name is coming up for the CBA"
- "the PE code is overlapping with another subject"

---

## 8. How do I remove duplicate students from a class in Class List Manager?

**Asked 4 times.** Replaces or merges with: *Duplicating students in a class*.

**Short answer:** Turn on **Allow Duplicates** for the class so you can move and remove its students. Turn it off again when you're done.

**Steps**

1. Click **Teaching Groups** on the left and select the year.
2. Find the class and click **Edit** on the right.
3. Tick **Allow Duplicates** and click **Update**.
4. Refresh the page. Select the current timetable, the year and the block. Duplicated students are highlighted in orange.
5. Hover over a student's name and click the small **x** to remove them.
6. If the removal doesn't seem to work, refresh the page and try again.
7. When you've finished, go back to **Edit** on the class, untick **Allow Duplicates** and click **Update**. This turns off the orange highlighting.

**Editor note:** two of the calls aren't answered by these steps. In one, a student who has left still shows on a State CBA. In the other, a staff member couldn't drag and drop in Class List Manager, though it worked when support mimicked their account.

**Use this when a school says**
- "a student is in the class twice"
- "it only lets me move duplicates out of the class"
- "why are some students orange in Class List Manager"

---

## 9. My timetable republish keeps stalling. How do I republish?

**Asked 4 times.** Replaces or merges with: *Publishing your Timetable*.

**Short answer:** Publish again from the timetable view. Check the year and start year, and type your own password rather than accepting a value the browser fills in.

**Steps**

1. Go to the timetable view.
2. Click **Actions > Publish Timetable**.
3. Select the correct school year (for example 26-27).
4. Check the start year is correct.
5. Type your password. Don't use a value the browser has filled in automatically.
6. Select **copy school day types** and auto-copy.
7. Submit.

Publishing overwrites any data already in the year you publish into. On a republish, you may be asked whether to match or deactivate teaching groups that have changed. *(from existing article)*

**Editor note:** the source doesn't say what caused the stall. The only fix it shows is entering the correct password. One call published "just for me" and couldn't get all users to see it; that is the **All Users** step in topic 5.

**Use this when a school says**
- "the republish keeps stalling"
- "I fixed the error but it still won't publish"
- "it's asking me to match a class because we merged classes"

---

## 10. How do I add a support class with students from several base classes?

**Asked 4 times.** Replaces or merges with: *Creating New Teaching Group/Special Tuition Classes*.

**Short answer:** Either cross a block of the core classes with the support class in construction, or, after publishing, create a teaching group and move the students in by hand.

**Steps**

**Option 1 (while building the timetable):** create a block with the core classes and cross it with the learning support class.

**Option 2 (after publishing):**

1. Go to **Admin > Current Timetable > Teaching Groups**.
2. Create a new teaching group and assign the teacher.
3. Put the class on the teacher's timetable: go to the teacher's profile > **Timetable > Actions > Make Editable**, click the period, then **Add Lesson** and choose the group. *(from existing article)*
4. Manually move the relevant students into the teaching group for that period.

**Editor note:** the agent gave Option 1 as a single line with no steps, and said "make it editable" without saying what to make editable. Step 3 is my reading, based on the existing article. One caller wanted to add a career appointment without attaching it to a class block; the source doesn't say whether this method suits that.

**Use this when a school says**
- "the support class has students from every base class"
- "how do I add the autism class with mixed years to the timetable"
- "I don't want it attached to a base class"

---

## 11. How do parents get on the app, and how do I message them through VSware?

**Asked 3 times.** Replaces or merges with: *VS-Mail - Everything you need to know* and *Getting Parents online - a step by step guide*.

**Short answer:** Parents use the app. You message them with VS-Mail, which is part of the communications package. There is no news feed; share links in a mail instead.

**Steps**

1. Parents find the school in the app by searching for the school's roll code rather than its name.
2. Check that the communications package is active: look for the envelope icon in the top right. If the package isn't active, clicking it prompts you to upgrade.
3. To message parents, click **Compose**, put the recipient group (for example all students) in **BCC**, and send.
4. Parents get a notification in the app when a new mail arrives. No SMS is sent automatically.
5. There is no news feed for parents. To share something, send a link (for example to a Google Doc or your website) in a mail.
6. To check what parents can see, go to **Settings > Users and Groups** and review the **Contact** column.
7. Encourage parents to download the app and log in there, rather than only using the website.
8. For guides to share, search "parents" on support.vsware.ie.

**Editor note:** the existing article says parents should search for the start of the school's VSware URL or its official name, not the roll code. Confirm which works. One call (rotations) isn't answered here.

**Use this when a school says**
- "is there a news feed for parents"
- "how do I send a mail to all parents"
- "parents can't find the school in the app"

---

## 12. Teachers and class groups look mismatched in next year's timetable. Will it fix itself?

**Asked 3 times.** New article.

**Short answer:** Yes. Leave mismatched class groups alone while you build. When you publish, the system corrects teacher and class list assignments using the class codes.

**Steps**

1. Don't change or swap teachers on class groups that show a mismatch while you build the new timetable.
2. When the timetable is published, the system corrects teacher and class list assignments based on the codes.
3. When you create a class block (for example a subject for a year group), select the subject and teacher, set the class size and spread, and save. The system assigns the correct class code.
4. If a teacher really is changing because the teaching arrangement is different, you can change them. Avoid changing teachers where the class list should stay the same, as this can leave class lists blank.
5. You can't see class lists or student numbers on the timetable construction screen before publishing.

**Editor note:** the other two calls asked about workload, feasibility and clash errors during construction. The steps don't answer them; see *Timetable - Feasibility Testing*.

**Use this when a school says**
- "the teachers and classes don't match in next year's timetable"
- "will the mismatches correct themselves when I publish"
- "should I swap the teachers back"

---

## 13. How do I compare a year group's mock results with earlier exams?

**Asked 3 times.** Replaces or merges with: *Term Assessment Performance Report*.

**Short answer:** Use the Term Assessment Performance report, one year group at a time, and export it to CSV.

**Steps**

1. Go to **Overview > Assessments > Academic Performance**.
2. Select **Term Assessment Performance**.
3. Select the base class. Working through one year group at a time is recommended.
4. Select the exam (for example the mocks).
5. The traffic-light colours show improving (green) and declining (red) performance.
6. View it on screen or export it to CSV (Excel). Most schools use CSV.

Teachers see only **Class Assessment Performance** by default. To give a teacher this report, add the permission **Allow teacher access to assessment reporting feature** in **Users and Groups**. *(from existing article)*

**Editor note:** two calls in this group asked for different reports: one for how many cover classes a teacher had, one for the best attendance in each class. This article doesn't answer either.

**Use this when a school says**
- "I want to compare sixth year's mocks with their Christmas results"
- "how do I pull academic tracking for a year group"
- "export the exam results to Excel"

---

## 14. How do I hide one student's subject result from parents?

**Asked 3 times.** Replaces or merges with: *Term Assessments* (show/hide subjects section).

**Short answer:** Hide the subject on that student's term assessment before you publish results. A subject with no result entered can't be hidden.

**Steps**

1. Search for the student.
2. Scroll to the **Term Assessments** section.
3. Select the assessment to view. *(from existing article)*
4. Click **Actions**.
5. Click **Enable Show/Hide Subjects**.
6. Hide the subject before results are published. You can't hide a subject that has no result entered yet.

You can undo this later if needed. *(from existing article)*

**Editor note:** the existing article calls the option **Enable remove subjects**, then a **Hide** button. Confirm the current label. The other two calls aren't answered here. Reopening an assessment window is topic 54; printing term reports is *Print Term Reports for a Year Group*.

**Use this when a school says**
- "can I hide one student's results from the parents"
- "don't show this subject on her report"
- "publish to everyone except these students"

---

## 15. How do I print address labels with students' names and addresses?

**Asked 3 times.** Replaces or merges with: *Saving Label Templates* and *Creating Mailing Label templates*.

**Short answer:** Use **Print Student Data** on the classes you need, add Full Name and Address, and export as labels.

**Steps**

1. Go to the student list and select the classes you need.
2. Click **Actions > Print Student Data**.
3. Add **Full Name** and **Address** to the fields.
4. Arrange the fields in the line order you want.
5. Click **Export As**.
6. Select **Labels 21, 3 by 7**.
7. Click **Accept** and **Generate**.

To reuse the layout, click **Save as template** and give it a name. *(from existing article)*

**Editor note:** the other two calls in this group asked how to print timetables and term reports for a year group. Those aren't answered here; see top-20 article 10 and *Print Term Reports for a Year Group*.

**Use this when a school says**
- "how do I print address labels for a class"
- "I need labels with the student's name and address"
- "print envelopes labels for first years"

---

## 16. How do I add students from other classes into a teaching group in Class List Manager?

**Asked 3 times.** Replaces or merges with: *Class List Manager - Moving students from class to class*.

**Short answer:** Open the year in Class List Manager, scroll to the unassigned students at the bottom, and drag them into the class.

**Steps**

1. Go to **Classes Manager** and select the year group.
2. If there's no scroll bar, use the small white arrows at the top and bottom to scroll.
3. Scroll to the bottom to see unscheduled or unassigned students.
4. Drag the students you need from unassigned into the class.

To move several students at once, click each one, then drag the group. *(from existing article)*

**Editor note:** agents called this screen "Classes Manager" here and "Class List Manager" elsewhere. The steps cover unassigned students only. They don't explain the second call, where some students were missing from a combined LCA1/LCA2 group. Creating a new group in a block is topic 60.

**Use this when a school says**
- "I need students from two groups in one class"
- "some students are missing from the combined LCA class"
- "there's no scroll bar in Class List Manager"

---

## 17. Why can't incoming first-year parents see the subject options I published?

**Asked 3 times.** Replaces or merges with: *Enabling parents access to Subject Preferences/Options* and *Where do I find my Incoming Year 1 Students?*

**Short answer:** Set up first-year options in the current year's dataset, not next year's. Parents also need login details and the options permission.

**Steps**

1. Set up the subject options in the current year's dataset, not next year's.
2. In **Student Setup**, use the grey box to change the year. For incoming first years, select the next academic year on the left and next year's first years on the right. *(from existing article)*
3. Make sure parents have login details.
4. Make sure parents have the permission. Go to **Settings > Users and Groups > Available Permissions**, filter by **Contact**, type "Option", and drag **Access to Options Preference Entry for Parents** into the **Contact** column. *(from existing article)*
5. Open entry for parents: **Options** > Screen 3 > **Actions > Publish to Parents**, set the dates, and save. *(from existing article)*
6. The options carry over automatically when timetable construction starts. The staff member building the timetable must still refresh them there (see topic 1).

**Editor note:** step 1 and step 2 read as if they contradict each other. Please confirm the exact year selections before publishing. The third call asked how to show parents only a language pool; the source doesn't answer that.

**Use this when a school says**
- "first-year parents can't see the options"
- "next year's first years aren't showing in subject setup"
- "I published the options but parents say there's nothing there"

---

## 18. How do I republish term results to parents after adding missing grades?

**Asked 3 times.** Replaces or merges with: *Term Assessments* (publishing results section).

**Short answer:** Unpublish the assessment, then publish it to parents again.

**Steps**

1. Go to **Overview > Term Assessments** and find the exam (for example the sixth-year mocks).
2. Click the three dots.
3. Select **Unpublish to parents**.
4. Click the three dots again.
5. Select **Publish to parents**.
6. Choose whether to send a push notification, then confirm.

**Editor note:** two calls in this group were parents not seeing current results. The source doesn't say whether republishing fixed those, so I haven't presented it as the fix for that symptom.

**Use this when a school says**
- "the missing subject's grades are in now, how do I republish"
- "parents can only see the old Christmas results"
- "parents can't see the results even though they're entered"

---

## 19. How do I create next year's timetable and bring in this year's option blocks?

**Asked 3 times.** Replaces or merges with: *Timetable Construction (Step 1) - Setup* and *Importing Generated Option Blocks into your Timetable Construction file*.

**Short answer:** Create a new timetable file, then refresh the options for each year in Screen 5. The current timetable isn't affected.

**Steps**

1. Go to **Admin > Timetabling**.
2. In Step 1, choose **Create new timetable**, give it a name (for example year and version), and click **Create**.
3. Wait for it to process. It moves on to Step 2, the grid.
4. Go to Screen 5, **Class Data**.
5. Select the year group on the left.
6. Click **Actions > Refresh Options**. This brings the current year's option choices into next year's file without changing the current timetable.
7. Select other year groups (for example second year) to see the rolled-over students with their existing teachers.
8. Build out the remaining bands and teachers before publishing.

Use **Create new timetable**, not **Clone**. Cloning the published file doesn't roll the data over. *(from existing article)*

**Editor note:** agents call this area both "Timetabling" and "Timetable Construction". This topic overlaps topics 1 and 35. To preview the timetable with the principal only, use **Just Me** (topic 5).

**Use this when a school says**
- "how do I roll over to next year's timetable"
- "how do I get the option blocks into next year's file"
- "what order do I do the steps in"

---

## 20. A warning says "proceeding will delete all existing solutions". Is it safe?

**Asked 3 times.** New article.

**Short answer:** The warning is about generated option block solutions. It doesn't remove other students' subject choices. If you haven't generated option blocks yet, it is safe to continue.

**Steps**

1. Read the warning. It removes generated option block solutions only. Other students' subject choices are kept.
2. If you haven't generated option blocks yet, type **confirm** and continue.

**Editor note:** the source doesn't say what to do if blocks have already been generated. Topic 31 says that changing preferences after generation means generating the blocks again. Consider merging this article into topic 31.

**Use this when a school says**
- "it says proceeding will delete all existing solutions"
- "will I lose the other students' choices"
- "is it safe to type confirm"

---

## 21. How do I move students into the right year group in Student Setup?

**Asked 3 times.** Replaces or merges with: *Step 1) Student Setup*.

**Short answer:** Remove the students from the wrong list, then add them to the correct one.

**Steps**

1. Go to **Student Setup** and check which year group list the students are showing under (for example next year's first years).
2. Select all the students in the wrong list and delete them, using **<< Delete Students** *(from existing article)*. This moves them back into the left column.
3. Add them to the correct list (for example next year's second years) with **Add Students >>** *(from existing article)*.

**Warning:** if you have already entered preferences for these students on later screens, moving them will lose those preferences. *(from existing article)*

**Editor note:** the source gives these steps for the first call. It doesn't confirm that the same steps answered the other two: sixth to fifth year in next year's timetable, and TY to fifth year.

**Use this when a school says**
- "the first years aren't showing as next year's second years in options"
- "move a student from sixth to fifth year for options"
- "a student is in the wrong year group in student setup"

---

## 22. How do I change CBA results entered in a previous school year?

**Asked 3 times.** Replaces or merges with: *Opening past & historic CBAs for editing*.

**Short answer:** Go back into the previous academic year, reopen the CBA, update the results there and resubmit, so they sync correctly.

**Steps**

1. Go to **Assessments > State CBA** and select the previous academic year. *(from existing article)*
2. Click the three dots beside the CBA and choose **View**. *(from existing article)*
3. Click the three dots beside the teaching group and choose **Reopen grading**, then confirm. *(from existing article)*
4. Click the three dots and **Add Results**. Update the results, then **Save and Exit**. *(from existing article)*
5. Click **Actions > Submit Results**. *(from existing article)*

**Editor note:** the agent said only "go back into the previous year, reopen the exam, update the results". All the numbered steps come from the existing article. Topics 33, 46 and 54 cover the same reopen flow; consider one article. The third call (attendance for a previous year) isn't answered.

**Use this when a school says**
- "how do I fix last year's CBA results"
- "a teacher wants to change a CBA result she already entered"
- "resync CBA results from a previous year"

---

## 23. Publishing fails with "unable to match elements" and Submit is greyed out

**Asked 3 times.** Replaces or merges with: *Publishing your Timetable*.

**Short answer:** Usually the timetable file hasn't been constructed yet. Check you are publishing the right file and run construction before publishing.

**Steps**

1. Check the name of the timetable file you are publishing.
2. Go into Timetable Construction and confirm the timetable has been constructed (run).
3. If it hasn't, run timetable construction, then publish again.

**Editor note:** the steps are brief. The source doesn't say what fixed the second call, where some class groups couldn't be matched. The third call in this group was a locked teacher account, which is unrelated; see top-20 article 14.

**Use this when a school says**
- "it says unable to match elements"
- "the submit button is greyed out when I publish"
- "it wants me to match classes but there are no options"

---

## 24. How do I generate and publish next year's timetable?

**Asked 3 times.** Replaces or merges with: *Publishing your Timetable*.

**Short answer:** Generate in Screen 7, then publish from Screen 8 into the next academic year. Get it right before publishing, because later changes count as a republish.

**Steps**

1. Go to Screen 7, **Construction**, and click **Generate**.
2. Wait for the timetable to generate. This can take a minute or two.
3. Go to Screen 8, **View**.
4. Click **Actions > Publish Timetable**.
5. Select the correct academic year (for example 26-27) and the start date.
6. Enter your password to confirm.
7. Choose whether to auto-populate the school calendar. This is recommended because it saves manual work.

**Note:** any change after publishing counts as a republish, which can be harder. Publishing again overwrites data already in that year. *(from existing article)*

**Editor note:** this topic overlaps topics 5, 9 and 37. The third call asked what happens to new students during rollover; the source doesn't answer that.

**Use this when a school says**
- "how do I publish next year's timetable"
- "can I republish if I need to change it"
- "how do I generate the timetable"

---

## 25. How do I add another class line to a timetable block?

**Asked 3 times.** Replaces or merges with: *Adding an Extra Base Class*.

**Short answer:** Try clicking the grey space beside the existing subject. If that doesn't work, add a base class and move the students across.

**Steps**

1. In **Class Data** *(from existing article)*, click the grey space beside the existing subject to add a new one.
2. If that doesn't work, go to **Actions > Add Base Class**.
3. Name the new base class to fit your existing pattern (for example 4B).
4. Drag and drop the students from the old class line into the new one.
5. Delete the old, now blank, class line.
6. Repeat **Add Base Class** for the next line (for example 4C) and save.

**Editor note:** the existing article says to add a new base class only when pupil numbers increase. To lengthen a block, it says to add a Dummy Class instead. That conflicts with the agent's advice; confirm before publishing. The other two calls (a resource class for Irish, and copying a group between blocks) aren't answered here.

**Use this when a school says**
- "how do I add a third subject line to block 12"
- "I need another line in the block alongside ethics and guidance"

---

## 26. Why isn't auto-assign rooms putting classes into specialist rooms?

**Asked 3 times.** Replaces or merges with: *Rooms - Room Pools*.

**Short answer:** A room that belongs to a pool isn't picked up by auto-assign. Remove the pool from the specialist rooms and run auto-assign again.

**Steps**

1. Go to Timetable Construction and click **Rooms** at the top.
2. Check the **Pool** column for each specialist room (for example PE, engineering, construction studies, home economics, science labs).
3. Rooms assigned to a pool are not picked up by auto-assign.
4. Remove the pool assignment (leave it blank) for each specialist room.
5. Run **auto-assign rooms** again.

**Editor note:** this conflicts with the existing *Room Pools* article. That article says putting a room in a pool is how you mark it as a specialist room, so it isn't given to general classes. Removing the pool may let auto-assign put general classes into specialist rooms. Please confirm with product before publishing. The third call asked whether auto-assign is safe to use; the source doesn't answer that.

**Use this when a school says**
- "auto-assign rooms isn't assigning the PE hall"
- "the specialist rooms aren't being used"
- "engineering classes have no room after auto-assign"

---

## 27. How do I move a pinned lesson, or remove an extra hour that appeared?

**Asked 3 times.** Replaces or merges with: *Timetable - Fixing/pinning Lessons on the Grid*.

**Short answer:** An extra hour usually comes from a class being unpinned and added again; remove the duplicate in Class Data. To move a pinned lesson you unpin, re-pin and regenerate.

**Steps**

**Extra hour after editing**

1. Open **Class Data** for the subject and find and remove the duplicate or extra hour.

**Moving a pinned lesson to another day**

2. Unpin the existing lesson, pin the replacement lesson, then unpin the lesson you want to move. To pin or unpin, click the lesson in Step 7 and choose **Pin** or **Unpin**. *(from existing article)*
3. Clear the grid for both affected timetables (for example LCA1 and fifth year).
4. Re-pin the lessons in their new slots.
5. Regenerate the timetable.

**Editor note:** most of this call was the agent diagnosing the problem. Step 1 is the agent's advice with no detail on how to find the extra hour. The unpin/pin order in step 2 is as the agent said it; please confirm it with product.

**Use this when a school says**
- "an extra class appeared after I edited the LCA timetable"
- "how do I move a pinned subject to a different day"
- "the split class isn't on the second teacher's timetable"

---

## 28. How do I move a class to a different period on a published timetable?

**Asked 3 times.** Replaces or merges with: *Make Editable - Manually Edit a Teacher's Timetable during the school year*.

**Short answer:** Edit the teacher's timetable, not the students'. Students follow automatically. Only go back to construction for big changes.

**Steps**

1. Open the teacher's profile > **Timetable > Actions > Make Editable**. *(from existing article)*
2. Add the lesson to the new period, as long as the teacher is free then.
3. Remove the lesson from the old period.
4. Students in that class follow the change automatically, because they are linked to the teacher's timetable.
5. To resolve a room clash, move the lesson the same way, as long as there is no conflict.
6. Go back to timetable construction and republish only if the changes are complex or teacher timetables are changing a lot.

**Caution:** changes made here are not written back to the timetable file. Republishing the file overwrites them. *(from existing article)*

**Editor note:** top-20 article 7 covers the same task in the opposite order (delete, then add). Merge the two and pick one order. The third call, about two teachers on one class, is top-20 article 3.

**Use this when a school says**
- "can I move a class on the published timetable or do I have to republish"
- "my changes in construction aren't showing on the teacher's timetable"
- "move the room and teacher to a different period"

---

## 29. I deleted a class from a slot and now can't add a new one there

**Asked 2 times.** Replaces or merges with: *Make Editable - Manually Edit a Teacher's Timetable during the school year*.

**Short answer:** The current week may still have the slot filled by a cover arrangement. Make a different week editable and add the class there.

**Steps**

1. Go back to the normal timetable view.
2. Click the calendar icon beside the week's date range at the top.
3. Select a different week, before or after the current one. The current week may already have the slot filled because of cover.
4. Click **Make Editable** on that week's timetable and add the class.
5. If a code (for example student intervention) can't be added because another teacher has the slot, make the slot editable, click the time, and choose **Add as Additional Teacher** at the bottom of the options.

**Editor note:** the second call asked about taking attendance for fourth years who join a fifth-year block for some periods. That isn't answered here. Step 5 overlaps top-20 article 3.

**Use this when a school says**
- "I deleted the class but it won't let me add anything in that slot"
- "the slot is free but I can't add a lesson"

---

## 30. How do I set up the PE subject code so CBA results sync to PPOD?

**Asked 2 times.** Replaces or merges with: *Add/Edit Subjects* and *Junior Cycle and short course Subject Codes*.

**Short answer:** Create a Physical Education subject with the PPOD code, then move every PE teaching group onto it.

**Steps**

1. Go to **Admin > Timetabling > Subjects**.
2. Add a new subject. Name it Physical Education (add the year group if needed), with short name PE and the subject code PPOD requires.
3. If another subject already uses that code, edit that subject first and rename or recode it.
4. Go to **Admin > Current Timetable > Teaching Groups**.
5. Search for the PE teaching groups by year or teacher, edit each one, and change it to the new subject code.
6. Repeat for every relevant year group (second and third year, and optionally first year).
7. Before creating the CBA, check that the correct number of active teaching groups appears.

**Editor note:** this call gave the path **Admin > Timetabling > Subjects**. Topic 2 and the existing article use **Settings > Subjects**. The existing article also says a subject code can't be edited later, which conflicts with step 3. Merge with topics 2 and 7.

**Use this when a school says**
- "how do I set up PE so the CBA syncs with PPOD"
- "change the subject code for junior cycle PE"
- "the PE code doesn't match PPOD"

---

## 31. Can I enter students' subject preferences for them?

**Asked 2 times.** Replaces or merges with: *Step 3) Preferences* and *Entering Subject Preferences as a School Admin- Video (4 minutes)*.

**Short answer:** Yes. Enter them on Screen 3 in Options before you generate blocks.

**Steps**

1. Go to **Options**.
2. Go to Screen 3.
3. Enter the student's preferences directly. Click a preference column to choose from the subjects allowed. *(from existing article)*
4. If no blocks have been generated on Screen 4 yet, you can ignore the warning that existing solutions will be cleared.
5. Don't generate blocks (Screen 4) until every preference is in. If you change preferences after generating, you have to generate the blocks again.

**Editor note:** the second call was about teacher assignments in the SNS roster and isn't answered here. Topic 20 covers the same warning; consider merging.

**Use this when a school says**
- "can I put in the fifth-year choices for students who haven't submitted"
- "enter subject preferences for a student manually"

---

## 32. How do I merge a parent's two logins for siblings into one?

**Asked 2 times.** Replaces or merges with: *Siblings Are Not Properly Linked* and *Linking Siblings & Incoming 1st Years*.

**Short answer:** Link the siblings, delete the duplicate parent contact, then copy the existing parent contact over from the sibling.

**Steps**

1. Link the two students as siblings: open the student's **Household** tab > **Add Siblings**, then select the sibling and save. *(from existing article)*
2. Before deleting, decide which contact to keep (the one the parent uses most). Note any details only the duplicate has, such as another phone number. *(from existing article)*
3. Delete the duplicate parent contact with the bin icon next to that parent.
4. Click **Add Contact** at the top.
5. Choose the option to copy the parent contact over from the sibling.
6. Refresh the page and check the same username now applies to both students.

**Editor note:** top-20 article 17 suggests giving duplicates distinct usernames as a quick fix instead of deleting one. Reconcile the two. The second call asked how to bulk remove all parent access before a migration; the source doesn't answer that.

**Use this when a school says**
- "the parent has two logins, one for each child"
- "merge the parent accounts after moving from our old system"
- "the parent can only see one child"

---

## 33. How do I change a CBA result that's already been synced to PPOD?

**Asked 2 times.** Replaces or merges with: *Opening past & historic CBAs for editing* and *State CBA*.

**Short answer:** Reopen grading on the CBA, edit the result, resubmit, and sync with PPOD again.

**Steps**

1. Go to **Overview > Assessments > State CBA**.
2. Find the assessment series.
3. Click the three dots next to the entry.
4. Select **Reopen grading** and confirm **Yes**.
5. Click the three dots again and select **Add results**.
6. Edit the student's result and **Save and Exit**.
7. Click **Actions > Submit Results**. *(from existing article)*
8. Sync with PPOD again: **Actions > Sync with PPOD**. *(from existing article)*

**Editor note:** the existing article opens **View** on the CBA, then reopens grading on the teaching group. The agent went straight to the entry's three dots. Confirm which level has **Reopen grading**. This overlaps topics 22, 46 and 54.

**Use this when a school says**
- "the CSPE result was synced but it's wrong"
- "change a CBA result after it went to PPOD"
- "how do I submit and sync CBA results to PPOD"

---

## 34. How do I upload CAT4 results for incoming first years?

**Asked 2 times.** Replaces or merges with: *CAT4 / Standardised Assessments – Bulk Upload*.

**Short answer:** Upload them under Standardised Assessments into next year's academic year. They then show on each student's profile.

**Steps**

1. Go to **Overview > Assessments > Standardised Assessments**.
2. Click **Upload Assessment**.
3. Select next year's academic year for incoming first years.
4. Enter the exam name (for example CAT4).
5. Upload the file. Teacher and parent reports may differ.
6. For more detail, watch the tutorial linked under **Standardised Attachment**.
7. Once uploaded, results show as an overview and on each student's profile under **Assessment**.

**Editor note:** the agent said to upload a zip file. The existing article says to download a CSV template, fill it in, and upload the CSV. Confirm whether these are two different uploads (results and reports) before publishing. The second call, setting up first-year parent accounts, is topic 4.

**Use this when a school says**
- "how do I upload the CAT4 results"
- "CAT4 results for the incoming first years"
- "link the CAT4 reports to student profiles"

---

## 35. How do I roll over to next year's timetable and refresh options for each year?

**Asked 2 times.** Replaces or merges with: *Timetable Construction (Step 1) - Setup* and *Creating a new file - What happens 'behind the scenes'*.

**Short answer:** Create a new timetable while staying in the current school year. Core years carry over; refresh options for any year that needs them, and add core blocks by hand.

**Steps**

1. Go to **Admin > Timetabling > Actions > Create new timetable**, staying in the same school year, and give it a name.
2. Core years (second, third, fifth and sixth) carry over automatically.
3. For incoming first years, or any group that needs options, go to Screen 5, **Class Data**, and select the year.
4. Use **Actions > Refresh Options** (not the system actions), while in the correct year.
5. Add core subject blocks by hand. There is no shortcut.
6. If first-year options look already done after refreshing another year, check whether they are real option classes or carried over from last year's setup.

**Editor note:** this overlaps topics 1 and 19; strongly suggest merging all three. The second call asked how to make a group of male students only and isn't answered here.

**Use this when a school says**
- "how do I create next year's timetable and roll the years over"
- "refresh the options for first, second and fifth year"
- "first-year options look like they're already there"

---

## 36. How do I delete a class without losing the option subjects linked to it?

**Asked 2 times.** New article.

**Short answer:** Move the linked subject or class block to the right-hand side first, delete the class, then move the block back if needed.

**Steps**

1. Move the subject or class block to the right-hand side.
2. Click the class you want to delete.
3. Click the **X** beside the class to delete it permanently.
4. Move the block back in if needed.

**Editor note:** the agent gave these steps in a different order: "move it back in if needed" came before the delete step. The source doesn't say which screen this is on. I have reordered the steps so they make sense; please check both the screen and the order in the product. The second call, about not losing class lists when setting up the new year, isn't answered here.

**Use this when a school says**
- "how do I delete 1F without losing the option subjects"
- "remove a class from the timetable but keep the options"

---

## 37. How do I publish next year's timetable before it's finished, for example to move to a new system?

**Asked 2 times.** Replaces or merges with: *Publishing your Timetable*.

**Short answer:** Import the option blocks, then publish into the next academic year as normal. It doesn't need to be complete.

**Steps**

1. Go to **Class Data**, select the year group, and click **Actions > Import Options** to bring in the option blocks.
2. Go to **Timetable Construction > Actions > Publish Timetable**.
3. Select the correct academic year (for example 26-27).
4. Check the start year is correct.
5. Enter your VSware password to confirm.
6. To make it visible to everyone, go to **Settings > Academic Year > gear icon > All Users**. *(from existing article)*

**Editor note:** this call said **Import Options**; other calls said **Refresh Options**. Confirm the label. This topic overlaps topics 5, 9 and 24.

**Use this when a school says**
- "we're moving to a new system, how do I publish so the data transfers"
- "the timetable isn't finished but I need to publish it"
- "how do I make next year's timetable visible to everyone"

---

## 38. How do I move a student from LCA1 to fifth year?

**Asked 2 times.** Replaces or merges with: *Class List Manager - Moving students from class to class*.

**Short answer:** After PPOD is corrected, move the student to unassigned, change their year, and put them in a base class in the new year.

**Steps**

1. Go to **Admin > Current Timetable**.
2. Open the LCA1 class list and find the student.
3. Move the student to unassigned.
4. Change the student's year to fifth year.
5. Assign them to a fifth-year base class.

**Editor note:** the source doesn't say where in VSware the year is changed in step 4. Top-20 article 13 covers the same task after a PPOD year change, and also covers option classes. Consider merging, and confirm step 4.

**Use this when a school says**
- "she was in LCA1 and is moving to fifth year"
- "a student is repeating and PPOD is updated, but VSware isn't"
- "move a student to a different base class after PPOD"

---

## 39. A room shows as unavailable to book, but I can't see a booking

**Asked 2 times.** Replaces or merges with: *Room Booking*.

**Short answer:** It is likely a recurring (block) booking at another time. Check the room's bookings and its timetable.

**Steps**

1. Print the room's timetable: go to **Admin > Current Timetable > Print Timetable**, choose **Rooms**, and select the room.
2. To view bookings for a date, go to **Room Booking > View or Cancel booking** and select the date. *(from existing article)*
3. To list all bookings for a period, go to **What rooms are Booked**, enter a start and end date, and click **Go**. You can export this list to Excel or PDF. *(from existing article)*

**Editor note:** the agent found the problem by looking in the bookings calendar themselves (a recurring meeting booking). Their advice was step 1. However, top-20 article 8 says manual room bookings do not appear on the room print-out. Confirm which is right; if article 8 is, drop step 1.

**Use this when a school says**
- "the meeting room won't let me book it but it's not booked"
- "which rooms are free each period"

---

## 40. What does "no matching subject assessment" mean on a State CBA?

**Asked 2 times.** Replaces or merges with: *State CBA* (adds an error section the article lacks).

**Short answer:** The subject the student has in VSware doesn't match the subject recorded for them in PPOD, or the subject code is wrong.

**Steps**

1. Click the error, then the three dots, then **View**.
2. Hover over the exclamation mark next to the student's name to see the message.
3. "No matching subject assessment" means the student's subject in VSware doesn't match the subject in PPOD.
4. Check whether the student actually studies that subject. They may have switched (for example from Irish to Geography), or joined or changed subjects partway through the year.
5. Check the correct subject code is selected. A wrong code causes the same error.

**Editor note:** topics 47 and 51 describe the same check; consider one "CBA won't sync" article.

**Use this when a school says**
- "some students have an error on the geography CBA"
- "it says subjects don't match"
- "one student's wood technology CBA won't sync"

---

## 41. How do I bring incoming first years into next year's options?

**Asked 2 times.** Replaces or merges with: *Where do I find my Incoming Year 1 Students?* and *Step 1) Student Setup*.

**Short answer:** In Options, change the year in the grey column to next year, select first year, and add the incoming students.

**Steps**

1. Incoming students must already be in PPOD and synced: go to **Settings > PPOD > Synchronise Students**. *(from existing article)*
2. Go to **Options**.
3. In the grey column, click the year (for example 25-26) and change it to next year (for example 26-27).
4. Make sure first year is selected.
5. Select all the incoming students.
6. Click **Add Students**.

**Editor note:** the second call asked how to stop students and parents seeing next year's timetable before it is final. That isn't answered here.

**Use this when a school says**
- "the incoming first years aren't showing in options"
- "how do I get next year's first years into subject setup"

---

## 42. I named a cloned timetable draft wrongly. How do I fix it?

**Asked 2 times.** Replaces or merges with: *Timetable Construction (Step 1) - Setup*.

**Short answer:** Clone the draft again with the right name, then delete the wrongly named copy.

**Steps**

1. In **Timetable Construction**, Step 1 (Setup), choose **Clone timetable** on the draft. *(from existing article)*
2. Give the clone the correct name.
3. Delete the wrongly named version.

**Caution:** deleted timetable files can't be restored by support. Make sure you delete the right one. *(from existing article)*

**Editor note:** the source doesn't say whether a draft can be renamed directly. The second call, about finishing a colleague's timetable and resolving clashes, isn't answered here.

**Use this when a school says**
- "I named the clone wrong"
- "is a misnamed timetable version a problem"

---

## 43. How do I put a clickable link in a VS-Mail?

**Asked 2 times.** New article.

**Short answer:** Paste the link, highlight it, and use the chain icon to turn it into a clickable link. Send yourself a test first.

**Steps**

1. Compose the mail in VSware.
2. Paste the link into the message.
3. Highlight the pasted text.
4. Click the link (chain) icon in the formatting toolbar.
5. Confirm, to turn the text into a clickable link.
6. Send a test to yourself and check the link works.
7. When sending to all parents or students, put the recipients in **BCC** so they can't see each other.

**Editor note:** the second call in this group asked how to print a room's timetable; see top-20 article 8.

**Use this when a school says**
- "how do I add a Microsoft Forms link to a mail"
- "the link isn't clickable"
- "attach a link in VS-Mail"

---

## 44. How do I publish allocated subject options to parents and students?

**Asked 2 times.** Replaces or merges with: *Step 4) Option Blocks* and *Removing access to Vsware when a teacher leaves*.

**Short answer:** When you're happy with the allocations, use the publish/allocate button on the option block screen.

**Steps**

1. On the option block screen in timetable construction, once you're happy with the allocated subjects, click the publish/allocate button. This sends the list to parents and students.

**Related: removing a retired staff member**

2. Open their profile. On the **Personal** tab, change **Left School** from **No** to **Yes**.
3. Confirm disabling their access when prompted. This also removes them from **Users and Groups**.

**Editor note:** the agent didn't name the button exactly ("publish/allocate"). The second caller wanted to publish allocations without letting parents change them. The source doesn't say whether this does that; the parent guide says parents then see an "allocated subjects" screen. Steps 2–3 overlap top-20 article 6.

**Use this when a school says**
- "how do I publish the subject allocations to parents"
- "can parents see the options without changing them"
- "remove a retired teacher from the system"

---

## 45. How do I find a parent's username and check their login works?

**Asked 2 times.** Replaces or merges with: *Mimic a parent account*.

**Short answer:** The username is on the parent's record under Household and Siblings. Parents reset their own password. You can use **Read Only Mimic User** to see their account.

**Steps**

1. Search for the student.
2. Click **Household and Siblings** on the left.
3. Click **Edit** on the parent's record.
4. Find the parent's username in their details.
5. Tell the parent to enter the username and reset the password themselves. School staff can't generate it.
6. To check the account works, click **Read Only Mimic User** at the bottom of the parent's edit screen.
7. Look at the parent dashboard to confirm the app is working. You can't change anything while mimicking. *(from existing article)*
8. To exit, click the four-boxes icon in the top right, log out, and log back in as yourself.

**Editor note:** this overlaps top-20 articles 2 and 11. The second call (the system won't allow the same username for a sibling's parent) is topic 32.

**Use this when a school says**
- "a parent can't log in and I don't know their username"
- "where do I find the parent's username"
- "can I see what the parent sees"

---

## 46. How do I reopen CBA grading so a teacher can submit late results?

**Asked 2 times.** Replaces or merges with: *Opening past & historic CBAs for editing* and *State CBA*.

**Short answer:** Reopen grading on the teacher's class. You don't need to change the original dates; only the status matters.

**Steps**

1. Go to **Assessments > State CBA** *(from existing article)*. Click the three dots beside the CBA and select **View**.
2. Click the three dots beside the subject or class and select **Reopen Grading**. The status shows "in progress".
3. The teacher then goes to their CBA overview and clicks the three dots > **View** > three dots > **Add Results** to enter results.
4. If the status shows **Not Submitted** in red, reopen grading the same way.
5. You don't need to change the original date range.

**Editor note:** this overlaps topics 22, 33 and 54; consider one "reopen a CBA" article.

**Use this when a school says**
- "the CBA window has closed and a teacher still needs to submit"
- "the date is greyed out"
- "it says not submitted in red"

---

## 47. Why are some CBA results only "partially synced" to PPOD?

**Asked 2 times.** Replaces or merges with: *State CBA* (adds an error section the article lacks).

**Short answer:** One or more students have an error. Hover over the yellow exclamation mark to see it. Usually the student doesn't have the subject in PPOD.

**Steps**

1. On the sync status screen, find the subject or class group showing **partially synced**.
2. Click the three dots next to it and select **View**.
3. Look for a yellow exclamation mark on a student's row.
4. Hover over it to see the error (for example "no matching subject assessment found").
5. This means the student is missing the subject on their eCard in PPOD, so the system doesn't know how to sync it. Check each flagged student.

**Editor note:** the second call was a PE short course whose code no longer matched PPOD; that fix is topic 30. Topics 40 and 51 overlap with this one.

**Use this when a school says**
- "some groups sync and others don't"
- "it says partially synced"
- "a generic sync error on the CBA"

---

## 48. How do I remove a subject with no students from an option block?

**Asked 2 times.** Replaces or merges with: *Step 4) Option Blocks*.

**Short answer:** Set the number of classes for that subject to zero and generate the blocks again.

**Steps**

1. Go to the year group's subject setup and option blocks.
2. Open the class details section for the subject block.
3. Set the number of classes to zero for each subject you want to remove.
4. Click **Generate Blocks**.
5. Check that the removed subjects no longer appear.

**Editor note:** the source doesn't name the exact screen for steps 1–2. The second call was about a student duplicated in two classes; see topic 8.

**Use this when a school says**
- "two subjects have no students, how do I take them out of the block"
- "remove a subject from the option block without affecting the others"

---

## 49. What does "unknown PPOD error" mean when I upload CBA results?

**Asked 2 times.** Replaces or merges with: *How to sync VSware with P-POD*.

**Short answer:** Usually the PPOD login saved in VSware has been rejected. Sync again using the school's own PPOD login, then retry.

**Steps**

1. Open the CBA, click the three dots and select **View** to see the error.
2. Go to **Admin > PPOD** and check the PPOD status.
3. If it says the PPOD login or password was rejected, click **Synchronize Students**.
4. Log in with the school's PPOD login, not a personal one.
5. If you don't have it, ask the principal for the school's PPOD login.
6. Once it syncs, upload the CBA results again.

**Editor note:** the existing article gives the path as **Settings > P-POD**; confirm. The second call (Leaving Cert results showing "not a member of the teaching group") isn't answered here.

**Use this when a school says**
- "it says unknown PPOD error"
- "CBA results won't upload"
- "the PPOD password was rejected"

---

## 50. How do I set up a new term assessment using last term's format?

**Asked 2 times.** Replaces or merges with: *Term Assessments* (creating a term assessment).

**Short answer:** Use **Duplicate** on last term's assessment, not **Edit**. Then change the dates and the exam name.

**Steps**

1. Go to **Overview > My Term Assessments**.
2. Find the previous term's assessment, click the three dots, and choose **Duplicate**. Edit won't let you change the dates.
3. Set the new start date. It must be tomorrow or later, not today. Leave it open until around the end of May.
4. Change the exam name (for example Summer 26).
5. Keep the existing template, even if it shows an older date; it already has the extra fields.
6. Click **Next** through the pre-set and custom fields without changing them.
7. On the review screen, click **Create Term Assessment**.

The exam name updates on the printed report, even if the template name shows an old date.

**To stop a subject appearing on one student's report:** go to the student's profile > **Classes & Groups**, click the edit pencil, untick **Subject is examinable for student**, and save. *(from existing article)*

**Editor note:** the existing article's path is **Assessments > Term Assessments**. Confirm "My Term Assessments".

**Use this when a school says**
- "set up the TY summer report the same as last time"
- "it won't let me change the dates"
- "a duplicate class is showing on a student's report"

---

## 51. Some CBA results won't sync to PPOD. What should I check?

**Asked 2 times.** Replaces or merges with: *State CBA*.

**Short answer:** Usually the teacher saved but didn't submit. Submit the results, then sync. If an error remains, it's usually the subject code or PPOD registration.

**Steps**

1. Go to **CBA** and choose the academic year.
2. Click the three dots on the CBA and select **View** to check the status.
3. **In progress** means the teacher clicked **Save** but not **Save and Submit**.
4. Click the three dots > **Add Results**, then **Actions > Submit Results**.
5. Confirm the status now shows **Submitted**.
6. Click the three dots and select **Sync with PPOD**.
7. If an error appears, hover over it to see why. It is usually a wrong subject code, or the student isn't registered for that course in PPOD.
8. Check PPOD that students are registered for the course. Irish, Maths and PE are common problems.
9. Remind teachers to use **Save and Submit**, not just Save, when they finish.

**Editor note:** this overlaps topics 40 and 47.

**Use this when a school says**
- "some CBA results aren't going to PPOD"
- "the woodwork CBA isn't syncing for some students"
- "the status says in progress"

---

## 52. How do I put staff meetings on next year's timetable?

**Asked 2 times.** Replaces or merges with: *Timetable - Adding Meetings (Video)*.

**Short answer:** Create a "Meeting" subject, add a meeting teaching group in Class Data, and add the attending teachers to it.

**Steps**

1. Add a subject called **Meeting**.
2. Go to **Class Data** and select the year group.
3. Add a teaching group by typing "meeting".
4. Add the teachers who attend as additional teachers in that group.
5. Create a separate teaching group for each different meeting if needed.

**Caution:** teachers in a meeting can't teach at that time, which also affects other teachers in their blocks. Don't add a large number of meetings. *(from existing article)*

**Editor note:** the existing article says there is no official "Meeting" subject. It renames an unused subject instead: **Settings > Subjects**, rename it to Meeting with short code MEET. It also places the group in a year not used for students. Confirm which approach to publish. The second call (two subjects at the same time on a student's timetable) isn't answered here.

**Use this when a school says**
- "how do I timetable senior management meetings"
- "add a meeting for several teachers to next year's timetable"

---

## 53. How do I text all parents in a group, and how do I check my SMS credit?

**Asked 2 times.** Replaces or merges with: *Send SMS to groups and classes* and *Topping Up SMS credit*.

**Short answer:** Click the phone icon beside the group to text everyone in it. Check and top up credit under Notifications > Top Up. Each SMS costs 5.5 cents.

**Steps**

1. Go to the classes or groups list where the group is (for example incoming first years).
2. Click the phone icon next to the group.
3. Type the message. Leave the template box blank if you aren't using a template.
4. Click **Send** to message all contacts in the group.
5. To check credit, go to **Admin Notifications > Top Up** to see your balance.
6. Top up there if needed. Each SMS costs 5.5 cents.

A text over 159 characters is charged as two. *(from existing article)*

**Editor note:** the existing article's path is three lines > **Notifications > Top Up**. Also, the agent instructions (top-20 article 20) tell the chatbot to hand off SMS credit and top-up questions to a person. Decide whether steps 5–6 belong in an article the bot will quote.

**Use this when a school says**
- "text all the incoming first-year parents"
- "how much credit do I have"
- "how much does a text cost"

---

## 54. How do I reopen a closed assessment so a teacher can enter late results?

**Asked 2 times.** Replaces or merges with: *Opening past & historic CBAs for editing*.

**Short answer:** Reopen grading on the class, enter the results, submit, and sync.

**Steps**

1. Go to **Overview > Assessments**.
2. Click **Assessments** again on the left.
3. Find the subject or class, click the three dots, and select **View**.
4. Click the three dots beside the class and select **Reopen Grading**.
5. Click the three dots again and select **Add Results**.
6. When all results are in, click **Actions > Submit Results**.
7. Go back to the previous page to sync with PPOD.

**Editor note:** these are the State CBA steps (they end with a PPOD sync). Both callers seem to have meant term assessments; one wanted to add year-head comments. The source doesn't confirm that term assessments reopen the same way; please check. This overlaps topics 22, 33 and 46.

**Use this when a school says**
- "the deadline has passed and a teacher still has results to enter"
- "reopen the assessment so I can add year head comments"

---

## 55. A double period shows as two singles. How do I fix it?

**Asked 2 times.** Replaces or merges with: *Lesson Spread in Timetable Construction (Step 5) - Class Data*.

**Short answer:** Correct the lesson count and spread for the subject in Stage 5, then drag the new blocks back into place in Stage 7.

**Steps**

1. Go to Stage 1, **Setup**, and select the timetable to work on.
2. Go to Stage 5.
3. Find the subject block (for example Maths) and click the arrow at its bottom right.
4. Change **Lessons** to the correct total (for example 6).
5. Change **Spread** to the correct pattern (for example 2-2-1-1) and click **Save**.
6. Go to Stage 7, **Construction**, and drag the new double and single blocks back to their original grid positions.
7. Check and reset any rooms that were unassigned; this process can unset rooms.
8. Keep the original (un-cloned) timetable as a backup.

**Editor note:** the existing article writes spreads with commas (2,2,1,1). Step 8 implies the school works on a clone, but the source doesn't say to clone first. Confirm both points. The second call (a duplicated music class showing as unscheduled) isn't answered here.

**Use this when a school says**
- "the double is showing as two singles"
- "the teacher has to take attendance twice for a double"

---

## 56. What business type and director should we choose in the Stripe setup?

**Asked 2 times.** Replaces or merges with: *Stripe Verify Company Directors*.

**Short answer:** Choose nonprofit organisation, then unincorporated non-profit. List the person who manages Stripe at the school as the director.

**Steps**

1. Go to **Admin > Fee Management > Stripe dashboard** and open the **Update Business information** banner. *(from existing article)*
2. If you're asked to upload a document to verify beneficial ownership, choose **Skip for now**. *(from existing article)*
3. Select **nonprofit organization** as the business type.
4. Select **unincorporated non-profit** as the business structure.
5. In the director field, list the person responsible for managing Stripe at the school.
6. Sign the electronic attestation. If you can't, choose **Upload a Directorship Document**, then download the **Director Digital Attestation** template. Print it, sign it, scan it and upload it. *(from existing article)*
7. Confirm the details and continue through the remaining verification steps.

**Use this when a school says**
- "what business type do we pick in Stripe"
- "who do we put down as director"
- "Stripe keeps asking for business documents that don't apply to a school"

---

## 57. Scheduling says "infeasible" after I assign rooms. How do I find the clash?

**Asked 2 times.** Replaces or merges with: *Timetable - Feasibility Testing*.

**Short answer:** Assign rooms one subject at a time and check feasibility after each, so you can see which assignment causes it. You can also unassign all rooms and start again.

**Steps**

1. Instead of assigning all rooms at once, assign them subject by subject.
2. After each subject, click **Check Timetable Feasibility** in Screen 5, **Class Data** *(from existing article)*. This shows which assignment causes the clash.
3. To remove all manually assigned rooms, go to Screen 5, **Class Data > Actions > Unassign Rooms**.

**Editor note:** the second call (blank periods, doubled-up classes and an oversized class list after publishing) isn't answered here.

**Use this when a school says**
- "it says infeasible since I added rooms"
- "the rooms aren't shared but it's still infeasible"
- "how do I remove all the rooms I assigned"

---

## 58. How do I get the total number of suspensions for a Tusla return?

**Asked 2 times.** Replaces or merges with: *Attendance crosstab report*.

**Short answer:** Run the Attendance Cross Tab report for all classes with the Suspension attendance code.

**Steps**

1. Go to **Overview > Attendance**.
2. Under **Reports**, select **Attendance Cross Tab**.
3. Under **Choose Class**, untick all classes so everyone is included.
4. Leave the filter selection as it is.
5. Under **Attendance Code**, select **Suspension**.
6. Run the report to get the total number of suspensions.
7. Repeat with the matching attendance code for full-day absences.

You can export the report to PDF or Excel. *(from existing article)*

**Editor note:** step 3 says to untick all classes to include everyone; check that this is right in the product. The second call asked for a list of absent students for a fire drill; that is in *Fire Evacuation/Fire Drill Report*.

**Use this when a school says**
- "how many suspensions for the Tusla report"
- "total suspensions for the year"
- "full-day absences for the Tusla return"

---

## 59. How do I print a master timetable on one page per year group?

**Asked 2 times.** Replaces or merges with: *Print and Export Timetable*.

**Short answer:** Use the horizontal layout with short codes and reduced spacing, then adjust orientation and scale in print preview. Set up each year group separately if needed.

**Steps**

1. Go to the **Print Timetable** screen *(**Admin > Current Timetable > Print Timetable**, from existing article)* and select the horizontal/individual layout.
2. Set print colour, and set rooms and teaching groups to show.
3. Set subject format to **short code** and teacher format to **short name**.
4. Set header period display type to **start time** and cell period display type to **hide**.
5. Try turning **reduce spacing** and the font size settings on and off.
6. Try the **single lines** period display type.
7. Compare **Export to PDF** with printing directly.
8. In print preview, try portrait and landscape.
9. Use the custom scale in print preview to reduce it slightly below 100%.
10. If a year group doesn't fit with the same settings, adjust it separately.

**Editor note:** the setting names are as the agent said them; check them against the screen. This overlaps top-20 article 10a (print settings).

**Use this when a school says**
- "fit each year's master timetable on one page"
- "print the master timetable in colour"
- "the master timetable runs onto two pages"

---

## 60. A new teaching group isn't showing in its block. How do I attach it?

**Asked 2 times.** Replaces or merges with: *How to create a block in Class List Manager*.

**Short answer:** Edit the teaching group and set its Block field to the right block.

**Steps**

1. Go to **Admin > Current Timetable > Teaching Groups** *(from existing article)* and find the teaching group.
2. Click **Edit**.
3. In the **Block** field, select or enter the correct block.
4. Save (**Update**).
5. Check it in **Class List Manager**: choose the year in **Select a Year** and the block in **Select a Grouping**. *(from existing article)*

**Editor note:** top-20 article 1 adds that the block name must match the other groups exactly (for example "Block 4", not "4"). That point isn't in this source; consider merging this topic into article 1.

**Use this when a school says**
- "I added a teaching group to the block but it's not showing"
- "how do I put the new class into block 4"
- "the new group isn't in Class List Manager"

---

*Drafted from March–September 2026 support calls. Steps reflect what agents said on the phone; check each one against the product before publishing.*
