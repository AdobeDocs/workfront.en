---
filename: copy-issues
product-area: projects
navigation-topic: manage-issues
title: Copy issues
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Copy issues

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

You can copy an issue or a request and save them on the same or another project. You can also copy an issue from a task to another project.

You can copy issues from the following objects:

* From a project to the same project (duplicate it on the same project)
* From a task to the same task (duplicate if on the same task)
* From a project to another project
* From a task to a project

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
   <td> <p><em>Request</em> or higher</p> <p><em>Review</em> or higher license to copy an issue in the Issues <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
     </MadCap:conditionalText>of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying&nbsp;the issue to with the ability to&nbsp;Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Considerations for issues associated with documents or request queues

Consider the following when copying issues that contain documents or are associated with a request queue:

* `When an issue is associated with a request queue:` When you copy&nbsp;an issue to another object&nbsp;and the issue&nbsp;is associated with a request queue, the copied issue is no longer associated with the original queue&nbsp;the first issue originated from.
* `When a document is attached to the issue:`&nbsp;When you copy&nbsp;an issue to another object&nbsp;and the issue has a document attached to it, the document and its versions also move to the new&nbsp;issue. Any *proofs* or approvals associated with the document do&nbsp;not move.

* `When an issue is linked to a document or a folder:`&nbsp;When you copy an issue which has documents or folders linked to a third party service like Google Drive, the&nbsp;links to the documents transfer to the copied issue.&nbsp;

## Copy issues in a list

You can copy one or multiple issues from a list of issues or from an issue report.

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">
<p>Copying issues differs depending on what environment you use. </p>
<ul>
<li> <p><a href="#copy2" class="MCXref xref">Copy issues in a list in the Production&nbsp;environment</a> </p> </li>
<li> <p><a href="#copy3" class="MCXref xref">Copy issues in a list in the Preview environment</a> </p> </li>
</ul>
<h3><a name="Copy2"></a>Copy issues in a list in the Production&nbsp;environment</h3>
</div>
-->

Copying issues differs depending on what environment you use.

