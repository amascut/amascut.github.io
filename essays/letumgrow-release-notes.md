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
Trying to work on LetUmGrow alone has been a challenging process. I have the freedom to pursue my personal vision for the app, however that vision of mine is still hazy. Also, I think I tend to get some of my productive energy from a team. Sometimes, it is a struggle just to tear myself away from the small distractions!<br />


I'm trying to relearn the helper, event, and onCreated functions of Meteor templates. At times, I would like to ask for help, but I still wonder if I have done the necessary work and due diligence to even ask a 'smart' question.<br />


I may pursue finding a way to create and use test users. Requiring that a user have a UH account to log in seems to provide quite an obstacle to would-be trolls and developers alike.


I have been following the Meteor Chef admin console tutorial, but I have had to adapt it to LetUmGrow in many ways. The meteor chef folder structure is quite different as is their naming conventions for templates.


Going over the tuturial has also led me to the FlowRouter and alanning:roles package documentation. Basically, my current goal is to have access to certain groups of meteor routes tied to certain user roles. But the meteor chef admin tutorial has a little bit more functionality than that, which makes it harder for me to tease out the most relevant sections. For example, their tutorial also has an invitation section that requires creating an Invitations MongoDB collection. I opted not to add that part.


Also, it has proven difficult to follow the structure of their tutorial from the top of the page to the bottom, since handlebars code in the html files may come before the associated backend function code in the js files. Often, that causes the meteor build to fail and leaves me wondering if I did something wrong or if I just didn't implement the associated functions yet.


I'm having trouble figuring out the alanning:roles package from its documentation, too. At first I was confused if it was its own collection. However it seems to be an addition to Meteor.users and seems to be included if 'import {Meteor};' is written at the top. 


I haven't been able to consistently add a role to my user account. Often I will get an insert failed error. I'm not sure if that is because I am trying to add a role that has already been added or if I just am not using the roles package properly.


If I can figure out how to use the alanning:roles package properly along with the FlowRouter routing that should make creating new admins and admin only pages quite easy.


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