---
filename: access-workfront-from-ms-teams
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Access Adobe Workfront from Microsoft Teams
description: You can access Adobe Workfront from Microsoft Teams and perform several actions in Workfront by typing commands in either the Workfront bot channel or any other team channel.
---

# Access *Adobe Workfront* from Microsoft Teams

You can access *Adobe Workfront* from Microsoft Teams and perform several actions in *Workfront* by typing commands in either the *Workfront* bot channel or any other team channel.

You can do the following in *Workfront* from Microsoft Teams:

* Search for projects, tasks, or issues
* Create personal tasks
* `<font size="2">Respond to notifications</font>` 
* `<font size="2">Manage document approvals</font>`

The commands you use from Microsoft teams to perform these actions are different depending on which channel you want to access *Workfront* from.

>[!NOTE]
>
>Microsoft Teams no longer supports Internet Explorer. To use the *Adobe Workfront* for Microsoft Teams integration, you must use a web browser other than Internet Explorer.

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

## Access *Workfront* from the *Workfront* bot chat channel

<ol> 
 <li value="1">Open the <span class="bold"><em>Workfront</em> </span>bot chat channel.</li> 
 <li value="2"> <p>Click the <span class="bold"><em>Workfront</em></span> icon underneath the text field to display the search box.</p> <p> <img src="assets/teams-search-box-in-the-bot-channel-350x456.png" alt="teams_search_box_in_the_bot_channel.PNG" style="width: 350;height: 456;"> <br> </p> </li> 
 <li value="3"> <p> Start typing the name of a project, task, or issue.</p> <p>For information about searching for items, see the section <a href="../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md" class="MCXref xref">Search for and share Adobe Workfront items in Microsoft Teams</a> in the article <a href="../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md" class="MCXref xref">Search for and share Adobe Workfront items in Microsoft Teams</a>.</p> </li> 
 <li value="4"> <p>Click the <span class="bold">Type your questions here</span> field.</p> <p> <img src="assets/ms-teams-type-your-questions-here-and-what-can-i-do-fields-350x71.png" alt="ms_teams_type_your_questions_here_and_what_can_I_do_fields.png" style="width: 350;height: 71;"> <br> </p> </li> 
 <li value="5"> Do one of the following: <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
    Check steps 4 and 5, make sure my re-write works
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   Check steps 4 and 5, make sure my re-write works
  </MadCap:conditionalText>
  <ul>
   <li>Click <span class="bold">What can I do?</span>, then <span class="bold">Log in</span> or <span class="bold">Lot out</span> of <em>Workfront</em>, create a <span class="bold">New task</span> (personal task) in <em>Workfront</em>, or get <span class="bold">Help</span> by listing available commands.</li>
   <li><p>Access <em>Workfront</em> directly by typing a command in the <span class="bold">Type your questions here</span> field.</p><p>Commands are not case sensitive.</p><p> The <em>Workfront</em> bot responds with your request in the <em>Workfront</em> bot chat channel.</p></li>
  </ul></li> 
</ol>

## Access *Workfront* from a team channel

<ol> 
 <li value="1"> <p>Open a team channel and type <i style="font-weight: bold; font-style: normal;">@Workfront</i><em>, </em>then select <span class="bold">Workfront.</span></p> <p><span class="bold"><img src="assets/teams-workfront-channel-highlighted-in-message-350x160.png" alt="teams_workfront_channel_highlighted_in_message.png" style="width: 350;height: 160;"><br></span> </p> </li> 
 <li value="2"> <p> Click <span class="bold">Search</span> to search for a project, task, or issue.</p> <p>For information about searching for items, see the <a href="../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md" class="MCXref xref">Search for and share Adobe Workfront items in Microsoft Teams</a> section in the <a href="../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md" class="MCXref xref">Search for and share Adobe Workfront items in Microsoft Teams</a> article.</p> </li> 
 <li value="3">Type any of the following commands to perform these actions in <em>Workfront</em>. <br>Commands are not case sensitive:
  <ul>
   <li><span class="bold">Log in</span> to log in to <em>Workfront</em></li>
   <li><span class="bold">Log out</span> to log out of <em>Workfront</em></li>
   <li><p><span class="bold">New task</span> to create a new personal task</p><p>For information about creating new tasks from Microsoft Teams, see <a href="../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/create-workfront-tasks-from-ms-teams.md" class="MCXref xref">Create Adobe Workfront tasks from Microsoft Teams</a>.</p></li>
   <li><p><span class="bold">Help</span> to view a list of all available commands.</p><p>The <em>Workfront</em> bot responds with your request in the <em>Workfront</em> bot chat channel.</p></li>
  </ul></li> 
 <li value="4">Go to the <em>Workfront</em> bot chat channel to access <em>Workfront</em> and complete your request.</li> 
</ol>

