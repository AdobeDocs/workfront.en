---
title: View User Login Information
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: You can see how often users log in to Workfront, as well as the last time they logged in, by indicating that you want to include this information in the view of a list of users, or in a report for users.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
---
# View user login information

You can see how often users log in to Adobe Workfront, as well as the last time they logged in, by indicating that you want to include this information in the view of a list of users, or in a report for users.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. For information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if User <b>Admin (Group Users)</b> is enabled, you must be a group administrator of a group where the user is a member.</p> <p>For more information about the <b>Users</b> setting in an access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## How Workfront records login information

Workfront records the following information about users logging in to the system:

* **Login Count**: Workfront counts a user logging in to the application once every 24 hours. If one user logs in multiple times using different browsers, computers, or mobile devices, Workfront counts all of the logins that occurred in one day as one login. The Login Count includes information starting with when the user was created.
* **Last Login Date**: The last date when a user logged in. The date of every login from any browser, mobile device, or other applications is recorded in this field.

Logging in to Workfront in any of the following ways counts as a login to Workfront:

* The Workfront Web Application
* The Workfront Mobile Apps (iOS or Android devices)
* Any supported Workfront integration with another third party application (Slack, Jira)
* Any custom integration between Workfront and another third party application. 
* The Workfront API

  >[!NOTE]
  >
  >Logging in to Workfront through the Workfront API is only available to organizations that are not yet onboarded to the Adobe Business Platform.

## Display usage information in a user list or report

You can display the Login Count and the Last Login Date fields in the view of a list of users, or in a report for users.  
For more information about creating a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

To display usage information in the view of a list of users:

1. Go to a list of users in Workfront.
1. From the **View** drop-down menu, select **New View**.

1. Click **Add Column** near the lower-right corner of the screen.
1. In the **Show in this column** field, start typing **Login Count**, then select it when it appears in the list under **User**.

1. Click **Add Column** again.
1. In the **Show in the column** field, start typing **Last Login Date**, then select it when it appears in the list under **User**.

1. (Optional) Click **Advanced Options**, then select a **Field Format** from the drop down menu to include the time or the day of the week of the last login in your column.

1. Click **Save View**.  
   The view includes information about how many times the users have logged in and when they logged in last.
