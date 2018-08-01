## 1. Project Summary

1. Name of product...
Campus Snapshot: FAUBook

2. Look at pdf instructions

3. Describe unique features if any

4. URL to product: 

    
    

## 2. Milestone Documents


### 1. Executive Summary

University students who reside on campus indulge in the various social activities and events the campus has to offer. However, they're also exposed to all of the issues that arise throughout the campus. The goal of this project is to create a centralized web application where students, as well as, faculty, staff and visitors can connect to post about any events taking place around campus. Our team will be developing the web application “Campus Snapshots” to serve this purpose. 
Campus Snapshots will be an application which could be accessed through a personal computer or mobile device using all major browsers like, Safari and Google Chrome. The main purpose of this application will be to serve as a place where individuals can report instant snapshots of any issues happening around campus such as, leakage in a classroom, broken A/C, etc. These real time snapshots will consist of images or videos along with a description and will appear instantly on our web page in order to alert university administrators of the problems that need fixing. Administrators will then be responsible for verifying if the claims are accurate and providing status updates for these claims until they are resolved. 
Due to the various social activities that take place around campus, our website will also serve as a means of sharing posts about fun events. People can interact by commenting on each other's posts and having the ability to share posts with friends. In order to ensure a safe online environment, we will require users to register for personal accounts to be able to add/delete their posts and chat with friends and/or administrators. Other features like checking for the weather and searching for specific events within the site will be implemented in order to create a better user experience. Ultimately, we plan to develop a user friendly and easy to navigate site that will aid in keeping our university in great shape while providing a means for everyone to communicate and engage with one another.  


### 2. Competitive Analysis

*Image of Table 1: Sites Comparison 

Campus Snapshots will have the ability to upload instant images and videos like our competitors, Instagram and Snapchat. We will use a fluid chat system, implement content monitoring and use a system to block/ban false comments and contents similar to Facebook. Students will also be able to search for events and friends. However, we will add a weather system to alert students of major environmental threats which isn’t an option offered by any of our competitors.


### 3. Data Definition

1. Event: Image or video posted by site users along with descriptions to report campus issues or 
    social activities. 
-Images must be in .jpg or .png format with a maximum size of 10 MB. 
-Videos must be in .mp4 format with a maximum size of 100 MB.
2. Power User: Administrative user in charge of keeping track of reports to update their status  
    and monitoring overall site.
3. User: Student, professor, faculty, or other user able to create an account and post    
    events/comments on site. 
-Must provide first and last name, email, username, password, nickname, date of birth, gender, major (if applicable), and security questions/answers for account recovery. 
-May add profile image in the format of .jpg or .png with a maximum size of 5 MB. 
4. Role: Power vs Regular user
5. Verified: Posted event has been verified by power user as credible or appropriate.
6. Resolved: Posted event pertaining to an issue has been fixed and marked as solved by power 
    user in order to notify all other users. 
7. Path: The path of file system in the server to get the media files uploaded by the user.


### 4. Overview, Scenarios and Use Cases

User Stories:
1. I as Power user need verification service to be able to achieve the goal of verifying events 
    posted by users.
2. I as Power user need Push Events service to be able to achieve the goal of posting new events 
    as school’s events.
3. I as Power user need Post Managing service to be able to achieve the goal of deleting and 
    editing system events and force deleting fault events from users.
4. I as Power user need Blocking service to be able to achieve the goal of blocking fault users.
5. I as Registered user need Posting service to be able to achieve the goal of posting new events.
6. I as Registered user need Post Managing service to be able to achieve the goal of deleting and 
    editing my posted events.
7. I as Registered user need Post Sharing service to be able to achieve the goal of sharing 
    interested events.
8. I as Registered user need Post Commenting service to be able to achieve the goal of adding 
    comments in interested events.
9. I as Registered user need Post Searching service to be able to achieve the goal of browsing and 
    searching for events.
10. I as Registered user need Profile managing service to be able to achieve the goal of editing 
      my profile.
11. I as Registered user need Friend service to be able to achieve the goal of browsing, searching 
      and adding my friends.
12. I as Registered user need Message/Chat service to be able to achieve the goal of talking to 
      my friends and online admins.
