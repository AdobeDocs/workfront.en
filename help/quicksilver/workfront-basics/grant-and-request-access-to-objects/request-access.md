---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Request access to objects
description: Your visibility to objects in Adobe Workfront depends on your access to that type of object as well as your permissions on an individual object.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
---
# Request access to objects

Your visibility to objects in Adobe Workfront depends on your access to that type of object as well as your permissions on an individual object.

>[!NOTE]
>
>This article describes how you can request permissions to all objects except for plans in the Adobe Workfront Scenario Planner. For information about requesting access to plans, see [Request access to a plan in the Scenario Planner](../../scenario-planner/request-access-to-plan.md). This requires an additional license.

Your Workfront administrator configures your access to a type of object in your access level. For more information, see [How access levels and permissions work together](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

If you need permissions to specific objects within Workfront, you can request access to them. Rather than sending email to the Workfront administrator or object owner to explain your needs, you can request additional access (or permissions) within Workfront.

You can request initial access to objects if someone shares a link to the object with you, or you can request additional access to objects you cat at least view.

For example, you might have View permissions to a project, but you need to add tasks to that project. In this case, you can request Contribute permissions to the project.

## Access requirements

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

You must have the following to share objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Understand standard sharing rules

The following standard sharing rules take effect automatically, as they are set up as default options in your Workfront system. 

* Users assigned to a task or an issue have Contribute access on it. 
* Project, Portfolio, and Program managers have Manage access on the objects they own.
* Users included in a conversation have View access on the object where the conversation happens.
* Users assigned as approvers have View access on the object waiting to be approved.
* When sharing a dashboard, all reports on the dashboard are also shared with the same access to the same users. 
* Object owners are unable to extend access to an object beyond their access on that object as defined by the administrator.

## Request access

You can request initial access to objects that you do not currently have access to, or you can request additional access to objects that you have only limited access to.

* [Request initial access](#request-initial-access) 
* [Request additional access](#request-additional-access)

### Request initial access  {#request-initial-access}

If you do not already have access to an object and you navigate to that object from a link, a screen is displayed informing you that you do not have access to view the information.  

To request initial access to an object:

1. Click **Request Access**.  
   The **Request Access** dialog box is displayed.  

1. (Conditional) If more than one user has the appropriate access to grant you additional access, a drop-down arrow is displayed next to the name of the user. 
1. Select the user from the drop-down list who you want to receive your access request.  
   Only 10 users are displayed in the drop-down list. The list is sorted alphabetically.  
   For more information on the order of the users listed in this drop-down menu, see  [Hierarchy of the "Request Access" and "Request More Access" drop-down menus](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. From the drop-down list, select the type of access that you are requesting.
1. (Optional) In the **P.S.** field, specify a note to the user regarding why you need additional access.

   ![](assets/request-access-dialog-350x314.png)

If you do not have access level rights to an object and you try to access that object from a link, a screen is displayed informing you to contact the Workfront administrator. 

For example, if you do not have portfolio access, but you were given a link to a portfolio, you would see the following message:  
![](assets/permission-request-initial2-350x96.png)

### Request additional access {#request-additional-access}

To request additional access to an object that you already have limited access to:

1. Go to the object for which you want to request additional access.

1. Click the **More** menu to the right of the project name, then click **Request More Access**.  

   ![](assets/request-access-in-project-350x201.png)  

1. (Conditional) If more than one user has the appropriate access to grant you additional access, a drop-down arrow is displayed next to the name of the user.
1. Select the user from the drop-down list who you want to receive your access request.  
   Only 10 users are displayed in the drop-down list. The list is sorted alphabetically.  
   For more information on the order of the users listed in this drop-down menu, see  [Hierarchy of the "Request Access" and "Request More Access" drop-down menus](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. From the drop-down list, select the level of access that you are requesting.
1. (Optional) In the **P.S.** field, specify a note regarding why you need additional access.
1. Click **Request Access**.  
   ![](assets/request-access-dialog-350x314.png)

## Hierarchy of the "Request Access" and "Request More Access" drop-down menus {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Understand the hierarchy of users listed in the Request Access and Request More Access drop-down menus](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus) 
* [Understand the owner of an object](#understand-the-owner-of-an-object)

### Understand the hierarchy of users listed in the Request Access and Request More Access drop-down menus {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

When populating the "Request Access" or "Request More Access" lists on objects, Workfront selects a list of up to ten users that fulfill various roles in the sharing of the object as described below. These users can grant access to the object to the user requesting it.  
The resulting list is then is sorted by their name in ascending alphabetical order.   
Workfront displays up to 10 users in the "Request Access" and the "Request More Access" lists. 

The order of the users in the "Request Access" or "Request More Access" drop-down menus is dictated by the following rules: 

* The first user in the list is the object "owner", as described in [Understand the owner of an object](#understand-the-owner-of-an-object). 
* Then the list is populated with users with whom the object is shared individually. They are listed in alphabetical order.
* Then the list is further populated with users who get the required access through sharing with their teams, groups, or companies. They are listed in alphabetical order.
* If the list is empty, the Workfront administrators are added so that there is always someone to request access from. They are listed in alphabetical order. 
* Each of the users in the list must have the requested access to the object and access to share the object. 

### Understand the owner of an object {#understand-the-owner-of-an-object}

The owner of an object is defined as follows: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Object</strong> </th> 
   <th><strong>Definition of the Owner of the Object</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projects</td> 
   <td>The owner is the Project Owner or, if it is missing or they don't have the necessary access, the owner of the parent portfolio. <p>They might not be the same person as the project creator. </p></td> 
  </tr> 
  <tr> 
   <td>Tasks</td> 
   <td>The owner is the Primary Assignee or, if it is missing or they don't have the necessary access, the owner of project on which the task resides, as defined above. <p>They might not be the same person as the task creator. </p></td> 
  </tr> 
  <tr> 
   <td>Issues</td> 
   <td> <p>The owner is the Primary Contact of the issue or, if it is missing or they don't have necessary access, the owner of the project on which the issue resides, as defined above. </p> <p>They might not be the same person as the issue creator. </p> </td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>The owner is the Portfolio Owner. <p>They might not be the same person as the portfolio creator. </p></td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>The owner is the Owner of the document (the user who uploaded the document) or, if it is missing or they don't have necessary access, the owner of the object on which the document resides.</td> 
  </tr> 
  <tr> 
   <td>Reports and dashboards</td> 
   <td>The owner is the creator or the report or the dashboard. </td> 
  </tr> 
  <tr> 
   <td>Calendars</td> 
   <td>The owner is the creator of the calendar. All users have a calendar assigned to them by default. They are considered the owner of that calendar. </td> 
  </tr> 
  <tr> 
   <td>Filters, views, and groupings</td> 
   <td>The owner of a filter, view, or grouping is the creator. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Plans</span> </td> 
   <td> <p><span>The owner is the creator of the plan.</span> </p> <p>This requires an additional license. </p> <p><span>For information about the Workfront Scenario Planner, see</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The Scenario Planner overview</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Goals</td> 
   <td> <p>The owner is the user designated as the Owner. They might not be the same person as the goal creator. </p> <p>This requires an additional license. </p> <p>For information about Workfront Goals, see <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront Goals overview</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

 
