---
filename: create-workfront-tasks-from-ms-teams
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Create Adobe Workfront tasks from Microsoft Teams
description: You must have the following access to perform the steps in this article:
---

# Create *Adobe Workfront* tasks from Microsoft Teams

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Work, Plan</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>[Insert any access level configurations needed] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: Edit access to Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: Edit access to Documents
      </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[Insert any access level configurations needed] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: Edit access to Documents
     </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed and specify the object] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: View access or higher on Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: View access or higher on Documents
      </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[Insert permissions needed and specify the object] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: View access or higher on Documents
     </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

You can create personal tasks in *Adobe Workfront* from Microsoft Teams if the following conditions are met:

* A team owner has installed and configured *Workfront* for Microsoft Teams for your team.
* You are logged into *Workfront* from Microsoft Teams.

>[!NOTE]
>
>Microsoft Teams no longer supports Internet Explorer. To use the *Adobe Workfront* for Microsoft Teams integration, you must use a web browser other than Internet Explorer.

For information about installing *Workfront* for Microsoft Teams and logging in to *Workfront* from Microsoft Teams, see [Install Adobe Workfront for Microsoft Teams](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Create personal tasks from Microsoft Teams

<ol> 
 <li value="1"> <p>Log in to <em>Workfront</em> from Microsoft Teams.<br></p> <p>For information about logging in to <em>Workfront</em>, see <a href="../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md" class="MCXref xref">Install Adobe Workfront for Microsoft Teams</a>.</p> </li> 
 <li value="2">To open a <span class="bold">New task</span> card: 
  <ul>
   <li>If you are in the <em>Workfront</em> bot chat channel, type <span class="bold">New task </span>in the conversation field to create a new task.&nbsp;</li>
   <li>If you are in a chat channel other than the <em>Workfront</em> bot chat channel: 
    <ol>
     <li value="1">Start typing <span class="bold">@workfront </span>in the conversation field, then select the <em>Workfront</em> bot channel you want.</li>
     <li value="2"><p>Continue typing&nbsp;<span class="bold">New task </span>in the conversation field to create a new task.</p><p>The New task card displays in the <em>Workfront</em> bot channel.</p><p><img src="assets/ms-teams-new-task-card-350x181.png" alt="ms_teams_new_task_card.png" style="width: 350;height: 181;"></p></li>
    </ol></li>
  </ul></li> 
 <li value="3"> In the <em>Workfront</em> bot channel, specify the following information on the New task card: 
  <ul>
   <li>Task name in the <span class="bold">Write the task's title</span> field.</li>
   <li>Task description in the <span class="bold">Write the tasks's description</span> field.</li>
   <li>The take the task must be completed by, in the <span class="bold">Due Date</span> field.</li>
  </ul></li> 
 <li value="4"> <p> Click <span class="bold">Save.</span>&nbsp;<br></p> <p>The new personal task is created in <em>Workfront</em>. A Reference Number is assigned to it and visible on the new task card.<br></p> <p>For information about reference numbers, see the <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects" class="MCXref xref">Reference Numbers of objects</a> section in the <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a> article.</p> </li> 
 <li value="5">(Optional) Click <span class="bold">Edit</span> to edit the task information further.</li> 
 <li value="6">(Optional) Click <span class="bold">View in <em>Workfront</em></span> to open the task in a new tab in <em>Workfront</em> and edit the task further, move it to a project, or assign it to someone else.&nbsp;</li> 
</ol>

