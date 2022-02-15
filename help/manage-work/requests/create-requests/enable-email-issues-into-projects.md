---
filename: enable-email-issues-into-projects
product-area: requests
navigation-topic: create-requests
---



# Enable users to email an issue into a Request Queue project {#enable-users-to-email-an-issue-into-a-request-queue-project}

You can configure a project to allow users to add issues to the project via email. You can allow for issues to be emailed into a project only if the project is designated as a Request Queue. For more information about creating a Request Queue project, see [Create a Request Queue](create-request-queue.md).


## Access requirements  {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Edit access to Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

The following prerequisites are required to configure a project to allow users to add issues to the project via email.


These conditions must be met, before enabling this feature:



*  Users who are emailing issues to this account must be active users with a license for *`Workfront`*.  

*  External Users cannot email issues to a request queue because they do not have access to create issues.
*  Users who are emailing issues to this account must have Add Issue permissions on the project. 
*  The emails coming from the email address associated with an active *`Workfront`* user are the only emails allowed to send issues to the project. 
*  The project is set up as a Request Queue. 
*  The email account associated with the project is not linked to a *`Workfront`* user account. 




## Configure the project in *`Workfront`* {#configure-the-project-in-workfront}

Keep the following in mind when enabling email queue settings:



*  Workfront allows one unique email per request queue across all clusters. If you choose to disable your request queue, you'll retain the email address you created as long as it is still in the Intake Email Address box. If you choose to discontinue use of the intake email, you must delete it from the Intake Email Field so it can be available for future use.





1. Go to the project that you want to enable to receive issues via email.
1.  Click `Queue Details` in the left panel. You might need to click `Show More` first.
1. In the `Queue Type` area, select `Publish as Help Request Queue`.

1. Scroll down to the `Email Queue Settings` area, then select `Enable Request intake via email`.

1.  Enter the beginning of the email address in the `Intake Email Address` box. You must create a unique email address. We recommend using your company name as part of your intake email address.

   ` `**Warning: **`` 
    
    
    * This email address cannot be recovered from the recycle bin if the project containing the request queue is deleted.
    * Because this email address must be unique, it may not be available in the future if deleted.
    * Emails forwarded to this email address are not added as issues to the project in  *`Workfront`*. Only emails created from this email address are added as issues.
    
    

1. (Optional) Select the `Forward all issues that fail to submit via email`, then enter a forwarding email address in the box below. This email address receives information about emails that failed to submit to the project.
1.  Click `Save`. Now, when users with an active *`Workfront`* account send an email to this email address, an issue is created in the *`Workfront`* project.


   >[!NOTE]
   >
   >Users must have access to create issues in the project in order to submit via email. You can grant this access in the Sharing dialog box under Advanced Settings.  
  
   >External Users cannot email issues to a request queue because they do not have access to create issues.







## Receive the issue in *`Workfront`* {#receive-the-issue-in-workfront}

When a *`Workfront`* user sends an email to *`Workfront`*, the following things happen:



* The Subject line of the email becomes the Issue Name.
* The body of the email becomes the Description of the Issue.
* If there are any documents attached to the email, those documents are attached to the issue in *`Workfront`*.
* The user who is sending the email becomes the Primary Contact of the new issue in *`Workfront`*.
* The body text of the email cannot exceed 4,000 characters.
* Email attachments cannot exceed 7 MB total.


