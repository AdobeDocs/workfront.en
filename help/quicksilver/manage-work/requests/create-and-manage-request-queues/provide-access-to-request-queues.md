---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Provide Access to Request Queues
description: When you provide access to a request queue, you determine who in your organization can view the request queue in the Requests area of Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/FG-KGqoEVFkHh6-n2h77HMfSfncJmWznEvViz1Zl-Uk
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
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Provide access to request queues

<!-- Audited: 6/2025 -->

When you provide access to a request queue, you determine who in your organization can view the request queue in the Requests area of Adobe Workfront.

You can provide different users access to a Request Queue depending on whether they're part of the project team, project group, or project company. You can also provide request queue access to everyone in the system. 

This is useful in organizations that invite external stakeholders into Workfront and wish to limit the access of users to specific areas. In this case, a request queue open just to the users associated with the company or group of the project limits visibility to external stakeholders. Giving access to anyone makes the request visible to both internal and external stakeholders.

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
   <p>Plan </p> </td> 
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

## Prerequisites

Before the request queue is available for users in the Requests area, you must create a project with the following settings:

* Designate it as a request queue. For more information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Update the Status of the project to Current.

## Provide access to a Request Queue

1. Go to the project where you want to provide access to the request queues.

   >[!NOTE]
   >
   >Only projects with a status of Current are visible in the Requests area.

1. Click **Queue Details** in the left panel. 
1. Select **Publish as Help Request Queue** to designate the project as a Request Queue. 
1. Select from the following options that appear:

   * **Anyone**: Any user can view and add requests to the request queue.
   * **People with view access to this project**: Users that have View permissions to the project can view and add requests to the request queue. 
   * **People in this project's company**: Users associated with the project's Company can view and add requests. The Company associated with the project is listed in parentheses next to this option. 
   * **People in this project's group**: Users associated with the project's Group can view and add requests. The Group associated with the project is listed in parentheses next to this option.

     Group queues are useful when several departments share a Workfront account to achieve unique organizational goals. Each department may have its own queues that members of other groups shouldn't be able to see.

     For information about who has permissions on a project see [Share a project in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md). 

     Groups and companies can be associated with the project when editing the project. For more information, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Click **Save**.
