---
filename: create-a-wf-request-from-an-outlook-email
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Create an Adobe Workfront request from an Outlook email
description: You can create a Adobe Workfront request from an email in Outlook.
---

# Create an `Adobe Workfront` request from an Outlook email

You can create a `Adobe Workfront` request from an email in Outlook.

When you create a `Workfront` request based on an email, the&nbsp;content of the email (including the subject and body) are included in the request by default.

>[!NOTE]
>
>You can not create a Workfront request from a shared Outlook mailbox.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p>Work, Plan</p> </td> 
  </tr> <!--
   Access level configurations* [Insert any access level configurations needed] Example: Edit access to Documents Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see Create or modify custom access levels. You must be a Workfront administrator. For information on Workfront administrators, see Grant a user full administrative access. You must be a group administrator. For more information on group administrators, see Group administrators.
  --> <!--
   Object permissions [Insert permissions needed and specify the object] Example: View access or higher on Documents For information on requesting additional access, see Request access to objects in Adobe Workfront.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

Your `Workfront administrator` must enable Outlook for Office with `Workfront` before you can use this integration.

## Create a request from an Outlook email

To create a `Workfront` Request from Outlook:

<ol> 
 <li value="1">Select the email that contains the information you want to include in&nbsp;a <span>Workfront</span> request.&nbsp;</li> 
 <li value="2">Click the&nbsp;<span class="bold"><span>Workfront</span></span>&nbsp;icon in the upper-right corner of the email message to display the <span>Workfront</span> add-in.<br>You might need to click the down-pointing arrow in the upper right of your email to access the <span>Workfront</span> icon.</li> 
 <li value="3"> <p>Click the <span class="bold">Menu</span> icon to display the list of available <span>Workfront</span> options.<br></p> <p> <img src="assets/o365-addin-menu2-icon.png" alt="o365_addin_menu2_icon.png"> <br> </p> </li> 
 <li value="4">Click <span class="bold">Submit Request</span>.</li> 
 <li value="5"> <p>In the <span class="bold">Select a Request Type</span> field, select the request queue where you want to submit the request.<br></p> <p> <img src="assets/o365-addin-submitrequest.png" alt="o365_addin_submitrequest.png"> </p> </li> 
 <li value="6">Specify the following information:<br>Depending on how the request queue was set up, available fields might vary. For a complete list and description of possible fields, see <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a> article.
  <ul>
   <li><span class="bold">Subject:</span> Specify a subject for the request. By default, the email subject is used.</li>
   <li><span class="bold">Description:</span> Specify a description for the request. By default, the email body is used.</li>
   <li><span class="bold">Documents:</span> Attach any documents that you want to include in the request. You can attach documents via drag and drop, or by clicking <span class="bold">Select File</span> and browsing to and selecting the document.<br>By default, any documents attached to the email are included in the request.</li>
  </ul></li> 
 <li value="7">Click <span class="bold">Submit Request</span>.<br>The Request is submitted to <span>Workfront</span>, in the specified request queue.&nbsp;</li> 
 <li value="8">(Optional) Navigate back to Outlook, and select the original email.<br>At the top of the <span>Workfront</span> add-in panel, notice the confirmation with a link that the email was added to <span>Workfront</span> as a request. The link includes the date on which it was converted.<br><img src="assets/outlook-submitted-as-a-request-350x130.png" alt="outlook_submitted_as_a_request.png" style="width: 350;height: 130;"></li> 
</ol>

