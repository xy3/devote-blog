---
title: Start/End dates and states for elections
date: 2020-03-01 18:05:17
tags:
---



  

# Election Start Times

We needed to have functionality to allow users to set a start and end date for their election. Before an election is started, users can observe but not vote. Once the current date reaches the start of the election, the app automatically starts it.

{% owl youtube S7r13EaDS84 %}

  

# Election Start & End Functionality and Election States

 **Election Start Dates**
A start and an end date can now be set for each election on their dedicated election pages. The input currently recognizes five different wrong inputs but only console logs them when they occur.

**Election States**
Elections now have one of four states. Awaiting Start, Pending Start, Active and Closed. 

**Awaiting Start**
When an election is made, it is automatically set to Awaiting Start. 

**Pending Start**
If a start date is set before the current date, the election goes into Pending Start. When in pending, candidates can still be added and deleted from the election. 

**Active**
If the start date is before the current date, the election is set to Active and can be voted in immediately. The candidates cannot be modified after the election is active. 

**Closed**
Finally, if an election reaches it's end date, the system will automatically close the election and wont accept any more votes.

{% owl youtube fU9bczmvIJA %}

  

## Date-Picker Error Feedback

When the functionality to start and end dates was created, the system only logged input errors. I made 8 different error checks when parsing the input of the date-picker. The errors can be seen in the video below.

{% owl youtube loY5aPDeNDE %}
