---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Create Queue Topics
description: Queue Topics work in conjunction with Routing Rules to automatically assign incoming work to a user, job role, team, or to place it on a project. Queue Topics define the conditions that need to exist for the Routing Rule to be implemented.
author: Alina
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
---
# Create Queue Topics

<!-- Audited: 12/2023 -->

Queue Topics work in conjunction with Routing Rules to automatically assign incoming work to a user, job role, team, or to place it on a project. Queue Topics define the conditions that need to exist for the Routing Rule to be implemented.

There is no limit to the number of Queue Topics that can be assigned to a Topic Group or to a project. Queue Topics are a reportable object type.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<!--drafted - replace table with P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
    <p>New: Standard</p>
    <p>or</p>
    <p>Current: Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create a Queue Topic

1. Create a Routing Rule, a Topic Group, and a custom form, if you plan to associate them with your Queue Topic.   
   For more information on how to create Routing Rules, Topic Groups or custom forms, refer to the following articles:

   * [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md) 
   * [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md) 
   * [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. Go to the project you chose to enable as a Help Request Queue and where you want to create a new queue topic.  
   For more information on how to designate a project as a Help Request Queue, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   You can organize related Queue Topics under a Topic Group. This will provide the requestor a series of drop-down menus when making a request.
   
   Or
    
   You can nest the Queue Topics directly under the project designated as a Help Request Queue, without a Topic Group.

   For information about creating Topic Groups, see [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Click **Queue Topics** in the left panel. You might need to click **Show More**, then **Queue Topics**. 
1. Click **New Queue Topic**.
1. On the **New Queue Topic** form, enter the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> Name of the Queue Topic.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Describe the Request Queue. The description displays when users select the queue topic in the process of submitting a new request. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add to Topic Group</strong> </td> 
      <td> If there are no Topic Groups on the project, the name of the project defaults as a Topic Group.<br>If you want to create additional Topic Groups from here, select <strong>Create New Topic Group</strong> from the drop-down menu.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom Forms</strong> </td> 
      <td>Select any custom forms you want to associate with the queue topic. You must create custom forms for issues before you can associate them with queue topics. For information about creating custom forms, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Default Approval</strong></td> 
      <td> <p>Associate an approval process with this queue topic. Only Issue Approval Processes are visible in this drop-down menu. All issues submitted to this queue will be associated with this Approval Process. Your Adobe Workfront administrator must define system-level Approval Processes before you can associate them with queue topics. <span>A user with administrative access to Approval Processes can also create group-specific approval processes.</span> For more information about creating Approval Processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.<br></p> 
       <div> 
        <p>Important: If the group of the project changes, the group-specific approval process attached to existing issues becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>.</p> 
        <p>Consider the following when adding approval processes to queue topics: </p> 
        <ul style="list-style-type: circle;"> 
         <li>Only active approval processes display in the list. </li> 
         <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Default Duration</strong> </td> 
      <td>This is the default duration of the request, and the Planned Completion Date of the request is calculated based on this value.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Default Route</strong> </td> 
      <td>Specify the routing rule you want to associate with the Queue Topic. You must create the routing rule before you can attach it to a Queue Topic. For information, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">Create Routing Rules</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Request Types</strong> </td> 
      <td> <p>Choose what kind of requests this queue topic stores. The visible options are set on the <strong>Queue Details</strong> tab of the project. This is a required field. </p> 
      
      <p><b>NOTE</b>:

      Types display as a selection in the Requests area only if the Request Type is selected in both the Queue Details and the Queue Topic pages. For information about setting up the Queue Details area of a project, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> <p>Select from the following types:</p> 
       <ul> 
        <li>Bug Report</li> 
        <li>Change Order</li> 
        <li>Issue</li> 
        <li>Request</li> 
       </ul> <p>Your Workfront administrator might have renamed some of these options. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![New Queue Topic box](assets/new-queue-topic-box.png)

1. Click **Save**.   
   The Queue Topic is now available to use and is visible in the Requests area of Workfront, after a Request Queue and a Topic Group are selected.
