---
title: Copy and submit requests
description: When you submit similar requests frequently you can copy an existing submitted request. In this case, you can copy an existing request, make minimal changes to it, and resubmit it as a new request.
author: Alina
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
---
# Copy and submit requests

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>-->

When you submit similar requests frequently you can copy an existing submitted request. In this case, you can copy an existing request, make minimal changes to it, and resubmit it as a new request.

## Access requirements

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

You must have a request that you or someone in your organization previously submitted to be able to copy it and resubmit it. If the request belongs to someone else, you must have at least access to View it to be able to copy and submit it as new.

## Considerations about copying and submitting requests as new

* You can only copy and submit submitted requests. You cannot copy drafted requests.
* You can copy and submit requests you originally submitted, or requests that others submitted and you have access to at least View.
* You always have access to copy and submit a copy of your own requests, unless someone removed your permissions to them.
* The access to copy and submit requests originally submitted by others might be granted automatically to people in the same company when the creator of the request queue enables the **People from the same company will inherit the same permissions for all requests** in the Queue Details or Edit Project areas. Disabling this setting allows only the original requestor to view their own requests.

  For more information, see the following articles:

   * [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) 
   * [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md)

* You can update the copy of the original request before resubmitting it as a new request.
* If the following changes occur after the original request is submitted, you can no longer copy it and resubmit it:

   * The request queue was deleted.
   * The queue topic was deleted.

     >[!TIP]
     >
     >If the queue topic was the only one in the request queue, you can still copy and submit the request and it will be saved under the request queue itself.

   * The request queue is no longer published as a Help Request Queue. For information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * If the request queue has no queue topic and the original request was submitted before January 2022.

   * The Status of the project associated with the request queue is no longer Current.

* You can copy and submit a copy of a converted request if the request was preserved in the conversion process. For more information, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >The copied request is not linked to a resolving object.

## Copy and submit requests

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Requests**.
1. (Conditional) If the Submitted section does not display by default, click **Submitted** in the left panel.
1. Locate the request that you want to copy and submit as new, and do one of the following:

   * Select it, then click **Copy** ![](assets/copy-and-submit-as-new-requests-area-nwe.png) in the upper-left corner of the Submitted requests list. 

   >[!TIP]
   >
   > If you did not select a request first, the Copy icon is dimmed. 

   * Click the **More** menu ![](assets/more-icon.png) to the right of the request name, then click **Copy and submit as new** 

     Or

     Right-click on the selected request, then click **Copy and submit as new**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >When you do not have access to create issues, you receive a warning that your administrator restricted you from creating requests.

1. (Optional) Update the following information, if needed:

   * **Request Type**: the request queue where the copied request is saved. By default, the copied request is saved to the request queue of the original request.
   * **Topic Groups** and **Queue&nbsp;Topics**, if they are selected. The names or topic groups and queue topics are customized for your environment. By default, the copied request is saved to the topic groups and the queue topics of the original request.

     >[!TIP]
     >
     >If the path changes from the path of the original request, then the creator of the request queue modified the queue.

1. (Optional) Update any information from the copied request. Depending on what fields the request queue creator enabled in the **New Issue Fields** section of the **Queue Details**&nbsp;subtab on the project, you might find&nbsp;any of the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Subject</strong> </td> 
      <td>Displays the name of the original request. Update it, if necessary.&nbsp;Otherwise, Workfront names the copied request <b>Copy of &lt;Name of original request&gt;</b>. This is a mandatory field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Displays the description of the original request. Update it, if necessary.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Displays the URL of the original request. Update it, if necessary.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong> </td> 
      <td> <p>Specify the priority of your request. The priority should define how fast you think this request should be resolved. The default&nbsp;options are:</p> 
       <ul> 
        <li>None</li> 
        <li>Low</li> 
        <li>Normal</li> 
        <li>High</li> 
        <li>Urgent</li> 
       </ul> <p>Your Workfront administrator can modify the names of priorities.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Severity</strong> </td> 
      <td> <p>Specify the severity for your request. The severity should define the impact this request has on your work should it not be resolved in time. The default&nbsp;options are:</p> 
       <ul> 
        <li>Cosmetic</li> 
        <li>Causes Confusion</li> 
        <li>Bug with workaround</li> 
        <li>Bug with no workaround</li> 
        <li>Fatal error</li> 
       </ul> <p>Your Workfront administrator can modify the names of severities.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Primary Contact</strong> </td> 
      <td>The Primary Contact of a request defaults to you, as you are the point person to address any questions pertaining to the request. However, you can change this to any other Workfront user.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Assignments</strong></span> </td> 
      <td> <p>Indicate the name of an active user, job role, or team that the request should be assigned to. </p> <p> You can specify more than one user, job role, or team. </p> <p>Depending on how the request queue was set up, you might be able to only assign the request to one or two types of resources, instead of all three. </p> <p>We recommend using Routing Rules for your Request Queues so that they can be automatically routed to the appropriate resources. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Depending on how the request queue was set up, you might be able to only assign one type of resource to the request (for example, users). If a routing rule is also associated to the request queue and it automatically routes the request to a different type of resource (for example, a team), your request is assigned to both the entity that you manually specify when submitting the request (users) and the resource specified in the routing rule (the team.)</p> <p style="font-weight: normal;">For more information, see the following articles:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Create Routing Rules</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Hours</strong> </td> 
      <td> <p>Estimate how many hours it would take for this request to complete.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Start Date</strong> </td> 
      <td> <p>The date when work on this request should start.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Completion Date</strong> </td> 
      <td>The date when you would like for this request to be resolved.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>The default status of a new request is "New." Your Workfront administrator might have changed the name of this&nbsp;status. You can also change the status to something else from this drop-down menu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documents</strong> </td> 
      <td> <p>Add documents to your request. The documents attached to the original request do not transfer to the copied request.</p> <p><b>TIP</b> 
      
      Depending on how the request queue was set up, the Documents section might display before or after the custom fields.</p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Update any information in the custom forms attached, if needed.

   >[!TIP]
   >
   >* All custom forms attached to the original request and the values included in the custom fields transfer to the copied request. This includes fields that contain logic.
   >* You cannot remove custom forms from the copied request.

1. Click **Submit**.

   The copied request is submitted as a new request in the request queue you specified.
