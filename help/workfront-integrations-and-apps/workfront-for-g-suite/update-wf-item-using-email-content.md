---
filename: update-wf-item-using-email-content
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Update a Adobe Workfront item from G Suite using email content
description: You can update an existing project, task, or issue with information from a non-Adobe Workfront email.
---

# Update a Adobe Workfront item from G&nbsp;Suite using email content

You can update an existing project, task, or issue with information from a non-Adobe Workfront email.

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
   <td> <p>Work, Plan</p> </td> 
  </tr> <!--
   Access level configurations* [Insert any access level configurations needed] Example: Edit access to Documents Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see Create or modify custom access levels. You must be a Workfront administrator. For information on Workfront administrators, see Grant a user full administrative access. You must be a group administrator. For more information on group administrators, see Group administrators.
  --> <!--
   Object permissions [Insert permissions needed and specify the object] Example: View access or higher on Documents For information on requesting additional access, see Request access to objects in Adobe Workfront.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you can update a Workfront item using email content from G Suite, you must

* Install Workfront for G suite  
  For instructions, see [Install Adobe Workfront for G Suite](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Update a Workfront item using email content from G Suite

<ol> 
 <li value="1">If the Workfront for G Suite panel is not displayed, click the&nbsp;Workfront icon <img src="assets/wf-lion-icon.png"> in the G Suite add-ons sidebar at the far-right of the page. </li> 
 <li value="2">With the email message open in G Suite, click <span class="bold">Post as a new update</span> in the G Suite panel.</li> 
 <li value="3">Under <span class="bold">Type</span>, click the drop-down arrow, then click the type of object where you want to add the update.</li> 
 <li value="4"> <p>Click the <span class="bold">Search for</span> option, start typing the name of the object where you want to add the update, then select the item when it appears in the list below.</p> <p> <img src="assets/click-search-for-task-issue.png"> </p> <p>This option varies, depending on what you selected in step 3. It might be <span class="bold">Search for a project</span>, <span class="bold">Search for a task</span>, or <span class="bold">Search for an issue</span>. </p> <note type="Note">
   When you are typing the name of a task, ad hoc personal tasks are excluded from the list of name that appears below.
   <!--
    For information about ad hoc personal tasks, see Creating Ad Hoc Work Items in the new Workfront experience Creating Ad Hoc Work Items in the new Adobe Workfront experience .
   -->
  </note> </li> 
 <li value="5">Make any of these optional changes: 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Update</td> 
     <td>Edit any part of this text, which is taken from the email's subject line and body text.</td> 
    </tr> Include email attachments (Available only if the email contains at least one attachment.) Click this option to save attachments in the email to the Documents tab for the task or issue. If you do not want to save an attachment, click the X to the right of its name. If the email contains links to documents in Google Drive, the links are saved to the Overview tab of the task or issue you are creating. Important: In order for this to work, your Workfront administrator must authorize Google Drive to work with Workfront , as described in Configure document integrations. If you enable this option, it remains enabled for other emails you convert to tasks, issues, and updates. Notify Click Notify, click the Search for a user or team option that appears, then start typing the name of the person or team and click it when it appears in the list below. Repeat this for each person and team you want to add, then click Save. 
   </tbody> 
  </table></li> 
 <li value="6"> <p>Click <span class="bold">Update</span>.</p> <p>When you refresh your browser, a message with a link at the bottom of the Workfront for G Suite panel confirms that you have converted the email to an update:</p> <p> <img src="assets/email-was-converted-as-update.png"> </p> <p>You can click the link to go to the Updates tab in Workfront for the object you specified in step 4.</p> <p>You can repeat these steps to convert the same email to updates, task, and issues (see <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md" class="MCXref xref">Create a Adobe Workfront issue in G Suite using email content</a>). When you refresh your browser or return to the email at another time, all links you have created for the email are listed at the bottom of the Workfront for G Suite panel.</p> </li> 
 <li value="7">(Optional) Continue to work with the update in the Workfront add-on panel by doing any of the following: 
  <ul> 
   <li>To add another update on the <span class="bold">Updates</span> tab, click <span class="bold">Start a new update</span> and type the information. </li> 
   <li><p>To reply to an update on the <span class="bold">Updates</span> tab, click <span class="bold">Reply</span> and type your reply. </p><p>For both of the options above, you can click <span class="bold">Notify</span> to specify recipients for the reply as in step 5. When you are ready, click <span class="bold">Post</span> to add the update or reply. </p></li> 
   <li>Click the <span class="bold">Details</span> tab to view the details for the new project, task, or issue.</li> 
  </ul></li> 
</ol>

