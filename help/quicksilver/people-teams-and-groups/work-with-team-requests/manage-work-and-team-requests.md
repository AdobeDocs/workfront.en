---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Manage Work and Team Requests
description: A request represents a pending task or issue assignment. Work requests are made to individuals, and team requests are made to teams.
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
---
# Manage work and team requests

A request represents a pending task or issue assignment. Work requests are made to individuals, and team requests are made to teams.

>[!NOTE]
>
>Agile teams do not have team requests.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>To assign or work on a request:
   <p>New: Light or higher</br>
    or</br>
   Current: Review or higher</p>
   <p>To reassign a request:
   <p>New: Standard</br>
    or</br>
   Current: Work or higher</p></td>
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Assign a request to a team {#assign-a-request-to-a-team}

Project managers and issue requestors can assign work to teams when they do not know which resource is right to do the work or when it does not matter who completes the work.

Tasks assigned to the team remain on the [!UICONTROL Team Requests] tab until a user on the team volunteers to work on the request.

When a request is assigned to both a team and a user who is not a member of the team, the request is visible in both the [!UICONTROL Team Requests] tab and in the user's work requests area. If the user who is not on the team volunteers to work on the task, the task still remains in the [!UICONTROL Team Requests] tab until a user on the team volunteers to work on it.

Teams can be assigned to tasks and issues in any of the following ways:

* Through the [!UICONTROL Gantt Chart]
* From a task or issue list (individually or in bulk)
* When a task or issue is created or modified
* Through routing rules on a request (issues only)

You can manually assign a request to a team from the team page, as described in this section.

To manually assign a request to a team from the team page:

{{step1-to-team}}

1. Click the **[!UICONTROL Switch team]** icon ![Switch team icon](assets/switch-team-icon.png), then either select a new team from the drop-down menu or search for a team in the search bar.

1. Click the **[!UICONTROL More]** icon ![](assets/more-icon.png), then select **[!UICONTROL Send work request]**.

   ![](assets/edit-team-settings-350x205.png)

1. Fill in the information in the box that opens.
1. Click **[!UICONTROL Send Request]**.  
   The team is now assigned a new task which is displayed on the Team Requests tab. This task is not currently associated with a project, but it can be moved, as described in [Move tasks](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Reassign requests {#reassign-requests}

You can reassign requests that have been assigned to your team:

{{step1-to-team}}

1. Click the **[!UICONTROL Switch team]** icon ![Switch team icon](assets/switch-team-icon.png), then either select a new team from the drop-down menu or search for a team in the search bar.
1. In the left navigation panel, select **[!UICONTROL Team Requests]**.
1. Click the **[!UICONTROL Reassign]** icon.  

1. Begin typing the name of the user, group, or team who you want to reassign the request to, then click **[!UICONTROL Assign]**.  
   The request is reassigned.
