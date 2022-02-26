---
filename: delete-issues
product-area: projects
navigation-topic: manage-issues
title: Delete issues
description: You can delete issues or requests in Adobe Workfront if you have the correct access and permissions to do so.
---

# Delete issues

You can delete issues or requests in&nbsp;*Adobe Workfront* if you have the correct access and permissions to do so.

>[!TIP]
>
>"Issues" and "requests" are used interchangeably in *Workfront*. You can record issues on both projects and tasks to indicate unforeseen work that needs to be addressed. You can also submit requests which are recorded as issues on a project designated as a Request Queue.

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
   <td> <p><em>Request</em> or higher</p> <p><em>Review</em> or higher license to delete issues in the Issues <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
     </MadCap:conditionalText>of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>Contribute or higher permissions on the project or task</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Considerations for deleting issues

* Your *Workfront administrator* or a *group administrator* must enable deleting issues in a project that has a status of Complete in your Project Preferences area. For information about setting up project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).   

* If the issue has logged hours, the *Workfront administrator* or a *group administrator* must allow the deletion of these issues by configuring the Task & Issue Preferences in your *Workfront* instance. 

  <!--
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">This also applies when you try to delete projects that have issues with hours logged on them.</span>
  -->

  `This also applies when you try to delete projects that have issues with hours logged on them.`

  For more information about enabling the deletion of issues where hours are logged, see the "Deletion" section in [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## The impact of deleting issues

When you delete an issue, you impact other objects linked to the issue.

The following objects attached to an issue are also deleted when you delete an issue:

* Documents

  You cannot delete an issue that has a document which has been checked out attached to it. For more information about checking out documents, see [Check out documents](../../../documents/managing-documents/check-out-documents.md).

* Notes
* Approvals

Depending on how your *Workfront* or *group administrator* configures the Project, Task, or Issue Deletion Preferences in the `Timesheet & Hour Preferences` of your *Workfront* instance, hours logged for the issues are handled in one of the following ways when deleting an issue:

* Move to the project and will not be restored on the issue, if the issue is later restored.
* Be deleted and will be restored on the issue, if the issue is later restored.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">This also applies when you try to delete projects that have tasks with hours logged on them.</p>
  -->

  This also applies when you try to delete projects that have tasks with hours logged on them.

  For more information about configuring the deletion preferences for hours logged on issues, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* The users assigned to the issue or to the issue approval remain on the project team.  
  For more information about project teams, see [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Delete issues

* [Delete multiple issues in a project simultaneously](#delete-tasks-in-a-project-task-list) 
* [Delete a single issue](#delete-a-task)

### Delete multiple issues in a project simultaneously

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Go to the 
    <span class="bold">Main menu</span>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Go to the 
   <span class="bold">Main menu</span>. 
  </MadCap:conditionalText></li> 
 <li value="2"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Projects</span>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Projects</span>. 
  </MadCap:conditionalText> </li> 
 <li value="3">Click the project name that contains the issues you want to delete.</li> 
 <li value="4"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Issues</span> in the left panel.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Issues</span> in the left panel.
  </MadCap:conditionalText> </li> <draft-comment>
  <li value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Select an issue, then click the <span class="bold">Delete</span> icon <img src="assets/delete.png"> at the top of the list. </li>
 </draft-comment>
 <li value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Select an issue, then click the <span class="bold">Delete</span> icon <img src="assets/delete.png"> at the top of the list. </li> 
 <li value="6">If the deletion is allowed, click <span class="bold">Yes, Delete it</span>.<br>Your <em>Workfront administrator</em> might not allow the deletion of issues where hours are logged.<br>For more information about the access and permissions needed to delete an issue, see <a href="#access-and-permissions-needed" class="MCXref xref">Delete issues </a>.</li> 
</ol>

### Delete a single issue

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main</span> menu. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click the 
   <span class="bold">Main</span> menu. 
  </MadCap:conditionalText></li> 
 <li value="2"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Projects</span>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Projects</span>. 
  </MadCap:conditionalText> </li> 
 <li value="3">Click the project name that contains the issue you want to delete.</li> 
 <li value="4"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
     <span class="bold">Issues</span> icon. 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Issues</span> icon. 
   </MadCap:conditionalText></p> <p> <draft-comment>
    <img src="assets/qs-issues-icon-highlighted-on-project-350x278.png" style="width: 350;height: 278;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/qs-issues-icon-highlighted-on-project-350x278.png" style="width: 350;height: 278;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="5">Click the name of the issue you want to delete.</li> 
 <li value="6"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
     <span class="bold">More</span> menu.
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">More</span> menu.
   </MadCap:conditionalText> </p> <p> <draft-comment>
    <img src="assets/qs-issue-more-menu-highlighted-350x225.png" style="width: 350;height: 225;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/qs-issue-more-menu-highlighted-350x225.png" style="width: 350;height: 225;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="7"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Delete</span>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Delete</span>.
  </MadCap:conditionalText> </li> 
 <li value="8">If the deletion is allowed, click <span class="bold">Yes, Delete it</span>.<br>Your <em>Workfront administrator</em> might not allow the deletion of issues where hours are logged.<br>For more information about the access and permissions needed to delete an issue, see <a href="#access-and-permissions-needed" class="MCXref xref">Delete issues </a>.</li> 
</ol>

## Restore deleted issues

A *Workfront* or *group administrator* can restore issues within 30 days after they are deleted. For more information about restoring items in *Workfront*, see [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
