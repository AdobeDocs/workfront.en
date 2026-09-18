---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Create Topic Groups
description: Topic Groups are associated with Request Queues. They allow you to layer your Request Queues in multiple categories, depending on the nature of the requests.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/7odH8kf-VPRXoOVlMEiX3dWFLTsDDuy-f4TJgHAUsk8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
    internal-label: Requests
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create Topic Groups

<!-- Audited: 2/2024 -->

Topic Groups are associated with Request Queues. You can layer your Request Queues in multiple categories, depending on the nature of the requests by using topic groups.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license</p> </td> 
   <td>   
      <p>Standard</p>
      <p>Plan</p>
 </td> 
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

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Overview of Topic Groups

For example, if you have a Request Queue for Marketing Requests, you can have a Topic Group of "Mother's Day Campaign", with a second-level Topic Group of "Digital Media", and an additional second-level Topic Group of "Print Media." Then, you can have multiple Queue Topics inside each Topic Group. For example, "Banner Ad" and "Blog" can be Queue Topics for the "Digital Media" Topic Group.

For more information about how to create Request Queues, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Consider the following when working with topic groups: 

* You can create up to 10 tiers of Topic Groups within a Request Queue.
* There is no limit to the number of Queue Topics that can be associated with a topic group. 
* Topic groups are a reportable object.
* You cannot move topic groups from one project to another.

## Create Topic Groups

We recommend that you create Topic Groups before you create a Queue Topic. However, a Topic Group can be created within in the Queue Topic builder. For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

To create a Topic Group:

1. Go to the project that you published as a Help Request Queue.  
   For more information about publishing a project as a Help Request Queue, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Click **Topic Groups** in the left panel. 
1. Click **New Topic Group**.

   <!--   ![New topic group box](assets/new-topic-group-box-nwe-350x306.png) -->

1. Specify the following information:

   * **Name**: The name is visible to users who submit requests to this request queue. 
   * **Description**: The description displays when users select the topic group in the process of submitting a new request. 
   * **Add to Topic Group**: You can add the new Topic Group to an existing Topic Group, or you can add it directly to the project published as a Help Request Queue.

1. Click **Save**.  
   This creates a new Topic Group in your Request Queue. You can now select additional categories from the first drop-down menu under a Request Queue.  
   For more information about submitting requests, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. To edit an existing Topic Group, select the Topic Group from the Topic Groups list, then edit the details in the window that opens. Click **Save** to save the changes.
