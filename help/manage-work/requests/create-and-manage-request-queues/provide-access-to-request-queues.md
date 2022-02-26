---
filename: provide-access-to-request-queues
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Provide access to request queues
description: When you provide access to a request queue, you determine who in your organization can view the request queue in the Requests area of Adobe Workfront.
---

# Provide access to request queues

When you provide access to a request queue, you determine who in your organization can view the request queue in the Requests area of *Adobe Workfront*.

You can provide different users access to a Request Queue, depending on whether they are part of the project team, project group, or project company. You can also provide access to everyone in the system to a request queue.&nbsp;

This is useful in organizations that invite external stakeholders into *Workfront* and wish to limit the access of users to specific areas — in this case a request queue open just to the users associated with the company or group of the project limits visibility to external stakeholders. Giving access to anyone makes the request visible to both internal and external stakeholders.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*

## Prerequisites

Before the request queue is available for users in the Requests area, you must create a project with the following settings:

* Designate it as a request queue. For more information about creating a Request Queue, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Update the Status of the project to Current.

## Provide access to a Request Queue

<ol> 
 <li value="1"> <p>Go to the project where you want to provide access to the request queues. </p> <note type="note">
   Only projects with a status of Current are visible in the Requests area. 
  </note> </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click&nbsp;<span class="bold">Queue Details</span> in the left panel. You might need to click&nbsp;<span class="bold">Show More</span>, then <span class="bold">Queue Details</span>. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click&nbsp;<span class="bold">Queue Details</span> in the left panel. You might need to click&nbsp;<span class="bold">Show More</span>, then <span class="bold">Queue Details</span>. </p> </li> 
 <li value="3"> <p>Select <span class="bold">Publish as Help Request Queue</span>&nbsp;to designate the project as a Request Queue.</p> </li> 
 <li value="4"> <p>Select from the following options:</p> 
  <ul> 
   <li><span class="bold">Anyone</span>: Any user can view and add requests to the request queue.</li> 
   <li><span class="bold">People with view access to this project</span>:&nbsp;Users that have View permissions to the project can view and add requests to the request queue.&nbsp;</li> 
   <li><span class="bold">People in this project's company</span>:&nbsp;Users associated with the project's Company&nbsp;can view and add requests. The Company associated with the project is listed in parentheses next to this option.&nbsp;</li> 
   <li> <p><span class="bold">People in this project's group</span>:Users associated with the project's Group can view and add requests. The Group&nbsp;associated with the project is listed in parentheses next to this option.</p> <p>Group queues are useful when several departments share a <em>Workfront</em> account to achieve unique organizational goals. Each department may have its own queues that members of other groups should not be able to see.</p> <p>For information about who has permissions on a project see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.<br>Groups and companies can be associated with the project when editing the project. For more information about editing projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li> 
  </ul> </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

