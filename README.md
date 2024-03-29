# COMP1004 Coursework 2

A front-end interface that queries a supabase backend.

## README Requirements

1. The URL to the GitHub Page where the front end is hosted.
   - This is the version that will be used for marking, so please make sure it is working.
     Please do not make any further changes after the submission, otherwise it will be considered
     as late submission (using the last commit date/time).
2. A description of the additional work for HTML, CSS, JavaScript, and/or database. Please see the marking rubrics below for the details about additional work (to achieve full mark
   for each criteria). Please describe separately for each aspect, i.e., HTML/CSS/JavaScript/database, what the additional work is, and where they are (file name and line number)

   - Please say so in this document if you don't attempt any of these.
   - Only the work described will be considered for mark.

## Criteria

#### Criteria - HTML

| Requirement                                                                                                                    | Complete | Hash | Description |
| ------------------------------------------------------------------------------------------------------------------------------ | -------- | ---- | ----------- |
| There are at least three HTML pages, one for each database query/update.                                                       |          |      |             |
| The files are named correctly.                                                                                                 |          |      |             |
| The page meta information is included and correct.                                                                             |          |      |             |
| The heading and text elements are used correctly.                                                                              |          |      |             |
| All the pages have the same navigation menu and the links works correctly.                                                     |          |      |             |
| Each page should have four sections: header, main, sidebar, and footer. These are marked up correctly using semantic elements. |          |      |             |
| There is at least one image or video for each page and all the required information is present and correct.                    |          |      |             |

#### Criteria - CSS

| Requirement                                                                                                                                 | Complete | Hash | Description |
| ------------------------------------------------------------------------------------------------------------------------------------------- | -------- | ---- | ----------- |
| All the pages should share the same external CSS file. Justifications are provided (as code comment) for internal or inline CSS formatting. |          |      |             |
| Class is used to selectively style some elements.                                                                                           |          |      |             |
| Location selector is used to selectively style some elements.                                                                               |          |      |             |
| Element border, margin, and padding are changed to improve the style.                                                                       |          |      |             |
| CSS Flex or Grid are used to layout the page:                                                                                               |          |      |             |
| The header should be at the top of a page;                                                                                                  |          |      |             |
| The side bar should be on the left or right of the main content;                                                                            |          |      |             |
| The footer should be at the bottom of a page.                                                                                               |          |      |             |

#### Criteria - JavaScript and database

| Requirement                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Complete | Hash                                                                                                                | Description                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------- | ------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| The user should be able to look up people by their names or their driving licence number (by typing either of these in to the system). If the person is not in the system it should give an appropriate message.                                                                                                                                                                                                                                                                                                   | ✅       | [2fc586d](https://github.com/Ben-Bromley/UON-COMP1004-Coursework-2/commit/2fc586d900807f11b5b12606829d44175c753e9a) | Using `getElementById` and `addEventListener` I've extracted the value from the text input when the form is submitted for us in the supabase JavaScript client |
| This search should not be case sensitive and it should work on partial names, e.g., “John”, “Smith” and “John Smith” would all find John Smith. If there are several people with the same name they should all be listed.                                                                                                                                                                                                                                                                                          | ✅       | [a77ddb5](https://github.com/Ben-Bromley/UON-COMP1004-Coursework-2/commit/a77ddb518b45a11f8dbb24a2b105b3e9af1020d0) | I've used the `ilike` method from supabase in order to do a case-insensitive search                                                                            |
| The user should be able to look up vehicle registration (plate) number. The system will then show details of the car (e.g., type, colour etc.), the ownerʼs name and license number. Allow for missing data in the system (e.g., the vehicle might not be in the system, or the vehicle might be in the system but the owner might be unknown).                                                                                                                                                                    |          |                                                                                                                     |                                                                                                                                                                |
| The user should be able to enter details for a new vehicle. This will include the registration (plate) number, make, model and colour of the vehicle, as well as its owner. If the owner is already in the database, then it should be a matter of selecting that person and assigning them to the new vehicle. If the owner is not in the database they should be added (along with personal information including the license number).                                                                           |          |                                                                                                                     |                                                                                                                                                                |
| (Only required for the full mark) The user should be able to file a report for an incident and retrieve existing reports (e.g., via a search). Filing new ones will involve submitting a textual statement, recording the time of the incident and the vehicle and person involved. If either the person or the vehicle are new to the system, then appropriate new entry/entries to the database should be added. An user should be able to record the offence from a list of offences contained in the database. |          |                                                                                                                     |                                                                                                                                                                |