13. I as Non-registered user need Register service to be able to achieve the goal of register and   
      become a member.
14. I as Non-registered user need Post Searching service to be able to achieve the goal of 
      browsing and searching for events.
15. I as Non-registered user need Message/Chat service to be able to achieve the goal of talking 
      online admins for help.


Use-case diagram:

*Image of Diagram 1: Use-Case Diagram


### 5. High-Level Functional Requirements 

1. Registration:
1.1. A user shall be able to make an account. [1]
1.2. A power user shall be able to make an account not by the registration page but by 
letting whoever responsible for the website put them in the database. [1]
2. Recover Access:
2.1. A user shall be able to answer security questions while register for an account in case 
       of forgotten access information such as username and/or password. [1]
2.2. A user shall be able to find his/her account in the recovery page with input 
       information. [1]
2.3. A user shall be able to reset password after correctly answering security question. [1]
3. Access: A user shall be able to login and logout after registered. [1]
4. Post Event and Write Comment: A user shall be able to post event and write comment. [1]
5. Delete Event: A user shall be able to delete his/her own post. [1]
6. Edit: A user shall be able to edit his or her post, comment, and profile. [2]
7. Verifying Event: A power user shall be able to label a post verified or not verified. [1]
8. Event Status: A power user shall be able to update the status of a report submitted by user. [1]
9. Force Remove Event: A power user shall be able to delete anyone’s post if it is wrong or 
    untruthful. [2]
10. Block User: A power user shall be able to block/ban a user if necessary. [2]
11. Search for Event: A user shall be able to search for posted events. [2]
12. Video Event: A user should be able to post a video event. [3]
13. Friend: A user should be able to make friends and have a friends list. [3]
14. Sharing: A user should be able to share a post event to his/her friends. [3]
15. Chat: A user should be able to chat with his or her friends and admins. [3]
16. Weather: A user should be able to check for the weather within the web page. [3]
17. Calendar: A user should be able to check for the date in the calendar section. [3]


### 6. List of Non-Functional Requirements

1. The website shall run on at least 3 major web browsers.
2. The user password shall be at least 8 characters including 1 uppercase, 1 number, 1 special 
    character, and no spaces.
3. The system shall send an email to the user to verify the email address after registration. This 
    email address is for the user to recover their account if necessary.
4. The system shall have 3 security questions for the user to answer during the registration 
    process.
5. A user shall be able to access his/her own account right after email verification.
6. A user shall be able to use all the website functions without prior training.
7. User data shall be stored in 1 database.
8. The language in the website shall be English.
9. The website shall be rich in content.
10. The user’s post shall be shown within 3 seconds.
11. A user shall be able to see status of submitted reports.
12. A user shall be able to scroll through webpage and see general content without logging in.
13. User password shall not be viewable at any point.
14. The system shall achieve 99% up time.
15. The system shall not be shut down for maintenance more than once in 2 days.
16. The time zone shall be obvious to the user on each post.


### 7. High-Level System Architecture 

Software products and Tools
Brackets, Notepad++, Putty, WinSCP, FileZilla, GitHub, etc
Languages and Systems
English, HTML, PHP, MySQL, Linux, Windows, MacOS, Mobiles , etc
APIs
Calendar, Weather
PHPMailer
Supported Browsers
Chrome, Firefox, Opera, Safari, Microsoft Edge, Internet Explorer
Frameworks
HTML, PHP, CSS



### 8. Database Organization

DB Organization: 
The database gets divided into multiple tables. With the UserID from the User table you can get access to the User_Info, Event, User_Comments, and Security_Answers tables. In addition, from Security_Answers you get data from Security_Questions using the QuestionID and both the Event and User_Comment tables get connected with not only UserID but EventID as well. In other words, as long as you have the UserID, you can get information in all the tables that belong to a specific person. 

List of DB Tables:
User: UserID, UserName, Password, Role, Status
User_Info: UserID, FirstName, LastName, NickName, DoB, Gender, Email, Telephone, Major
Event: EventID, UserID, Location, Description, Date/Time, Media, Verify, Path
User_Comments: C_ID, UserID, EventID, Comment
Security_Answers: UserID, QuestionID, Answers
Security_Questions: QuestionID, Questions

