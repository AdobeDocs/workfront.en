---
filename: copy-issues
product-area: projects
navigation-topic: manage-issues
title: Copy issues
description: You can copy an issue or a request and save them on the same or another project. You can also copy an issue from a task to another project.
---

# Copy issues

You can copy an issue or a request and save them on the same or another project. You can also copy an issue from a task to another project.

You can copy issues from the following objects:

* From a project to the same project (duplicate it on the same project)
* From a task to the same task (duplicate if on the same task)
* From a project to another project
* From a task to a project

>[!TIP]
>
>"Issues" and "requests" are used interchangeably in Workfront. You can record issues on both projects and tasks to indicate unforeseen work that needs to be addressed. You can also submit requests which are recorded as issues on a project designated as a Request Queue.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to copy an issue in the Issues tab of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying&nbsp;the issue to with the ability to&nbsp;Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for issues associated with documents or request queues

Consider the following when copying issues that contain documents or are associated with a request queue:

* **When an issue is associated with a request queue:** When you copy&nbsp;an issue to another object&nbsp;and the issue&nbsp;is associated with a request queue, the copied issue is no longer associated with the original queue&nbsp;the first issue originated from.
* **When a document is attached to the issue:**&nbsp;When you copy&nbsp;an issue to another object&nbsp;and the issue has a document attached to it, the document and its versions also move to the new&nbsp;issue. Any proofs or approvals associated with the document do&nbsp;not move.
* **When an issue is linked to a document or a folder:**&nbsp;When you copy an issue which has documents or folders linked to a third party service like Google Drive, the&nbsp;links to the documents transfer to the copied issue.&nbsp;

## Copy issues in a list

You can copy one or multiple issues from a list of issues or from an issue report.

1. Go to a project whose issues you want to copy.

   Or

   Go to an issue report.

1. Issues
1. 
1. Click the **More**&nbsp;drop-down menu at the top of the issue list, then click **Copy** **to**.

   The **Copy Issue** or **Copy Issues** box displays. 

1. Specify&nbsp;the name of the project where you want to copy&nbsp;the issues in the **Select Destination Project** section.

   >[!TIP]
   >
   >Only 50 projects display in the list.

1. Continue copying the issue as described in the section [Copy a single issue](#copy5) in this article, starting with Step 3.

## Copy a single issue

You can copy one issue when viewing it.

1. Go to an issue that you want to copy, then click **Issue Actions** in the upper-right corner of the page, then click **Copy**.  The **Copy Issue** box displays. 

1. Specify&nbsp;the name of the project where you want to copy&nbsp;the issues in the **Select Destination Project** section. The name of the current project displays by default. 
1. Click **Next Step**.
1. (Optional) Select&nbsp;any of the options below to remove&nbsp;the items&nbsp;from&nbsp;the new issue.

   >[!NOTE]
   >
   >This impacts&nbsp;only the copied issues not the original issues.

   * **Clear Progress**
   * **Clear Documents**:  ```Removes everything in the documents tab, including document versions, linked documents, and folders.```  
     By default, document proofs and approvals cannot be copied to another issue.
   
   * **Clear Assignments**
   * **Clear Updates**: This is checked by default.&nbsp;
   * **Clear Permissions**
   * **Clear Custom Data**:&nbsp;This will remove the information from the custom form on the issue, as well as the information on the custom forms&nbsp;associated&nbsp;with Documents attached to the issue, if those are also copied with the issue. The custom forms will remain attached to the issues&nbsp;and documents, but the information on the forms will not carry over to the new issue.&nbsp;

1. (Optional)&nbsp;Click **Go back a step** to go back to the previous screen in the Copy&nbsp;Issue box. 
1. Click **Finish and Copy**&nbsp;**Issue**.

   Or

   Click**Finish and Copy Issues** when you copy multiple issues in a list.

   The copied issue is added to the specified project.&nbsp;

&nbsp;
