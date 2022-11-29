---
title: Access levels overview
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,level,system,administrator,planner,worker,reviewer,requestor,external,user
navigation-topic: access-levels
description: Every user must have an access level in order to log in and work in Workfront. You use the access level to control what a user can see and do with certain Workfront objects and areas.
author: Courtney
feature: System Setup and Administration
role: Admin
---
# Access levels overview

As an Adobe Workfront administrator, you assign an access level to a user for 2 purposes:

* Every user must have an access level in order to log in and work in Workfront. 
* You use the access level to control what a user can see and do with certain Workfront objects and areas.

## Built-in access levels in Adobe Workfront {#built-in-access}

Workfront has 3 built-in access levels. Each of the built-in access levels is attached to one of the 3 paid Workfront licenses: Standard, Light, Contributor. There is also an External unpaid license designed primarily for sharing documents with people who don't use Workfront.

Depending on the access level, up to 3 settings are available for most of the Workfront object types:

<table style="table-layout:auto">
    <tr>
        <td>Edit</td>
        <td>Users can create, edit, delete, and share the Workfront object</td>
    </tr>
    <tr>
        <td>View</td>
        <td>Users can review and share the Workfront object</td>
    </tr>
    <tr>
        <td>No Access</td>
        <td>Users cannot access the Workfront object</td>
    </tr>
</table>

If you need a custom access level, you can copy the built-in access level and adjust the amount of access you want it to allow for the various Workfront object types. For information on creating a custom access level, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>We strongly recommend that you leave the built-in access levels unchanged so that you can refer to them after you set up your users.

### System Administrator access level

Attached to the Standard license, this built-in access level is designed for a user who is in charge of administering the Adobe Workfront system. You cannot modify this built-in access level.

Users with the System Administrator access level can do everything within Workfront. They can view and edit all Workfront objects and information entered in Workfront by all other users.

They also have access to the complete Setup area, where they can change any setting at the system level. And they can access all areas in the  Main Menu ![](assets/main-menu-icon.png).

