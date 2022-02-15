---
filename: request-document-approvals
product-area: documents
navigation-topic: approvals
---



# Request document approvals {#request-document-approvals}

You can request approval from managers or other users for a document in *`Adobe Workfront`*. You can also request document approvals from people without *`Workfront`* accounts if your *`Workfront administrator`* has enabled this capability, as described in [Configure system security preferences](configure-security-preferences.md).



## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View or higher access to Projects, Tasks, Issues, Templates, Portfolios, Programs, Reports, Dashboards, and Calendars, Documents</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View or higher access to the object associated with the request access or approval </p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Request a document approval {#request-a-document-approval}




1. In a document list that contains the document , click on the document .
1. Scroll down to the `Approvals` section in the Summary, and begin typing in the `Add Approver` text box. You can add Workfront users by name or external users by email.

1.  If your *`Adobe Workfront administrator`* has enabled the capability to collaborate with people who don't use *`Workfront`*, as described in [Configure system security preferences](configure-security-preferences.md), you can type their email addresses to include them.


   You cannot request approval from teams or groups.

1.  Repeat the previous step to add other approvers.




## Resubmit an approval on a new version {#resubmit-an-approval-on-a-new-version}

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show “changes” as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.



1. In a document list that contains the document , click on the document .
1.  Scroll down to the `Approvals` section in the Summary, click the `More`icon, then click `Resubmit`.


   ![](assets/nwe-resubmit-approval-350x149.png)







## Delete a document approval request {#delete-a-document-approval-request}




1. In a document list that contains the document , click on the document .
1.  `<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Scroll down to the <span class="bold">Approvals</span> section in the Summary, then click the <span class="bold">More</span> menu inline with the approver's name and select <span class="bold">Delete</span>.</p> </li>` The approval request is removed and the approver receives a notification that their approval is no longer needed. Their approval-related share access is also removed.





## Send a reminder to an approver {#send-a-reminder-to-an-approver}

You can send a message to remind document an approver that you're waiting for their feedback.



1. In a document list that contains the document , click on the document .
1.  Scroll down to the `Approvals` section in the Summary, then click the `More` menu inline with the approver's name and select `Remind`.


   The approver receives a notification informing them the approval is still pending. They may also receive an email reminder if they have that enabled.



