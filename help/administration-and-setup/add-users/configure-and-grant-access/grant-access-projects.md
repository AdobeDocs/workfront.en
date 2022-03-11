---
filename: grant-access-projects
title: Grant access to projects
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
title: Grant access to projects
description: As an Adobe Workfront administrator, you can use an access level to define a user’s access to projects in Workfront, as explained in Access levels overview.
---

# Grant access to projects

As an `Adobe Workfront administrator`, you can use an access level to define a user’s access to `projects`, as explained in [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).&nbsp;

For information about using custom access levels to manage users' access to other object types in `Workfront`, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure user access to projects using a custom access level

<ol> 
 <li value="1">Begin creating or editing the access level, as explained in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</li> 
 <li value="2"> <p>Click the gear icon <img src="assets/gear-icon-settings.png"> on the <span class="bold">View</span> or <span class="bold">Edit</span> button to the right of <span>Projects</span>, then select the abilities you want to grant under <b>Fine-tune your settings</b>.</p> <p> <img src="assets/planner-fine-tune-your-settings-with-copy-projects-350x93.png" style="width: 350;height: 93;"> </p> <note type="note"> 
   <ul> 
    <li>Users with a Work license have limited project rights. They can contribute to a project, but not manage one.</li> 
    <li>Users with a Review license have View rights on projects from converted issues, but their View rights are limited.</li> 
    <li> <p>For information about permissions users can grant when sharing projects with others, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> </li> 
    <li> <p>When you configure an access level setting for a certain type of object, that configuration doesn't affect the users' access to objects with a lower rank. For example, you can restrict users from deleting <span>projects</span> in their access level, but this does not restrict them from deleting <span>tasks</span>, which are lower-ranking than <span>projects</span>.For more information about the hierarchy of objects, see the section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref" data-mc-variable-override="">Interdependency and hierarchy of objects</a> in&nbsp;the article <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref" data-mc-variable-override="">Understand objects in Adobe Workfront</a>.</p> </li> 
   </ul> 
  </note> </li> 
 <li value="3"> <p>(Optional) Click <span class="bold">set sharing defaults</span> to the right of the Create option, then <span class="bold">Add Rule</span> to add a sharing rule for new projects.</p> <p>When the user with this access level creates a project, the project is shared automatically with the users you select in the menu on the left. </p> <p> <img src="assets/project-sharing-menu-350x230.png" style="width: 350;height: 230;"> </p> <p>In the menu on the right, you specify how you want the project shared with those users:</p> <p> <img src="assets/project-sharing-right-menu-350x234.png" style="width: 350;height: 234;"> </p> <note type="note">
    If a user with this access level is using a project access template, the template overrides the sharing settings in the access level. For information about project access templates, see 
   <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.
  </note> <p>You can repeat this step to add as many project sharing rules as you need for the access level.</p> </li> 
 <li value="4">Click the X to close the <span class="bold">Fine-tune your settings</span> box.</li> 
 <li value="5"> <p>(Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref" data-mc-variable-override="">Configure access to Adobe Workfront</a>, such as <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref" data-mc-variable-override="">Grant access to tasks</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref" data-mc-variable-override="">Grant access to financial data</a>.</p> </li> 
 <li value="6"> <p>When you are finished, click Save.</p> <p>After the access level is created, you can assign it to a user. For more information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Edit a user's profile</a>.</p> </li> 
</ol>

## Access to reports, dashboards, and calendars by license type

For information about what users in each access level can do with issues, see the section [Projects](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) in the article [Functionality available for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Access to shared projects

As the owner or creator of an issue, you can share with other users by granting them permissions to it, as explained in [Share a project in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

When you share any object with another user, the recipient’s rights on it are determined by a combination of two things:

* The permissions that you grant to your recipient for the object
* The recipient’s access level settings for the object's type

##  

