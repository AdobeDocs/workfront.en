---
filename: update-issue-status
product-area: projects
navigation-topic: update-work-in-a-project
title: Update issue status
description: You can update the status of an issue to inform others about where the issue is and how it is progressing.
---

# Update issue status

You can update the status of an issue to inform others about where the issue is and how it is progressing.

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
   <td> <p><em>Request</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Issue statuses

The following are the default statuses for issues in *Workfront*:

* New
* In Progress
* Awaiting Feedback
* On Hold
* Won't Resolve
* Reopened
* Closed
* Resolved

Your *Adobe Workfront administrator* can add custom statuses for issues for your organization. They can also make statuses available depending on the issue type.

For more information about custom statuses and issue types, see the following articles:

* [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) 
* [Create issues](../../../manage-work/issues/manage-issues/create-issues.md)

You can manually update issue statuses or you can let *Workfront* automatically update them when certain actions take place.

## Manually update issue status

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

<ol> 
 <li value="1">Go to an issue that you are assigned to for which you want to update the status.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Status</span> field in the issue header and select a new status. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Status</span> field in the issue header and select a new status. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-issue-status-expanded-in-header-350x370.png" style="width: 350;height: 370;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-issue-status-expanded-in-header-350x370.png" style="width: 350;height: 370;"> </p> </li> 
 <li value="3"> <p>(Optional) Do any of the following to provide additional information about the update, then click <span class="bold">Update</span> or, if the issue has a status that equates with Complete, click <span class="bold">Done:</span></p> 
  <ul> 
   <li> <p>To add a note about the update, go to the <span class="bold">Updates</span> <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section
     </MadCap:conditionalText> and click <span class="bold">Start a new update</span>, then type your note.</p> <p> <draft-comment>
      <img src="assets/nwe-issue-update-stream-message-box-350x125.png" style="width: 350;height: 125;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     </draft-comment><img src="assets/nwe-issue-update-stream-message-box-350x125.png" style="width: 350;height: 125;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
   <li>To notify certain users about the update, type their names in the <span class="bold">Notify</span> box that appears when you type a note about the update.</li> 
   <li>To update the condition of the issue, click <span class="bold">Condition</span>, then select the condition that best reflects the current condition of the issue. Select from the following options:
    <ul>
     <li>Going Smoothly</li>
     <li>Some Concerns</li>
     <li>Major Roadblocks</li>
    </ul></li> 
   <li>To update the Commit Date of the issue, expand the <span class="bold">Commit Date</span> drop-down calendar, and select a new date.</li> <draft-comment>
    <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>To provide a visual indication of issue completion, drag or double-click the bubble under <span class="bold">Percent Complete</span> in the header of the issue</p> <p>Or</p> <p>Click inside the bubble to enter a percentage. </p> <p> <img src="assets/drag-the-progress-bar-350x155.png" style="width: 350;height: 155;"> </p> </li>
   </draft-comment>
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>To provide a visual indication of issue completion, drag or double-click the bubble under <span class="bold">Percent Complete</span> in the header of the issue</p> <p>Or</p> <p>Click inside the bubble to enter a percentage. </p> <p> <img src="assets/drag-the-progress-bar-350x155.png" style="width: 350;height: 155;"> </p> </li> 
  </ul> </li> 
</ol>

## Automatically update issue status

*Workfront* automatically updates the existing status of an issue to a different status when the actions listed in the table below occur.

>[!NOTE]
>
>The statuses in the following table are default system statuses. Your *Workfront administrator* or a *group administrator* can rename the statuses in your instance of *Workfront*. For information about creating and managing statuses in *Workfront*, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Action</td> 
   <td>Original Status</td> 
   <td>New Status</td> 
  </tr> 
  <tr> 
   <td>Update the issue percent complete to 100%</td> 
   <td>New or In Progress</td> 
   <td>Closed</td> 
  </tr> 
  <tr> 
   <td>Update the issue percent complete from 100% to a lower number</td> 
   <td>Closed </td> 
   <td>In Progress</td> 
  </tr> 
  <tr> 
   <td>Update the status of a resolving object attached to the issue</td> 
   <td>Various statuses</td> 
   <td> <p>Various statuses</p> <p>For information about resolving objects and how they affect the status of issues, see the section "Synchronize the Status of the Resolvable Object with that of the Resolving Object" in the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td><span>Click the Start Issue button to accept working on an issue assigned to you</span> </td> 
    <td><span>New</span> </td> 
    <td> <p>Any status associated with the Start Issue button in your Home Team settings. </p> <p>For information about replacing the Work On It button with a Start Issue button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span><span>.</span> </p> <p>Tip: Clicking <draft-comment>
       <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">the Undo button</span>
      </draft-comment><span data-mc-conditions="QuicksilverOrClassic.Quicksilver">the Undo button</span> after clicking Start Issue reverts the status to New. </p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td><span>Click the Start Issue button to accept working on an issue assigned to you</span> </td> 
   <td><span>New</span> </td> 
   <td> <p>Any status associated with the Start Issue button in your Home Team settings. </p> <p>For information about replacing the Work On It button with a Start Issue button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span><span>.</span> </p> <p>Tip: Clicking <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">the Undo button</span> after clicking Start Issue reverts the status to New. </p> </td> 
  </tr> 
 </tbody> 
</table>

