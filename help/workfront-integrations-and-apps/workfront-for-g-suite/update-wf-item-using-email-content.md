---
filename: update-wf-item-using-email-content
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
---



# Update a *`Adobe Workfront`* item from G&nbsp;Suite using email content {#update-a-adobe-workfront-item-from-g-suite-using-email-content}

You can update an existing project, task, or issue with information from a non- *`Adobe Workfront`* email.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Work, Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Before you can update a *`Workfront`* item using email content from G Suite, you must



* Install *`Workfront`* for G suite  
  For instructions, see [Install Adobe Workfront for G Suite](install-workfront-for-gsuite.md).





## Update a *`Workfront`* item using email content from G Suite {#update-a-workfront-item-using-email-content-from-g-suite}




1. If the *`Workfront for G Suite`* panel is not displayed, click the  *`Workfront`* icon ![](assets/wf-lion-icon.png) in the G Suite add-ons sidebar at the far-right of the page. 

1. With the email message open in G Suite, click `Post as a new update` in the G Suite panel.
1. Under `Type`, click the drop-down arrow, then click the type of object where you want to add the update.
1.  Click the `Search for` option, start typing the name of the object where you want to add the update, then select the item when it appears in the list below.


   ![](assets/click-search-for-task-issue.png)




   This option varies, depending on what you selected in step 3. It might be `Search for a project`, `Search for a task`, or `Search for an issue`. 


   >[!NOTE]
   >
   >When you are typing the name of a task, ad hoc personal tasks are excluded from the list of name that appears below.



1. Make any of these optional changes:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 180px;">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Update</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Edit any part of this text, which is taken from the email's subject line and body text.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Include email attachments</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>(Available only if the email contains at least one attachment.) Click this option to save attachments in the email to the Documents tab for the task or issue. </p><p>If you do not want to save an attachment, click the X to the right of its name. </p><p>If the email contains links to documents in Google Drive, the links are saved to the Overview tab of the task or issue you are creating. </p><p>Important: <span style="color: #ff1493;"><span style="color: #000000;">In order for this to work, your </span></span><span style="color: #000000;" class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span><span style="color: #ff1493;"><span style="color: #000000;"> must authorize Google Drive to work with <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></span></span></p><p>If you enable this option, it remains enabled for other emails you convert to tasks, issues, and updates.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Notify</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Click <span class="bold">Notify</span>, click the <span class="bold">Search for a user or team</span> option that appears, then start typing the name of the person or team and click it when it appears in the list below. Repeat this for each person and team you want to add, then click <span class="bold">Save</span>.</td>
  </tr>
 </tbody>
</table>

1.  Click `Update`.


   When you refresh your browser, a message with a link at the bottom of the *`Workfront for G Suite`* panel confirms that you have converted the email to an update:


   ![](assets/email-was-converted-as-update.png)




   You can click the link to go to the Updates tab in *`Workfront`* for the object you specified in step 4.


   You can repeat these steps to convert the same email to updates, task, and issues (see [Create a Adobe Workfront issue in G Suite using email content](create-wf-issue-in-g-suite-using-email-content.md)). When you refresh your browser or return to the email at another time, all links you have created for the email are listed at the bottom of the *`Workfront for G Suite`* panel.

1. (Optional) Continue to work with the update in the Workfront add-on panel by doing any of the following:
    
    
    * To add another update on the `Updates` tab, click `Start a new update` and type the information. 
    
    * To reply to an update on the `Updates` tab, click `Reply` and type your reply. 
    
    
      For both of the options above, you can click `Notify` to specify recipients for the reply as in step 5. When you are ready, click `Post` to add the update or reply. 
    
    * Click the `Details` tab to view the details for the new project, task, or issue.
    
    


