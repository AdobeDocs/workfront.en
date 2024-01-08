---
title: How access levels and permissions work together
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,diagram,levels,permissions
navigation-topic: access-levels
description: The Adobe Workfront administrator determines what access level each user should have. That access level defines what users can see and do with object types and areas in the system.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
---
# How access levels and permissions work together

The Adobe Workfront administrator determines what access level each user should have. That access level defines what users can see and do with object types and areas in the system.

Also, users gain access to individual objects when other users share and grant certain permissions on those objects.

So, the activities a user can do with an object are defined by a combination of their access level and the permissions given to them for that project.

![](assets/security-model-hierachy.png)

For example, if your access level says that you can create tasks, but the permissions you receive on a specific project don't allow you to add tasks to it, you can't add tasks on the project even though you can create tasks elsewhere in Workfront.

This article explains how this combination works.

## Access level

The access level assigned to each user by a Workfront administrator is required for logging in to Workfront.

The default access levels are:

* System Administrator (attached to the Plan license)
* Planner (attached to the Plan license)
* Worker (attached to the Work license)
* Reviewer (attached to the Review license)
* Requestor (attached to the Request license)
* External User (attached to the External Email license)

The Workfront license for each default access level determines what is available and configurable in the access level. For information about the Workfront licenses, see [Adobe Workfront licenses overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

For the users who are assigned to it, an access level defines what they can see and do with the following object types and areas in Workfront:

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
* Workfront Goals

In a custom access level, you can configure the settings for these objects and areas to change how much access users have to them. Depending on the license associated with the access level, as well as the type of the object or area, you can configure the access level to allow no access, view access, or edit access to an object or area.

>[!IMPORTANT]
>
>We strongly recommend that you leave the built-in access levels unchanged so that you can refer to them after you set up your users. To customize an access level, copy the default access level and modify the copy. (You can do this for every access level except for System Administrator and External User.)

For a detailed explanation of each of the default access levels, see [Built-in access levels](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

For instructions on assigning an access level to a user, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Permissions

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

## More example scenarios

When Olivia shares a Workfront project with Tony, Tony's access to it is determined by a combination of two things:

* Tony's access level, assigned by the Workfront administrator
* Tony's permissions to the project, specified by Olivia

Tony's actions on the project can be further restricted on the project, but they cannot be unrestricted beyond what is allowed on his access level:

* If Tony's access level doesn't allow him to create tasks, he can't add tasks to the project , even if Olivia gave him permissions to add tasks to it.
* If Tony's access level does allow him to create tasks, but Olivia did not grant permissions to add tasks to the project, he can't add tasks to that project, but he can add tasks to other projects where he has been granted permissions to do so.
