---
layout: essay
type: essay
title: LetUmGrow Release Notes
date: 2017-02-15
labels:
  - Project Management
  - Software Engineering
  - Web Apps
---



## M6 LetUmGrow Release Notes (02-15-17)

### Tasks Completed
Added pre-database wipe backup data .json files to LetUmGrow /backups directory

Made progress creating pages for the Admin functionality

### Tasks To Do (see <a href="https://github.com/LetUmGrow/LetUmGrow/projects/8">M7 Project Page</a>)
Finish implementing Admin functionality

### Notes
Working on LetUmGrow mostly solo this semester has been a challenging process. I have the freedom to pursue my personal vision for the app, however that vision of mine is still hazy. Also, I think I tend to get some of my productive energy from a team; it helps that my teammates from last semester still talk in the LetUmGrow slack, so I can keep them posted on updates and get encouragement from them.


Earlier in February, I was able to get some feedback from my instructor, Philip Johnson, which helped me decide on what to focus on first. In January, I tried to concurrently work on optimize my app for mobile and implementing the admin functionality but was able to achieve neither of those objectives. Following Dr. Johnson's arrangement of tasks, I decided to focus on getting the admin functionality working first. So my goal for the last milestone was to tie access to specific groups of meteor routes tied to specific user roles.


I decided to follow the <a href="https://themeteorchef.com/tutorials/building-a-user-admin">Meteor Chef admin console tutorial</a>, but I had to adapt it to LetUmGrow in many ways. The Meteor Chef folder structure, naming conventions, and base meteor app code were all a little bit different from what I had been used to working with. For example when creating new routes in /startup/client/router.js the tutorial used 'BlazeLayout.render( 'default', { yield: 'managers' } );'. I changed that to 'BlazeLayout.render( 'App_Body', { main: 'Managers_Page' } );' to get the managers page to display.


The admin tutorial also led me to the FlowRouter, Blaze.js, and alanning:roles package documentation.  But the meteor chef admin tutorial implemented a little bit more functionality than that, which made it harder for me to tease out the most relevant sections. Their tutorial had an email invitation section that requires creating an Invitations MongoDB collection. I opted not to add that part.


It sometimes proved difficult to follow the structure of their tutorial from top to bottom, since Spacebars code in the html files sometimes came before the associated backend function code in the .js files. Often, that caused the meteor build to fail and left me wondering if I did something wrong or if I just didn't implement the associated functions yet.


I had some issues figuring out how the alanning:roles package worked from its documentation, too. At first I wasn't sure if the roles were implemented as their own collection and needed to be imported on their own. However, I eventually learned that roles were implemented as an addition to Meteor.users and were included using the 'import {Meteor};' statement. 


At first when trying out the roles methods I was not able to consistently add a role to my user account. Often, I would get an insert failed error. It turned out that the methods associated with the roles package worked best when executed from the server in 'app/both/methods/update/' instead of from .js template files in 'app/imports/ui/pages/. I will have to conduct further research into Meteor best practices for security, to make sure that access to the database is secure to prevent unauthorized access to the database by the client.


Over the next couple of weeks, I will try to associate the user roles that I've implemented with specific groups of pages. (e.g. having the admin pages accessible by admins only) So far, I have 3 types of roles in mind: a general user role, a staff role (for use by UH Manoa staff), and an admin role (for developers).


## M5 LetUmGrow Release Notes (02-01-17)

### Tasks Completed
Redeployed to meteor galaxy at <a href="https://letumgrow.meteorapp.com">letumgrow.meteorapp.com</a>

Prepared for reset of database by backing up Users and Plants to json files

Researched Admin page and user roles

### Tasks To Do (see <a href="https://github.com/LetUmGrow/LetUmGrow/projects/7">M6 Project Page</a>)
Implement Admin page and user roles

Research and Implement Mobile First Usability
-Landing Page


## M4 LetUmGrow Release Notes (01-16-17)

### Current Features
<ul>
<li>Plant Map - displays plants on a google Map
  users can add plants to the map by clicking on the map
  users can move existing plants by clicking and dragging on plant icons</li>
<li>Hawaiian Remedies - plant remedies for conditions such as dry skin or irritable bowel syndrome</li>
<li>Tutorial - slide show explaining how the app works</li>
<li>Add Plants
   <ul>
      <li>has a form where users add new plants by entering information</li>
      <li>latitude and longitude are required</li>
      <li>plant name, scientific name, and description are not required</li>
      <li>partially functional 'Use current location' button; will auto populate latitude and longitude when clicked if location sharing is enabled</li>
   </ul>
 </li>
<li>Species Database</li>
<li>My Profile 
<ul><li> displays the current user's username, email, first name, and last name</li>
  <li> Saved locations - lists any plants they have added</li>
  <li> Contacts - lists other users that the current user has added as contacts</li>
  </ul>
  </li>
</ul>
<br><br>
For the past several weeks I have not made significant progress adding functionality to LetUmGrow, mostly some minor css tweaks, fixing some conflicts in Github, and figuring out how to self deploy. Last semester, I had trouble explaining what my plans for LetUmGrow were, so instead of rushing headfirst into programming, I wanted to clarify the goals I had for this app. So I decided to write out more of what I wanted to do and fit those goals into a timeline. In the interim between the previous and current semesters, I also wanted to do more research on similar apps. I found a plant identification app called Pl@ntNet which is used to identify plants by images taken by users. I would like to try contacting them in the future to see if future collaboration would be possible. However they are based in France so that could interfere with the communication process.
<br><br>

### Future Features
In the next couple of weeks once I have satisfactory goals and plans, I will be making LetUmGrow more user friendly, so that the plant map is easier to use. I will also be implementing different user roles like admin and general user. That way I will be able to keep features used for testing separate from features for general users. During testing, there had been a lot of confusion over that.

<br><br><a href="https://github.com/LetUmGrow/LetUmGrow/projects/6">M5 Project Page</a>