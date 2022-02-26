---
filename: create-routing-rules
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Create Routing Rules
description: Routing Rules control what Adobe Workfront does with issues when they are submitted to a Request Queue. For more information about creating Request Queues, see Create a Request Queue.
---

# Create Routing Rules

Routing Rules control what *Adobe Workfront* does with issues when they are submitted to a Request Queue. For more information about creating Request Queues, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Routing Rules send issues to specific users or job roles best equipped&nbsp;to resolve the submitted issue or request. Routing rules are usually associated with queue topics,&nbsp;which are used to control which routing rule will be applied to the issue or request.

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

## Create a Routing Rule

<ol> 
 <li value="1">Go to the project which you want to add the routing rules for your requests. </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Routing Rules</span> in the left panel. You might need to click <span class="bold">Show More</span>, then&nbsp;<span class="bold">Routing Rules</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Routing Rules</span> in the left panel. You might need to click <span class="bold">Show More</span>, then&nbsp;<span class="bold">Routing Rules</span>.</p> </li> 
 <li value="3">Click <span class="bold">New Routing Rules</span>&nbsp;to add the new rule.&nbsp; </li> 
 <li value="4"> <p>Specify the following information for the Routing Rule:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>&nbsp;</th> 
     <th>&nbsp;</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Name</span> </td> 
     <td> <p>The name of the&nbsp;Routing Rule. You can see the Routing Rule if you have access to see this information on the project.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Description</span> </td> 
     <td>Add a description for the Routing Rule.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Default Assignee*</span> </td> 
     <td>Add an active user or an <span data-mc-edit-date="2021-05-27T11:52:45.4165986-04:00" data-mc-editor="alinawilson" data-mc-comment="yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-05-25T13:04:12.7687137-04:00">active</span> job role&nbsp;to whom the new issues should be assigned. You can only have one default assignee in this field. </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Default Team*</span> </td> 
     <td>Add an active team to whom the new issue should be assigned. You can only have one team assigned to the issue. </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Route to Project</span> </td> 
     <td>This is the project where the issue is added.</td> 
    </tr> 
   </tbody> 
  </table> <note type="note">
   *If a user, 
   <span>job role</span>, or team are deactivated after they are associated with a routing rule, the requests continue to be routed to them. You must periodically take an inventory of all routing rules and replace deactivated assignments with active ones. 
  </note> <p>When you route an issue to a project, users with permissions on the issue receive the permissions set on that project. For information about setting permissions on projects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> </li> 
 <li value="5">Select<span class="bold">&nbsp;Save</span>&nbsp;when done.<br>This process only defines&nbsp;the Routing Rule. To ensure that the issue is routed when it is submitted to the Request Queue, you must&nbsp;select the routing&nbsp;rule&nbsp;on the <span class="bold">Queue Details</span> tab under&nbsp;<span class="bold">Default Route</span>. For information about adding a Default Route to a Request Queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>.<br>If you want to associate multiple routing rules with the Request Queue, you must create multiple Queue Topics and associate each one with a separate Routing Rule. For more information about creating a queue topic, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>.</li> 
</ol>

