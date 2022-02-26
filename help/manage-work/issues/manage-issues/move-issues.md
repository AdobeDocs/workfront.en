---
filename: move-issues
product-area: projects
navigation-topic: manage-issues
title: Move issues
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Move issues

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

You can move issues between the following objects:

* From a project to another project
* From a task to another task in the same project or in another project
* From a task to the project or to another project
* From a project to a task in the same project or a task in another project

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
   <td> <p><em>Request</em> or higher</p> <p><em>Review</em> or higher license to move issues in the Issues <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
     </MadCap:conditionalText>of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are moving the issue with the ability to&nbsp;Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Considerations about moving issues

Consider the following when moving&nbsp;issues that contain documents or are associated with a request queue:

* `When an issue is associated with a requests queue:` When you move&nbsp;an issue to another object&nbsp;and the issue&nbsp;is associated with a request queue, the moved&nbsp;issue is no longer associated with the original queue&nbsp;the first issue originated from.
* `When a document is attached to the issue:`&nbsp;When you move&nbsp;an issue to another object&nbsp;and the issue has a document attached to it, the document, its versions and *proofs* also move to the new&nbsp;issue. Any approvals associated with the document do&nbsp;not move.

* `When an issue is linked to a document or a folder:`&nbsp;When you move&nbsp;an issue which has documents or folders linked to a a third party service like Google Drive, the&nbsp;links to the documents move with the issue.&nbsp;

##

## Move issues in a list

You can move one or multiple issues from a list of issues or from an issue report.

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">
<p>Moving issues differs depending on what environment you use. </p>
<ul>
<li> <p><a href="#copy2" class="MCXref xref">Move issues in a list in the Production&nbsp;environment</a> </p> </li>
<li> <p><a href="#copy3" class="MCXref xref">Move issues in a list in the Preview environment</a> </p> </li>
</ul>
<h3><a name="Copy2"></a>Move issues in a list in the Production&nbsp;environment</h3>
</div>
-->

Moving issues differs depending on what environment you use.

