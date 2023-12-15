---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Overview of sharing permissions on objects
description: You can share or remove permissions to an object you created or an object that was shared with you.
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
---
# Overview of sharing permissions on objects

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
When sharing an object with someone in the system, you can grant the recipient any of the following permissions: view, contribute, and manage.

You do not have to be an Adobe Workfront administrator to share permissions on objects that you have access to, but your permissions on objects work within the access levels set by the Workfront administrator.

You can share or remove permissions to an object you created or an object that was shared with you. When you are not the creator of the object, you must have Share access on the object that you want to share in your access level in addition to Share permissions on the object. For information about access levels, see [New access levels overview](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) or [Access levels overview](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>A Workfront administrator can add or remove permissions to any items in the system, for all users, without being the owner of those items.

## Objects that you can share in Workfront

You can share the following objects in Workfront with other users:

* **Projects**: For more information, see [Share a project in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Templates**: For more information, see [Share project templates](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolios**: For more information, see [Share a portfolio](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

* **Programs**: For information, see [Share a program](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **Tasks**: For information, see [Share a task](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Issues**: For information, see [Share an issue](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Documents**: For information, see [Share a document](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Document Folders**: For information, see [Share a document folder](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Proofs**: For information, see [Share a Proof within Workfront](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md). 

* **Reports, dashboards, and calendars**: For information, see [Share reports, dashboards, and calendars](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).&nbsp;Additionally, see the following articles:

   * [Share a report in Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Share a dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Share a calendar report](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filters, views, and groupings**: For information, see [Share a filter, view, or grouping](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md). 

* **Plans**: For information, see [Share a plan in the Scenario Planner](../../scenario-planner/share-a-plan.md).

  This requires an additional license.

* **Goals**: For information, see [Share a goal in Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  This requires an additional license.

## Considerations about sharing objects

* You can share only the same level or a lower level of permissions you have on the object.

  For example, if you have Contribute permissions on the object, you cannot grant another user Manage permissions on that object.

* You cannot share an object with a permission level higher than the access level of a user. 

  For example, if a user has View access to Projects in their access level, you cannot give them Manage permissions on a project. 
* A user with permissions to at least View an object can share that object with someone else.
* You can share objects with active users, job roles, teams, groups, or companies.

  >[!NOTE]
  >
  >You can share a plan or a goal only with other active users. This requires additional licenses.
  >
  >
  >For more information see:
  >
  >* [Share a plan in the Scenario Planner](../../scenario-planner/share-a-plan.md) 
  >* [Share a goal in Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md) 

## Share limitations

You can share an object with up to 100 entities (users, teams, groups, job roles, companies). We recommend that you share objects with groups, teams, or companies rather than with individual users to avoid this limitation.

## Share permissions for objects

The following table illustrates the level of permissions that you can select when sharing an object. Not all objects have all these settings available. You can grant another entity permissions to View or Manage an object. If you are sharing a project, task, or issue, you can also grant permissions to Contribute to it.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>View</strong></td> 
   <td> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li><p>View the object</p></li> 
     <li><p>Add documents to the object</p></li> 
     <li><p>View Finance information about the object</p></li> 
     <li> <p>Share the object<br></p> <p>When you share the object, you can grant other users the same permission level you have only on the object, not a higher level.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Contribute</strong></td> 
   <td> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>All the actions included with the View permission.</li> 
     <li>Add Expenses to it</li> 
     <li>Add issues to it (if it is a task or a project)</li> 
     <li>Add tasks to it (if it is a project)</li> 
     <li>Edit Custom Forms on it</li> 
     <li>Log Hours on the object</li> 
     <li>Make assignments in it</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Manage</strong></td> 
   <td> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>All the actions included with the View and Contribute permissions</li> 
     <li>Delete it</li> 
     <li>Manage Finance information in it</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Make this public to external users</strong></td> 
   <td> <p>Anyone without a Workfront account can view the object by clicking a link to it. This is not available for all objects.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Make this visible system-wide</strong></td> 
   <td> <p>The object can be found in searches and viewed by anyone with a Workfront account.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Understand inherited permissions and the hierarchy of objects

### Permissions inherited from parent objects {#permissions-inherited-from-parent-objects}

Permissions in Workfront are inherited hierarchically. This means that if you are granting permissions to a user on a parent object, they gain the same permissions on the children objects associated with it by default.

For example, if you give a user Contribute permissions to a project, the user has Contribute permissions to all tasks and issues (child objects) associated with that project.

Continuing with the example above, you cannot restrict permissions to child objects. If you do not want the user to have Contribute permissions to child objects associated with the project, you must manually remove the Inherited Permissions from the objects and then adjust the permissions for the individual user, including any Advanced Settings.&nbsp;

For more information about the hierarchy and interdependency of objects in Workfront, see the section [Interdependency and hierarchy of objects](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) in the article [Adobe Workfront objects overview](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Your Workfront administrator can disable inherited permissions for documents in your access level.&nbsp;For more information about disabling inherited permissions for documents in the access level, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Permissions acquired through organizational memberships&nbsp; {#permissions-acquired-through-organizational-memberships}

If you grant Manage permissions to a Group of users on an object, and you grant View permissions to an individual user in that Group on the same object, the user has the highest level of permissions (Manage) granted through the Group membership on the object.&nbsp;

If you want to grant lower permissions to a user who is already part of an organizational unit (Group, Team, Job Role, or Company) with a higher permission level, you must remove the permissions from the organizational unit, and add users individually with a lower level of permissions.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Share an object

For information about how to share objects, see [Share an object](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Remove permissions from objects

For information about how to remove permissions from objects, see [Remove permissions from objects](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Request permissions to objects

When someone sends you a link to an object which you do not have permissions to View, or when you have lower permissions on an object and you want to request a higher level of permissions, you can request permissions on the object.&nbsp;

You can request access to an object from anyone who has Share permission to the object.&nbsp;

For more information about requesting permissions to objects, see [Request access to objects](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
