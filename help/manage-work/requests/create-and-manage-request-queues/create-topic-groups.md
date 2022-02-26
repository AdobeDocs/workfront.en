---
filename: create-topic-groups
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Create Topic Groups
description: Topic Groups are associated with Request Queues. They allow you to layer your Request Queues in multiple categories, depending on the nature of the requests.
---

# Create Topic Groups

Topic Groups are associated with Request Queues. They allow you to layer your Request Queues in multiple categories, depending on the nature of the requests.

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
   <td role="rowheader"> <p role="rowheader"><em>Adobe Workfront</em> license*</p> </td> 
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

## Overview of Topic Groups

For example, if you have a Request Queue for Marketing Requests, you can have a Topic Group of "Mother's Day Campaign", with a second-level Topic Group of "Digital Media", and an additional second-level Topic Group of "Print Media." Then, you can have multiple Queue Topics inside each Topic Group. For example, "Banner Ad" and "Blog" can be Queue Topics for the "Digital Media" Topic Group.

For more information about how to create Request Queues, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

` `**Tips: **``

* You can create up to 10 tiers of Topic Groups within a Request Queue.
* There is no limit to the number of Queue Topics that can be associated with a topic group. 
* Topic groups are a reportable object.

## Create Topic Groups

We recommend that you create Topic Groups before you create a Queue Topic. However, a Topic Group can be created within in the Queue Topic builder. For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

To create a Topic Group:

<ol> 
 <li value="1"> Go to the project that you published as a Help Request Queue.<br>For more information about publishing a project as a Help Request Queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Topic Groups</span> in the left panel. You might need to click <span class="bold">Show More</span>, then <span class="bold">Topic Groups</span>. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Topic Groups</span> in the left panel. You might need to click <span class="bold">Show More</span>, then <span class="bold">Topic Groups</span>. </p> </li> 
 <li value="3"> Click <span class="bold">New Topic Group</span>.<br><img src="assets/10-350x170.png" alt="" style="width: 350;height: 170;"></li> 
 <li value="4"> Specify the following information: 
  <ul>
   <li><span class="bold">Name</span>: The name is visible to users who submit requests to this request queue. </li>
   <li><span class="bold">Description</span>: The description displays when users select the topic group in the process of submitting a new request. </li>
   <li><span class="bold">Add to Topic Group</span>: You can add the new Topic Group to an existing Topic Group, or you can add it directly to the project published as a Help Request Queue. </li>
  </ul></li> 
 <li value="5"> Click <span class="bold">Save</span>.<br>This creates a new Topic Group in your Request Queue. You can now select additional categories from the first drop-down menu under a Request Queue.<br>For more information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>.</li> 
</ol>