Media Storage:
The images and video/audio will be kept in file system. The database only stores the path to the files (Event table). 
Search/filter architecture and implementation:
The execution of a “select” statement to the database will be used for searching, where the condition for the statement can be any of the element in a collection of  fields used for searching.

Terms that will be used for searching: 
Username: a String stored in User table. Once the Username is found, the system will get the UserID and find the corresponding Nickname and display the Nickname back to UI.
Nickname: a String stored in User_Info table. Once the Nickname is found, the system will return and display the Nickname back to UI.
First Name/Last Name: two Strings stored in User_Info table. Once either one or both First Name Last Name is found, the system will return and display the corresponding Nickname back to UI.
Event Description (partial also works): a String stored in Event table. Once found, the system will return everything about that event back and display in UI.
Location: a String stored in Event table. Once found, the system will return every event in that location back and display in UI.
Term that will be filtered/sorted:
Location: a String stored in Event table. By applying this filter, the system will execute a search on the selected location.
Date/Time: a DateTime field in Event table, entered by the system when an event is posted, and will be sorted from newest to oldest.
Verify: a Boolean field in in Event table. By applying this filter, the system will show only the events that were verified by Power User.

Your own APIs:  
We will not create any API of our own.

Describe any significant non-trivial algorithm or process:
The order of the event post will be shown in order (newest first):  have to read the event from bottom up according to datetime. Before outputting each post, the Event table (store all of the event post from user) will get descending (DESC) sort by the Date/Time before outputting to the Home Screen.
Verifying is the process where a power user verifies whether a post is accurate or appropriate. In Event table there’s a verify field which all post will be masked as false at first. Then Power User can check the event physically and indicate whether the post is acceptable. From there the Power User can decide whether the post can stay in the system by click on verified or delete. 


### 9. High-Level UML Diagrams 

*Includes two images: class diagram and component and deployment diagram

Class diagram:
Diagram 2: Class Diagram


Component and deployment diagram:
Diagram 3: Component and Deployment Diagram



### 10. Identify Key Risks and Actions

Skills risks: Some of the development team members lack the database skills.
Schedule risks: Some of the team members are too busy, but other members are trying to make up for that. We’re trying our best to make it in time.
Technical risks: None
Teamwork risks: Lack of communication. Each member will have to review the idea for the project and communicate with the other members more. This is especially important when it comes to asking questions about anything that may seem unclear in order for all members to be on the same page and avoid any delays.
Legal/content risks: None


### 11. Vertical Software Demo

https://lamp.cse.fau.edu/~cen4010sum18_g04/demo_project
Demo Includes: 
User registration with email confirmation 
User information stored in database 
Password is hashed and salted
Verification of password to check if it meets the following criteria:
Minimum length of 8 characters
Must include at least one uppercase letter
Must include at least one lowercase letter 
Must include at least one number 
Login: 
Verifies user from database
Keeps count of how many times user fails to login


## 3. Product Screenshots





## 4. Google Analytics





## 5. Team Members Contribution


Jessica Carmona Matos <br>
Contribution Points: 25 points <br>

- Aid in writing all milestone's reports
- Final review and editing of reports before submission
- Submission of all milestone documents to canvas
- Assigning tasks to team members and updating information on Trello
- Email professor in the event of questions
- Database creation
- GUI mockup page creation 
- Demo video recording
- 
- 

Number of submissions on GitHub:



Tri Nguyen <br>
Contribution Points: 25 points <br>

- Aid in writing all milestone's reports
- Delegating tasks for each members
- Creation of team's Github and Trello accounts
- Database creation 
- GUI mockup page creation 
- Prototype development with user login/register, email confirmation, and security precautions
- 
-

Number of submissions on GitHub:



Vinh Huynh <br>
Contribution Points: 25 points <br>

- Aid in writing all milestone's reports
- GUI mockup multiple page creation 
- Design UI for website 
- Prototype development editing of page's layout 
-
-

Number of submissions on GitHub:



Carl Saintilmont <br>
Contribution Points: 25 points <br>

- Aid in writing all milestone's reports
- GUI mockup page creation 
- Various diagram creations for reports
- 
-

Number of submissions on GitHub:



## 6. Post-project Analysis