* [Copy issues in a list in the Production environment](#copy2) 
* [Copy issues in a list in the Preview environment](#copy3)

### Copy issues in a list in the Production&nbsp;environment

<ol> 
 <li value="1"> <p>Go to a project whose issues you want to copy. </p> <p>Or </p> <p>Go to an issue report.</p> </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">If you selected to go to a project, click the <span class="bold">Issues</span> section, then select the issue or issues you want to copy. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">If you selected to go to a project, click the <span class="bold">Issues</span> section, then select the issue or issues you want to copy. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-issues-icon-highlighted-on-project-350x216.png" style="width: 350;height: 216;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-issues-icon-highlighted-on-project-350x216.png" style="width: 350;height: 216;"> </p> </li> 
 <li value="3">Click the <span class="bold">More</span>&nbsp;drop-down menu <draft-comment>
   <img src="assets/more-icon.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  </draft-comment><img src="assets/more-icon.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> at the top of the issue list, then click <span class="bold">Copy</span> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    <span class="bold"><span class="preview">to</span></span>
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <span class="bold"><span class="preview">to</span></span>
  </MadCap:conditionalText>. <draft-comment>
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><img src="assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png" style="width: 350;height: 119;"></p>
  </draft-comment><p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><img src="assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png" style="width: 350;height: 119;"></p><p>The <span class="bold">Copy Issue</span> or <span class="bold">Copy Issues</span> box displays. </p></li> 
 <li value="4"> <p>Specify&nbsp;the name of the project where you want to copy&nbsp;the issues in the <span class="bold">Select Destination Project</span> section. </p> <note type="tip">
   Only 50 projects display in the list.
  </note> <p> <draft-comment>
    <img src="assets/qs-copy-issues-ui-350x215.png" style="width: 350;height: 215;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/qs-copy-issues-ui-350x215.png" style="width: 350;height: 215;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="5"> <p>Continue copying the issue as described in the section <a href="#copy5" class="MCXref xref">Copy a single issue</a> in this article, starting with Step 3. </p> </li> 
</ol>

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">
<h3><a name="Copy3"></a>Copy issues in a list in the Preview environment</h3>
<ol>
<li value="1"> <p>Go to the project that contains the issue or issues that you want to copy.</p> <p>Or</p> <p>Go to an issue report. </p> </li>
<li value="2"> <p>If you selected to go to a project, click <span class="bold">Issues</span> in the left panel. </p> </li>
<li value="3"> <p>Select the issue or issues that you want to copy and click the <span class="bold">More menu <img src="assets/qs-more-menu.png"></span> at the top of the issue list, then click <span class="bold">Copy to</span>. </p> <p> <img src="assets/copy-issue-in-list-nwe-350x169.png" style="width: 350;height: 169;"> </p> </li>
<li value="4"> <p>Continue with copying the issue, as described in the section <a href="#copy6" class="MCXref xref">Copy a single issue in the Preview environment</a> starting with Step 4.</p> </li>
</ol>
</div>
-->

### Copy issues in a list in the Preview environment

<ol> 
 <li value="1"> <p>Go to the project that contains the issue or issues that you want to copy.</p> <p>Or</p> <p>Go to an issue report. </p> </li> 
 <li value="2"> <p>If you selected to go to a project, click <span class="bold">Issues</span> in the left panel. </p> </li> 
 <li value="3"> <p>Select the issue or issues that you want to copy and click the <span class="bold">More menu <img src="assets/qs-more-menu.png"></span> at the top of the issue list, then click <span class="bold">Copy to</span>. </p> <p> <img src="assets/copy-issue-in-list-nwe-350x169.png" style="width: 350;height: 169;"> </p> </li> 
 <li value="4"> <p>Continue with copying the issue, as described in the section <a href="#copy6" class="MCXref xref">Copy a single issue in the Preview environment</a> starting with Step 4.</p> </li> 
</ol>

## Copy a single issue

You can copy one issue when viewing it.

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">
<p>Copying issues differs depending on what environment you use. </p>
<ul>
<li> <p><a href="#copy4" class="MCXref xref">Copy a single issue in the Production&nbsp;environment</a> </p> </li>
<li> <p><a href="#copy6" class="MCXref xref">Copy a single issue in the Preview environment</a> </p> </li>
</ul>
<h3><a name="Copy4"></a>Copy a single issue in the Production&nbsp;environment</h3>
</div>
-->

Copying issues differs depending on what environment you use.

* [Copy a single issue in the Production environment](#copy4) 
* [Copy a single issue in the Preview environment](#copy6)

### Copy a single issue in the Production&nbsp;environment

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Go to an issue that you want to copy, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png">to the right of the issue name, then <span class="bold">Copy</span> <span class="preview">to</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Go to an issue that you want to copy, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png">to the right of the issue name, then <span class="bold">Copy</span> <span class="preview">to</span>.</p> <draft-comment>
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-copy-at-issue-level-highlighted-350x580.png" style="width: 350;height: 580;"> </p>
  </draft-comment><p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-copy-at-issue-level-highlighted-350x580.png" style="width: 350;height: 580;"> </p> <p>The <span class="bold">Copy Issue</span> box displays. </p> </li> 
 <li value="2"> <p>Specify&nbsp;the name of the project where you want to copy&nbsp;the issues in the <span class="bold">Select Destination Project</span> section. The name of the current project displays by default. </p> </li> 
 <li value="3">Click <span class="bold">Next Step</span>.</li> 
 <li value="4">(Optional) Select&nbsp;any of the options below to remove&nbsp;the items&nbsp;from&nbsp;the new issue.<br><note type="note">
    This impacts&nbsp;only the copied issues not the original issues.
  </note><br>
  <ul>
   <li><span class="bold">Clear Progress</span></li>
   <li><span class="bold">Clear Documents</span>:&nbsp;<span style="line-height: 1.5;">Removes everything in the documents tab, including document versions, linked documents, and folders.</span><br>By default, document <em>proofs</em> and approvals cannot be copied to another issue.</li>
   <li><span class="bold">Clear Assignments</span></li>
   <li><span class="bold">Clear Updates</span>: This is checked by default.&nbsp;</li>
   <li><span class="bold">Clear Permissions</span></li>
   <li><span class="bold">Clear Custom Data</span>:&nbsp;This will remove the information from the custom form on the issue, as well as the information on the custom forms&nbsp;associated&nbsp;with Documents attached to the issue, if those are also copied with the issue. The custom forms will remain attached to the issues&nbsp;and documents, but the information on the forms will not carry over to the new issue.&nbsp;</li>
  </ul></li> 
 <li value="5">(Optional)&nbsp;Click <span class="bold">Go back a step</span> to go back to the previous screen in the Copy&nbsp;Issue box. </li> 
 <li value="6"> <p>Click <span class="bold">Finish&nbsp;and Copy</span>&nbsp;<span class="bold">Issue</span>. </p> <p>Or</p> <p>Click<span class="bold"> Finish and&nbsp;Copy Issues</span> when you copy multiple issues in a list. </p> <p>The copied issue is added to the specified project.&nbsp;</p> </li> 
</ol>

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">
<h3><a name="Copy6"></a>Copy a single issue in the Preview environment</h3>
<ol>
<li value="1"> <p>Go to an issue that you want to copy, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png">to the right of the issue name, then <span class="bold">Copy</span><span class="preview">to</span>.</p> <p> <img src="assets/nwe-copy-at-issue-level-highlighted-350x580.png" style="width: 350;height: 580;"> </p> <p>The <span class="bold">Copy Issue</span> box displays. </p> <p> <img src="assets/copy-issue-box-nwe-350x285.png" style="width: 350;height: 285;"> </p> </li>
<li value="2"> <p> In the <span class="bold">Select Destination Project</span> section, specify&nbsp;the name of the project where you want to copy&nbsp;the issues. The name of the current project displays by default. </p> <note type="tip">
Only 100 projects display in the list.
</note> </li>
<li value="3"> <p>(Conditional) Click&nbsp;<span class="bold">request access</span> if you do not have access to copy issues to the project. </p> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue to copy the issue on the selected destination project without requesting access if you have access to add issues to one of the tasks on the destination project. </p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue to copy the issue on the selected destination project without requesting access if you have access to add issues to one of the tasks on the destination project. </p> </li>
<li value="4"> <p>(Optional) In the <span class="bold">Options</span> section, deselect any of the items listed in the table below to remove&nbsp;them&nbsp;from&nbsp;the new issue. All options are selected by default. </p> <note type="note">
This impacts&nbsp;only the copied issues not the original issues.
</note>
<table cellspacing="0">
<col>
<col>
<tbody>
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
<td><span style="line-height: 1.5;">Removes everything in the documents tab, including document versions, linked documents, and folders.</span> <br>By default, document <em>proofs</em> and approvals cannot be copied to another issue.</td>
</tr>
<tr>
<td role="rowheader">Permissions</td>
<td>Removes the entities that the issue is shared with. </td>
</tr>
<tr>
<td role="rowheader">Updates</td>
<td>Removes comments from the Updates section of the issue.</td>
</tr>
<tr>
<td role="rowheader">Custom Data</td>
<td>Removes the information from the custom form on the issue, as well as the information on the custom forms&nbsp;associated&nbsp;with Documents attached to the issue, if those are also copied with the issue. The custom forms will remain attached to the issues&nbsp;and documents, but the information on the forms will not carry over to the new issue.&nbsp;</td>
</tr>
</tbody>
</table> <p> <br> </p> </li>
<li value="5"> <p>(Optional) In the <span class="bold">Select Task</span> section, select the task where you want to move the issue. </p> </li>
<li value="6"> <p>Click <span class="bold">Copy issue</span> or <span class="bold">Copy issues</span> if you selected multiple issues in a list.</p> <p>The copied issues are added to the specified project.</p> </li>
</ol>
</div>
-->

### Copy a single issue in the Preview environment

<ol> 
 <li value="1"> <p>Go to an issue that you want to copy, then click the <span class="bold">More</span> menu <img src="assets/more-icon.png">to the right of the issue name, then <span class="bold">Copy</span><span class="preview">to</span>.</p> <p> <img src="assets/nwe-copy-at-issue-level-highlighted-350x580.png" style="width: 350;height: 580;"> </p> <p>The <span class="bold">Copy Issue</span> box displays. </p> <p> <img src="assets/copy-issue-box-nwe-350x285.png" style="width: 350;height: 285;"> </p> </li> 
 <li value="2"> <p> In the <span class="bold">Select Destination Project</span> section, specify&nbsp;the name of the project where you want to copy&nbsp;the issues. The name of the current project displays by default. </p> <note type="tip">
   Only 100 projects display in the list.
  </note> </li> 
 <li value="3"> <p>(Conditional) Click&nbsp;<span class="bold">request access</span> if you do not have access to copy issues to the project. </p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue to copy the issue on the selected destination project without requesting access if you have access to add issues to one of the tasks on the destination project. </p> </li> 
 <li value="4"> <p>(Optional) In the <span class="bold">Options</span> section, deselect any of the items listed in the table below to remove&nbsp;them&nbsp;from&nbsp;the new issue. All options are selected by default. </p> <note type="note">
   This impacts&nbsp;only the copied issues not the original issues.
  </note> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
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
     <td><span style="line-height: 1.5;">Removes everything in the documents tab, including document versions, linked documents, and folders.</span> <br>By default, document <em>proofs</em> and approvals cannot be copied to another issue.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Permissions</td> 
     <td>Removes the entities that the issue is shared with. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Updates</td> 
     <td>Removes comments from the Updates section of the issue.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Custom Data</td> 
     <td>Removes the information from the custom form on the issue, as well as the information on the custom forms&nbsp;associated&nbsp;with Documents attached to the issue, if those are also copied with the issue. The custom forms will remain attached to the issues&nbsp;and documents, but the information on the forms will not carry over to the new issue.&nbsp;</td> 
    </tr> 
   </tbody> 
  </table> <p> <br> </p> </li> 
 <li value="5"> <p>(Optional) In the <span class="bold">Select Task</span> section, select the task where you want to move the issue. </p> </li> 
 <li value="6"> <p>Click <span class="bold">Copy issue</span> or <span class="bold">Copy issues</span> if you selected multiple issues in a list.</p> <p>The copied issues are added to the specified project.</p> </li> 
</ol>

&nbsp;
