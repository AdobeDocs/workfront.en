---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Define Request Types for a Project
description: You can organize the kind of issues or requests that are logged in Adobe Workfront by Request Types.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fOdoie2wI-EHoKmQTHy0cDaVipi6XYE1JgMHdX6-Tbo
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
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Define Request Types for a project

<!-- Audited: 6/2025 -->

You can organize the kind of issues or requests that are logged in Adobe Workfront by Request Types. This is useful for reporting reasons and helping users understand what kind of unexpected work might occur during the lifetime of a project.

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
   <td>
    <p>Standard</p>
    <p>Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you begin, you must do the following: 

* Have or create a project.

  For information about creating projects, see [Create a project](../../../manage-work/projects/create-projects/create-project.md).

## Considerations about Request Types

* You can specify the type of issues or requests that can be logged on a project when you configure the Queue Details area for the project.
* You don't have to enable the project to be a request queue to be able to define Request Types for a project. Any issues logged for a project can be labeled with a different Request Type. 
* If you add Queue Topics to your project, you must define Request Types on each queue topic to display it when adding a new issue or request. For more information, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Define the issue or request types for a project

{{step1-to-projects}}

1. On the **Projects** page, select a project.
1. In the left panel, click **Queue Details**. 
1. In the **Queue Properties** section, select the **Request Types** you want for the project:
   * Bug Report
   * Change Order
   * Issue
   * Request

   >[!NOTE]
   >
   >* You must have at least one request type selected. You can select multiple types.
   >* Your Workfront administrator might have renamed some of these options. For information, see [Configure request types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Click **Save**. The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project (if the project is enabled as a request queue).