* [Move issues in a list in the Production environment](#copy2) 
* [Move issues in a list in the Preview environment](#copy3)

### Move issues in a list in the Production&nbsp;environment

<ol> 
 <li value="1"> <p>Go to a project whose issues you want to move. </p> <p>Or </p> <p>Go to an issue report.</p> </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">If you selected a project, click the <span class="bold">Issues</span> section, then select the issue or issues you want to move in the list of issues. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">If you selected a project, click the <span class="bold">Issues</span> section, then select the issue or issues you want to move in the list of issues. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-issues-icon-highlighted-on-project-350x216.png" style="width: 350;height: 216;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-issues-icon-highlighted-on-project-350x216.png" style="width: 350;height: 216;"> </p> </li> 
 <li value="3"> <p>Click the <span class="bold">More</span>&nbsp;drop-down menu <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     <draft-comment>
      <img src="assets/more-icon.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     </draft-comment>
     <img src="assets/more-icon.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    <img src="assets/more-icon.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </MadCap:conditionalText> at the top of the issue list, then click <span class="bold">Move</span> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     <span class="bold"><span class="preview">to</span></span>
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    <span class="bold"><span class="preview">to</span></span>
   </MadCap:conditionalText>. </p> <p> <draft-comment>
    <img src="assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png" style="width: 350;height: 119;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png" style="width: 350;height: 119;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="4">The <span class="bold">Move Issue</span> or <span class="bold">Move Issues</span> box displays. </li> 
 <li value="5"> <p>Specify&nbsp;the name of the project where you want to move the issues in the <span class="bold">Select Destination Project</span> section. </p> <note type="tip">
   Only 50 projects display in the list.
  </note> <p> <img src="assets/ci3-350x203.png" alt="" style="width: 350;height: 203;"> </p> </li> 
 <li value="6"> <p>Continue moving the issue as described in the section <a href="#copy5" class="MCXref xref">Move a single issue</a> in this article, starting with Step 3. </p> </li> 
</ol>

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">
<h3><a name="Copy3"></a>Move issues in a list in the Preview environment</h3>
<ol>
<li value="1"> <p>Go to the project that contains the issue or issues that you want to move.</p> <p>Or</p> <p>Go to an issue report. </p> </li>
<li value="2"> <p>If you selected to go to a project, click <span class="bold">Issues</span> in the left panel. </p> </li>
<li value="3"> <p>Select the issue or issues that you want to move and click the <span class="bold">More menu <img src="assets/qs-more-menu.png"></span> at the top of the issue list, then click <span class="bold">Move to</span>. </p> <p> <draft-comment>
<img src="assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png" style="width: 350;height: 119;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
</draft-comment><img src="assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png" style="width: 350;height: 119;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="4"> <p>Continue with moving the issue, as described in the section <a href="#copy6" class="MCXref xref">Move a single issue in the Preview environment</a> starting with Step 2.</p> </li>
</ol>
</div>
-->

### Move issues in a list in the Preview environment

<ol> 
 <li value="1"> <p>Go to the project that contains the issue or issues that you want to move.</p> <p>Or</p> <p>Go to an issue report. </p> </li> 
 <li value="2"> <p>If you selected to go to a project, click <span class="bold">Issues</span> in the left panel. </p> </li> 
 <li value="3"> <p>Select the issue or issues that you want to move and click the <span class="bold">More menu <img src="assets/qs-more-menu.png"></span> at the top of the issue list, then click <span class="bold">Move to</span>. </p> <p> <img src="assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png" style="width: 350;height: 119;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="4"> <p>Continue with moving the issue, as described in the section <a href="#copy6" class="MCXref xref">Move a single issue in the Preview environment</a> starting with Step 2.</p> </li> 
</ol>

## Move a single issue

You can move one issue when viewing it.

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">
<p>Moving issues differs depending on what environment you use. </p>
<ul>
<li> <p><a href="#copy4" class="MCXref xref">Move a single issue in the Production&nbsp;environment</a> </p> </li>
<li> <p><a href="#copy6" class="MCXref xref">Move a single issue in the Preview environment</a> </p> </li>
</ul>
<h3><a name="Copy4"></a>Move a single issue in the Production&nbsp;environment</h3>
</div>
-->

Moving issues differs depending on what environment you use.

* [Move a single issue in the Production environment](#copy4) 
* [Move a single issue in the Preview environment](#copy6)

### Move a single issue in the Production&nbsp;environment

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Go to an issue that you want to move, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png"> to the right of the issue name, then <span class="bold">Move</span> <span class="preview" style="font-weight: bold;">to</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Go to an issue that you want to move, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png"> to the right of the issue name, then <span class="bold">Move</span> <span class="preview" style="font-weight: bold;">to</span>.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-move-at-issue-level-highlighted-350x579.png" style="width: 350;height: 579;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-move-at-issue-level-highlighted-350x579.png" style="width: 350;height: 579;"> </p> <p>The <span class="bold">Move Issue</span> box displays. </p> </li> 
 <li value="2"> <p>Specify&nbsp;the name of the project where you want to move the issues in the <span class="bold">Select Destination Project</span> section. The name of the current project displays by default. </p> <note type="tip">
   Only 50 projects display in the list.
  </note> </li> 
 <li value="3"> <p>(Optional) Click <span class="bold">Next Step.</span></p> <p>Or</p> <p>Select <span class="bold">Task</span> to select a task to move the issue to.</p> <p> <img src="assets/move-issue-last-step-350x165.png" alt="move_issue_last_step.png" style="width: 350;height: 165;"> </p> </li> 
 <li value="4">(Optional)&nbsp;Click <span class="bold">Go back a Step</span> to go back to the previous screen in the Move Issue box. </li> 
 <li value="5"> <p>Click <span class="bold">Finish and Move Issue</span>.</p> <p>Or</p> <p>Click<span class="bold"> Finish and&nbsp;Move Issues</span> when you copy multiple issues in a list. </p> <p>The copied issue is added to the specified project.&nbsp;</p> </li> 
</ol>

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">
<h3><a name="Copy6"></a>Move a single issue in the Preview environment</h3>
<ol>
<li value="1"> <p>Go to an issue that you want to copy, click the <span class="bold">More</span> menu <img src="assets/more-icon.png">to the right of the issue name, then select <span class="bold">Move</span><span class="preview" style="font-weight: bold;"> to</span>.</p> <p> <img src="assets/nwe-move-at-issue-level-highlighted-350x579.png" style="width: 350;height: 579;"> </p> <p>The <span class="bold">Move Issue</span> box displays.</p> <p> <img src="assets/move-issue-box-nwe-350x281.png" style="width: 350;height: 281;"> </p> </li>
<li value="2"> <p> In the <span class="bold">Select Destination Project</span> section, specify&nbsp;the name of the project where you want to move the issues. The name of the current project displays by default. </p> <note type="tip">
Only 100 projects display in the list.
</note> </li>
<li value="3"> <p>(Conditional) Click&nbsp;<span class="bold">request access</span> if you do not have access to move issues to the project. </p> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue to move the issue on the selected destination project without requesting access if you have access to add issues to one of the tasks on the destination project. </p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue to move the issue on the selected destination project without requesting access if you have access to add issues to one of the tasks on the destination project. </p> </li>
<li value="4"> <p>(Optional) In the <span class="bold">Options</span> section, deselect any of the items listed in the table below to remove&nbsp;them&nbsp;from&nbsp;the moved issue. All options are selected by default. </p> <note type="important">
Deselecting items in the Options list results in loss of data. Information from the existing issue will be removed and cannot be recovered.
</note>
<table cellspacing="0">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Select all</td>
<td>Deselect this option to remove all information from the issue when moving it to its new location. </td>
</tr>
<tr>
<td role="rowheader">Assignments</td>
<td>Removes users, job roles, or teams that are assigned to the issue.</td>
</tr>
<tr>
<td role="rowheader">Progress</td>
<td>Removes the percent complete, if any, of the issue. </td>
</tr>
<tr>
<td role="rowheader">Documents</td>
<td> <p><span style="line-height: 1.5;">Removes everything in the documents tab, including document versions, linked documents, and folders.</span> <br> </p> </td>
</tr>
<tr>
<td role="rowheader">Permissions</td>
<td>Removes the entities that the issue is shared with. </td>
</tr>
<tr>
<td role="rowheader">Updates</td>
<td>Removes comments from the Updates section of the issue.</td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>(Optional) In the <span class="bold">Select Task</span> section, select the task where you want to move the issue. </p> </li>
<li value="6"> <p>Click <span class="bold">Move issue</span> or <span class="bold">Move issues</span>, if you selected multiple issues in a list. </p> <p>The moved issues are added to the specified project.&nbsp;</p> </li>
</ol>
</div>
-->

### Move a single issue in the Preview environment

<ol> 
 <li value="1"> <p>Go to an issue that you want to copy, click the <span class="bold">More</span> menu <img src="assets/more-icon.png">to the right of the issue name, then select <span class="bold">Move</span><span class="preview" style="font-weight: bold;"> to</span>.</p> <p> <img src="assets/nwe-move-at-issue-level-highlighted-350x579.png" style="width: 350;height: 579;"> </p> <p>The <span class="bold">Move Issue</span> box displays.</p> <p> <img src="assets/move-issue-box-nwe-350x281.png" style="width: 350;height: 281;"> </p> </li> 
 <li value="2"> <p> In the <span class="bold">Select Destination Project</span> section, specify&nbsp;the name of the project where you want to move the issues. The name of the current project displays by default. </p> <note type="tip">
   Only 100 projects display in the list.
  </note> </li> 
 <li value="3"> <p>(Conditional) Click&nbsp;<span class="bold">request access</span> if you do not have access to move issues to the project. </p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue to move the issue on the selected destination project without requesting access if you have access to add issues to one of the tasks on the destination project. </p> </li> 
 <li value="4"> <p>(Optional) In the <span class="bold">Options</span> section, deselect any of the items listed in the table below to remove&nbsp;them&nbsp;from&nbsp;the moved issue. All options are selected by default. </p> <note type="important">
   Deselecting items in the Options list results in loss of data. Information from the existing issue will be removed and cannot be recovered. 
  </note> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Select all</td> 
     <td>Deselect this option to remove all information from the issue when moving it to its new location. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Assignments</td> 
     <td>Removes users, job roles, or teams that are assigned to the issue.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Progress</td> 
     <td>Removes the percent complete, if any, of the issue. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Documents</td> 
     <td> <p><span style="line-height: 1.5;">Removes everything in the documents tab, including document versions, linked documents, and folders.</span> <br> </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Permissions</td> 
     <td>Removes the entities that the issue is shared with. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Updates</td> 
     <td>Removes comments from the Updates section of the issue.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>(Optional) In the <span class="bold">Select Task</span> section, select the task where you want to move the issue. </p> </li> 
 <li value="6"> <p>Click <span class="bold">Move issue</span> or <span class="bold">Move issues</span>, if you selected multiple issues in a list. </p> <p>The moved issues are added to the specified project.&nbsp;</p> </li> 
</ol>

