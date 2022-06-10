---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Username Already in Use
description: Read these tips when you get an error that the username is already taken.
feature: "People Teams and Groups"
---

# Username Already in Use

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Question

When creating a new user, a Whoops error is displayed stating that the username is already taken. There are no other occurrences of this email in the system. Why is this being displayed?

## Solution

This can occur either because the username or email address is not unique in the current Adobe Workfront instance. Users can have the same username or email address in separate instances. For example, User A could have the following email addresses associated with a Workfront account: usera@company1.com and usera@company2.com.

>[!NOTE]
>
>The primary Workfront administrator can't have the same username or email address if they are in separate Workfront instances on the same cluster.   
>
>If the instances are on different clusters, the primary admin can have the same username or email address. You can view the cluster your instance is on under Setup > System > Customer Info.

### Check if your username is unique in your instance

Ensure that the username and email address is unique in the current Workfront instance:

1. As the Workfront administrator, click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Users**.
1. In the list of people, look in the **Email** column to ensure there are no duplicate emails.
1. Add a column for username to the view.

   1. In the **View** drop-down menu, click **Customize View**.
   1. Click **Add Column**.
   1. In the search field, type *username*.
   1. Select **User** > **Username**.
   1. Save the view.  
      This results in a view to display the usernames where you can look for the duplicate.

1. In the list of people, look in the **Username** column to ensure there are no duplicate usernames.