For more information, see [Grant a user full administrative access](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Standard access level

Also attached to the Standard license, this access level is designed for:

* Managers of groups, teams, projects, and resources
* Anyone who is responsible for planning, creating, and managing tasks, projects, portfolios, and programs
* Anyone who is responsible for assigning work (tasks and issues) to other users
* Users who build reports and who approve timesheets, work items, and documents
* Users who need access to all areas in the  Main Menu ![](assets/main-menu-icon.png)

You can create a custom version of the Standard built-in access level and adjust the amount of access it allows for the various Workfront object types. For information on creating a custom access level, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

The following are the highest access settings available for objects in the Standard access level:

| Workfront object type |No access |View access |Edit access |
|---|---|---|---|
| Projects |&nbsp; |&nbsp; |✓ |
| Tasks |&nbsp; |&nbsp; |✓ |
| Issues |&nbsp; |&nbsp; |✓ |
| Portfolios |&nbsp; |&nbsp; |✓ |
| Programs |&nbsp; |&nbsp; |✓ |
| Reports (including dashboards and calendar reports) |&nbsp; |&nbsp; |✓ |
| Filters, views, and groupings |&nbsp; |&nbsp; |✓ |
| Documents |&nbsp; |&nbsp; |✓ |
| Users |&nbsp; |&nbsp; |✓ |
| Templates |&nbsp; |&nbsp; |✓ |
| Financial data |&nbsp; |&nbsp; |✓ |
| Resource Management |&nbsp; |&nbsp; |✓ |
| Scenario Planner  |&nbsp; |&nbsp; |✓ (The default setting is No Access.) |
| Workfront Goals  |&nbsp; |&nbsp; |✓ (The default setting is No Access.) |

{style="table-layout:auto"}

### Light access level

Attached to the Light license, this access level <!-- need content from lauren -->


Users with the Light access level:

* Cannot be assigned work items or approve time sheets
* Can access requests and documents in the  Main Menu ![](assets/main-menu-icon.png).
* Have limited ability to create objects—they can't create projects, portfolios, programs, or reports.

You can create a custom version of the Light built-in access level and adjust the amount of access it allows for the various Workfront object types. For information on creating a custom access level, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

More limited for projects and tasks than the Worker access level, the following are the highest access settings available for objects in the Light access level:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront object type</th> 
   <th>No access</th> 
   <th>View access</th> 
   <th>Edit access</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projects</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Tasks</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Issues</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>&nbsp;</td> 
   <td>✓ (The default setting is No Access.)</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Programs</td> 
   <td>&nbsp;</td> 
   <td>✓ (The default setting is No Access.)</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Reports (including dashboards and calendar reports)</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Filters, views, and groupings</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Users</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
    <tr> 
   <td>Teams</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr>
  <tr> 
   <td>Templates</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Financial data</td> 
   <td>✓</td> 
   <td> <p>&nbsp;</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Resource Management</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Scenario Planner </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓ (The default setting is No Access.)</td> 
  </tr> 
 </tbody> 
</table>

### Contributor access level

Attached to the Contributor license, this built-in access level is designed <!-- need content from Lauren -->

For example, a user can log issues to your organization's help desk request queue.

Users with this built-in access level:

* Can make requests and update those requests
* Can upload and approve documents
* Can review the status of issues they have submitted
* Cannot be assigned to work items  
* Can  access requests only from the Main Menu ![](assets/main-menu-icon.png). For more information about request queues, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

You can create a custom version of the Contributor built-in access level and adjust the amount of access it allows for the various Workfront object types. For information on creating a custom access level, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

The following are the highest access settings available for objects in the Contributor access level:

| Workfront object type |No access |View access |Edit access |
|---|---|---|---|
| Project |&nbsp; |✓ (Only the Project Details page) |&nbsp; |
| Task |&nbsp; |✓(Only the Details page) |&nbsp; |
| Issue |&nbsp; |&nbsp; |✓ |
| Portfolios |✓ |&nbsp; |&nbsp; |
| Programs |✓ |&nbsp; |&nbsp; |
| Reports (including dashboards and calendar reports) |&nbsp; |✓ (Only the Details page) |&nbsp; |
| Filters, views, and groupings |&nbsp; |&nbsp; |✓ |
| Document |&nbsp; |&nbsp; |✓ |
| User |&nbsp; |✓ |&nbsp; |
| Teams |&nbsp; |✓ |&nbsp; |
| Template |✓ |&nbsp; |&nbsp; |
| Financial data |✓ |&nbsp; |&nbsp; |
| Resource Management |✓ |&nbsp; |&nbsp; |
| Scenario Planner  |✓ |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### External User access level

This access level is not attached to a paid Workfront license. It is the most restrictive access level, designed primarily for collaborators like external consultants who don't log into Workfront, but need to review, download, or view documents occasionally.

Workfront users can assign tasks to external users even though external users can't log in to the system. But we advise against this because that work would remain unresolved in the system. <!--still true?-->

Users with the External User access level:

* Can view only documents and calendar reports that are shared with them
* See the users who share documents and calendar reports with them
* Approve the documents that are shared with them

You cannot modify this access level.

>[!IMPORTANT]
>
>External User is available only if the option "Collaborate with people without Workfront accounts by using their email address" is enabled in the System Preferences area in Setup. For more information, see [Configure system security preferences](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md). 

The following are the highest access settings available for objects in the External User access level.

| Workfront object type |No access |View access |Edit access |
|---|---|---|---|
| Project |✓ |&nbsp; |&nbsp; |
| Task |✓ |&nbsp; |&nbsp; |
| Issue |✓ |&nbsp; |&nbsp; |
| Portfolios |✓ |&nbsp; |&nbsp; |
| Programs |✓ |&nbsp; |&nbsp; |
| Reports (including dashboards and calendar reports) |&nbsp; |✓ (Only for calendar reports; no ability to share reports) |&nbsp; |
| Filters, views, and groupings |✓ |&nbsp; |&nbsp; |
| Document |&nbsp; |✓ (without the ability to share documents) |&nbsp; |
| User |&nbsp; |✓ |&nbsp; |
| Teams |✓ |&nbsp; |&nbsp; |
| Template |✓ |&nbsp; |&nbsp; |
| Financial data |✓ |&nbsp; |&nbsp; |
| Resource Management |✓ |&nbsp; |&nbsp; |
| Scenario Planner  |✓ |&nbsp; |&nbsp; |


## How access levels and permissions work together

The Adobe Workfront administrator determines what access level each user should have. That access level defines what users can see and do with object types and areas in the system.

Users also gain access to individual objects when other users share and grant certain permissions on those objects.

So, the activities a user can do with an object are defined by a combination of their access level and the permissions given to them.

![](assets/security-model-hierachy-copy.png)

>[!INFO]
>
>**Example**: If your access level says that you can create tasks, but the permissions you receive on a specific project don't allow you to add tasks to it, you can't add tasks on the project even though you can create tasks elsewhere in Workfront.

### Access level

The access level assigned to each user by a Workfront administrator is required for logging in to Workfront.

The default access levels are:

* System Administrator (attached to the Plan license)
* Standard (attached to the Standard license)
* Light (attached to the Light license)
* Contributor (attached to the Contributor license)
* External User (attached to the External license)

The Workfront license for each default access level determines what is available and configurable in the access level. For information about the Workfront licenses, see [Adobe Workfront licenses overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Access levels define what assigned users can see and do with the following object types and areas in Workfront:

* Projects
* Tasks
* Issues
* Portfolios
* Reports, Dashboards, and Calendars
* Filters, Views, and Groupings
* Documents
* Other users
* Templates
* Financial Data
* Resource Management
* Scenario Planner 

In a custom access level, you can configure the settings for these objects and areas to change how much access users have to them. Depending on the license associated with the access level, as well as the type of the object or area, you can configure the access level to allow no access, view access, or edit access to an object or area.

>[!IMPORTANT]
>
>We strongly recommend that you leave the built-in access levels unchanged so that you can refer to them after you set up your users. To customize an access level, copy the default access level and modify the copy. (You can do this for every access level except for System Administrator and External User.)

For a detailed explanation of each of the default access levels, see [Built-in access levels in Adobe Workfront](#built-in-access)in this article. 

For instructions on assigning an access level to a user, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

### Permissions

When sharing an object with someone in the system, a user can grant the recipient any of the following permissions to the object.

* **View**: This level of permission allows the recipient to share the object in one of the following ways:

  * System-wide so that all users can see it (not available for all objects)
  * With external users who don't have a Workfront license (not available for all objects)
  * With an email address (available only for documents)

* **Contribute**: (not available for all objects)
* **Manage**: When someone shares an object, the recipient's rights to the object are determined by a combination of the recipient's access level and the permissions to the object that were granted by the sharer. The lowest degree of access available in that combination is what determines what the recipient can do with the object.

  >[!INFO]
  >
  >**Example:** If the recipient's access level doesn't allow project editing, that person can't edit or delete a project even if the sharer granted permissions to manage it.
  >
  >Or, if the recipient's access level allows project editing, but the sharer granted view-only permissions to a project, the user cannot edit or delete the project.

The following table compares a user's general access to objects (defined by the user's access level) to permissions for a specific shared object:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>&nbsp;</th> 
   <th>Access level </th> 
   <th>Permissions </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Granted by a Workfront administrator in the access level of a user</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Granted by a user sharing an object at the object level</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Inherited from a higher-ranking shared object 
   </td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* If a user shares an object with certain permissions and that object has any child objects below it, the recipient inherits the same permissions for those child objects. 
>* If an access level restricts users from deleting certain objects, this doesn't keep them from deleting child objects that are contained in those objects.
>

### More example scenarios

When Olivia shares a Workfront project with Tony, Tony's access to it is determined by a combination of two things:

* Tony's access level, assigned by the Workfront administrator
* Tony's permissions to the project, specified by Olivia

Tony's actions on the project can be further restricted on the project, but they cannot be unrestricted beyond what is allowed on his access level:

* If Tony's access level doesn't allow him to create tasks, he can't add tasks to the project , even if Olivia gave him permissions to add tasks to it.
* If Tony's access level does allow him to create tasks, but Olivia did not grant permissions to add tasks to the project, he can't add tasks to that project, but he can add tasks to other projects where he has been granted permissions to do so.
