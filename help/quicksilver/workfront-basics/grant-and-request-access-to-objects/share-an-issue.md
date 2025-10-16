---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Share an issue
description: Your Adobe Workfront administrator grants users access to view or edit issues when they assign access levels. For more information about granting access to issues, see Grant access to issues.
author: Courtney
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
---
# Share an issue

Your Adobe Workfront administrator grants users access to view or edit issues when they assign access levels. For more information about granting access to issues, see [Grant access to issues](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md).

Along with the access level that users are granted, you can also grant them permissions to View, Contribute, or Manage specific issues that you have access to share. For more information about access levels and permissions, see [How access levels and permissions work together](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Permissions are specific to one item in Workfront and define what actions one can take on that item.


## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p> 
   <p>Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View access or higher to the objects you want to share</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations about sharing issues

In addition to the considerations below, also see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>A Workfront administrator can add or remove permissions to any items in the system, for all users, without being the owner of those items.

* The creator of an issue has Manage permissions for it by default.
* You can share issues individually, or you can share several of them at a time. Sharing issues is identical to sharing other items in Workfront. For more information about sharing items in Workfront, see [Share an object](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md). 
* You can grant the following permissions to an issue:&nbsp;

   * View
   * Contribute  
   * Manage

* When you share an issue, all the documents attached to the issue inherit the same permissions.

  The Workfront administrator can specify whether documents should inherit permissions from higher objects in the user's access level. For more information about restricting inherited permissions on documents, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* You can remove inherited permissions from an issue. For more information, see [Remove permissions from objects](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Ways to share an issue

* Manually, which is similar to sharing any other object in Workfront. 
* Automatically, by doing one of the following:

   * Specify the permissions on any of the parent objects of the issue: project, program, or portfolio. Issues inherit the permissions from their parent objects. For information about viewing inherited permissions on objects, see [View inherited permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md). 
   * Add entities to Project Sharing on a template used to create the project the issue is on. For information about sharing projects from templates, see [Share a template](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Specify the permissions on all issues in a project when you edit the project. For information about managing the access to issues or requests on the project based on a user's permissions to the project, see the [](../../manage-work/projects/manage-projects/edit-projects.md#access) section in the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >If you don't specify what issue permissions you want users to have when they are assigned to the issues on the project, they receive the same permissions they have on the project by default.

   * Specify the permissions users receive on issues they submit in a request queue when creating a request queue. For information, see [Create a Request Queue](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

     >[!IMPORTANT]
     >
     >Permissions are granted differently depending on whether or not the project is published as a request queue:
     >
     >   
     >   
     >   * When a user submits a request to a project published as a request queue, the Primary Contact and Entered By users are granted the permission specified.
     >   * When a user submits a request to a project not published as a request queue, the Primary Contact (if different from Entered By user) is granted the permission specified, and the Entered By user is granted Manage permissions to the issue.
     >   
     >

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue at the project level</h2>
<p>(NOTE: this info duplicates in Edit projects - linked there instead (above).)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are added to a project.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2"> Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. </li>
<li value="3">In the <strong>Edit Project</strong> box that displays, click <strong>Access</strong>.</li>
<li value="4">In the <strong>When someone is assigned to an ISSUE</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><strong>Manage</strong><br>Now, when someone is assigned to an issue on the selected project, they are granted the specified permissions to the issue.&nbsp;</li>
</ul></li>
<li value="5">(Optional) Select the <strong>Also grant ... access to the project</strong> field to also grant View, Contribute, or Manage permissions to the projects to the user assigned to the issue</li>
<li value="6">In the <strong>When someone submits a REQUEST ...</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><p><strong>Manage</strong></p><note type="important">
<p>Permissions are granted differently depending on whether or not the project is published as a request queue:</p>
<ul>
<li>When a user submits a request to a project published as a request queue, the Primary Contact and Entered By users are granted the permission specified.</li>
<li>When a user submits a request to a project not published as a request queue, the Primary Contact (if different from Entered By user) is granted the permission specified, and the Entered By user is granted Manage permissions to the issue.</li>
</ul>
</note></li>
</ul></li>
<li value="7"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong> field.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="8">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue in request queues</h2>
<p>(NOTE: drafted because it's duplicated from Create a Request Queue which is linked above)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are submitted to a request queue.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2">Click <strong>Edit Project</strong>.</li>
<li value="3">Click <strong>More</strong> then click <strong>Queue Setup</strong>. </li>
<li value="4"> <p>On the <strong>Queue Details</strong> sub-tab, in the drop-down menu under <strong>When someone makes a request, automatically grant</strong>, select from the following permissions levels:</p>
<ul>
<li><strong>View Access</strong> </li>
<li><strong>Contribute Access</strong> </li>
<li> <p><strong>Manage Access</strong> </p> </li>
</ul> <p>Now, when someone submits a request to the selected project, they are granted the specified permissions to the request.</p> </li>
<li value="5"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong>.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Share an issue

1. Navigate to the issue you want to share.

1. To the right of the issue name, click **Share**. The **Share [Issue Name]** dialog box opens.

    ![Share issue button](assets/share-issue-button.png)

1. In the **Grant issue access to** field, begin typing the name of the user, team, role, group, or company you want to share the issue with, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >You can only share an issue with active users, teams, roles, or companies.


1. (Optional) Select the **Who has access** drop-down and select the issue's access level:

   * **Only invited people can access:** Only users who are invited to the issue can access it (Default).
   * **Everyone in the system can view**: All users in the system can view the issue without an invitation.

1. Click the drop-down to the right of the user's name and select their permission level for this issue:

   * **View**: User can review and share the issue. 
   * **Contribute**: User can make updates, log information, make minor edits, and share the issue (also includes all View permissions).
   * **Manage**: User has full access to the issue without administrative rights, which are granted at the access level (also includes all View and Contribute permissions).

1. (Optional) Click the advanced options icon next to the permission level you've granted to configure specific permissions on the issue.

    ![Configured advanced permission options](assets/advanced-permission-options.png)

1. (Optional) To quickly share the issue using a link, click **Copy link** and then forward it to the recipient.

1. Click **Save**.

## Share issues in bulk 

1. Navigate to the project that contains the issues you want to share. 

1. In the **Issues** tab on the project page, select the box to the left of each issue you want to share, then click the **Share** icon ![Share icon](assets/share-icon.png) at the top of the page. The share modal opens.

    ![Bulk share issues](assets/bulk-share-issues.png)

1. In the **Grant issue access to** field, begin typing the name of the user, team, role, group, or company you want to share the issues with, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >You can only share issues with active users, teams, roles, or companies.


1. (Optional) Select the **Who has access** drop-down and select the issues' access level:

   * **Only invited people can access:** Only users who are invited to the issues can access them (Default).
   * **Everyone in the system can view**: All users in the system can view the issues without an invitation.


1. Click the drop-down to the right of the user's name and select their permission level for the issues:

   * **View**: User can review and share the issues. 
   * **Contribute**: User can make updates, log information, make minor edits, and share the issues (also includes all View permissions).
   * **Manage**: User has full access to the issues without administrative rights, which are granted at the access level (also includes all View and Contribute permissions).

1. (Optional) Click the advanced options icon next to the permission level you've granted to configure specific permissions on the issues.

    ![Configured advanced permission options](assets/advanced-permission-options.png)

1. Click **Save**.

## Issue permissions

The following table displays what permissions you can grant users when allowing them to View, Contribute, or Manage an issue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Actions</strong> </td> 
   <td><strong>Manage</strong> </td> 
   <td><strong>Contribute</strong> </td> 
   <td><strong>View</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>Add issues</p> </td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Delete&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Attach Custom Form</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Edit Custom Fields</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Approve Issue</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Add An Approval Process</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Add Documents</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Copy Issue*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Move Issue</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Log Hours</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Convert to Project*</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Accept Assignment</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Updates/ comments</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modify Planned Dates</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Make Assignments</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Share</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Share System-wide</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Controlled by the access levels and the permissions on the project.
