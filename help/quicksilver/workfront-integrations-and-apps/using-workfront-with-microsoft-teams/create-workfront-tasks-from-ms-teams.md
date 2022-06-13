---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Create Adobe Workfront tasks from Microsoft Teams
description: You can create personal tasks in Adobe Workfront from Microsoft Teams if a team owner has installed and configured Workfront for Microsoft Teams for your team, and you are logged into Workfront from Microsoft Teams.
feature: Workfront Integrations and Apps
---

# Create Adobe Workfront tasks from Microsoft Teams

## Access requirements

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
   <td> <p>Work, Plan</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>[Insert any access level configurations needed]
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: Edit access to Documents
       </MadCap:conditionalText>
      </p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a group administrator. For more information on group administrators, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
     </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed and specify the object]
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: View access or higher on Documents
       </MadCap:conditionalText>
      </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

You can create personal tasks in Adobe Workfront from Microsoft Teams if the following conditions are met:

* A team owner has installed and configured Workfront for Microsoft Teams for your team.
* You are logged into Workfront from Microsoft Teams.

>[!NOTE]
>
>Microsoft Teams no longer supports Internet Explorer. To use the Adobe Workfront for Microsoft Teams integration, you must use a web browser other than Internet Explorer.

For information about installing Workfront for Microsoft Teams and logging in to Workfront from Microsoft Teams, see [Install Adobe Workfront for Microsoft Teams](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Create personal tasks from Microsoft Teams

1. Log in to Workfront from Microsoft Teams.

   For information about logging in to Workfront, see [Install Adobe Workfront for Microsoft Teams](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. To open a **New task** card:

   * If you are in the Workfront bot chat channel, type **New task** in the conversation field to create a new task.&nbsp;
   * If you are in a chat channel other than the Workfront bot chat channel:

      1. Start typing **@workfront** in the conversation field, then select the Workfront bot channel you want.
      1. Continue typing&nbsp;**New task** in the conversation field to create a new task.

         The New task card displays in the Workfront bot channel.

         ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. In the Workfront bot channel, specify the following information on the New task card:

   * Task name in the **Write the task's title** field.
   * Task description in the **Write the tasks's description** field.
   * The take the task must be completed by, in the **Due Date** field.

1. Click **Save.**&nbsp;

   The new personal task is created in Workfront. A Reference Number is assigned to it and visible on the new task card.

   For information about reference numbers, see the [Reference Numbers of objects](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects) section in the [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) article.

1. (Optional) Click **Edit** to edit the task information further.
1. (Optional) Click **View in Workfront** to open the task in a new tab in Workfront and edit the task further, move it to a project, or assign it to someone else.&nbsp;

