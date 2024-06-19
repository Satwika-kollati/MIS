# MIS-Branch Change Module for UG Students

This module allows undergraduate students to submit a priority list for branch change preferences. The interface facilitates students to select and submit their branch change preferences from all available options.

## Project Description

**Course:** Software Engineering(CSC306) <br>
**Instructor:** Dr Saurabh Srivastava. Assistant Professor, Indian Institute of Technology (ISM) Dhanbad. <br>
**Description:** This project is developed to be integrated as one of the modules into our ISM Dhanbad's MIS website. The module provides an easy-to-use interface for students to make informed decisions about their branch changes.

## Tech Stack Used

- **Frontend:** Next.js with MUI
- **Backend:** Laravel (PHP)
- **Database:** MariaDB

## Features Implemented

1. **Student Authorization:**
    - Validates if the credentials belong to a registered student.
    - Ensures the user is registered as an undergraduate student in the 3rd semester.
    - Checks if the student has passed all courses in the 1st and 2nd semesters.
    - Verifies that the student's CGPA is greater than or equal to 7.
    - Confirms the student has not completed the physical registration process for the 3rd semester using the `status` attribute of the semester registration table.
![8](https://github.com/Satwika-kollati/MIS/assets/102177900/3a1e1581-0a36-483e-ae0b-eb075f83223b)![11](https://github.com/Satwika-kollati/MIS/assets/102177900/296ecafb-b3ac-4d17-870b-dd2df114f1b3)

2. **Redirection on Ineligibility:**
    - Redirects ineligible students to a page showing an error message.
![9](https://github.com/Satwika-kollati/MIS/assets/102177900/35c4be70-d2f4-4b9e-be12-29936709f58f)

3. **Priority Selection Form:**
    - Multi-step form where users first select a course, then branch options are dynamically rendered based on the chosen course.
    - Students can select at least 1 and at most 5 branches for the priority list.
    - The current branch of the student is not shown as a selectable option in the dropdown list while filling the priority.
![15](https://github.com/Satwika-kollati/MIS/assets/102177900/093b564a-0b64-416a-842b-a4d178ccb5c2)

4. **Dynamic Rendering:**
    - API call from the frontend to backend to fetch the list of courses and corresponding branches.
    - Branches selected are dynamically removed from the selectable options to avoid duplicates.
![16](https://github.com/Satwika-kollati/MIS/assets/102177900/901ea784-af37-4b32-a0be-1850cbd68b6f)

5. **Editable Priority List:**
    - Students can shuffle branches by dragging and dropping to change the priority order.
    - They can also delete branches, with the priority order adjusting dynamically.
![17](https://github.com/Satwika-kollati/MIS/assets/102177900/a8844f90-d463-4980-9c86-8ff8ba57736b)

6. **Submission Preview:**
    - Students get a preview of their priority list before final submission. A checkbox must be checked to confirm submission.![18](https://github.com/Satwika-kollati/MIS/assets/102177900/8ed467bc-c4b6-4de8-ac15-c266e19f2974)


7. **Post-Submission Page:**
    - Displays the student's current course and branch, submission date and time, and the approval status of the branch change.
    - Provides options to view and download the priority list in PDF format using the `jspdf` node package.![19](https://github.com/Satwika-kollati/MIS/assets/102177900/eb5cc418-e207-45c3-87a2-55e15283968d)

![22](https://github.com/Satwika-kollati/MIS/assets/102177900/284d31c3-8314-429b-bf81-966c3f1466b5)
![23](https://github.com/Satwika-kollati/MIS/assets/102177900/ff525d61-22cd-4669-9635-79906d3f441a)

8. **Approval Update:**
    - The approved branch will be updated in the front-end preview.
    - Students can submit the priority list form only once and will be redirected to the final preview page if they try to open the form again.  

## Team Members

- **Chandra Prakash** (21JE0260)
- **Vibhanshu Sharma** (21JE1039)
- **Parth Pandya** (21JE0635)
- **Kollati Satwika** (21JE0474)
- **Sake Raviteja** (21JE0804)

 Thank you!

