---
filename: update-linked-items-between-jira-wf
product-area: workfront-integrations
navigation-topic: workfront-for-jira
---



# Update linked items between Jira and *`Adobe Workfront`* {#update-linked-items-between-jira-and-adobe-workfront}

When you link Jira issues to *`Adobe Workfront`* tasks or issues, your users can update items in one application and the counterpart of that item also updates for the users working in the second application.&nbsp;


For more information about linking items between *`Workfront`* and Jira, see [Link items between Adobe Workfront and Jira](link-items-between-wf-jira.md).


As you are setting up *`Workfront`* for Jira, as a Jira system administrator, you can configure certain fields from one application to synchronize with fields from linked items in the other application.


For more information about synchronizing fields between linked Jira and *`Workfront`* items, see [Configure Adobe Workfront for Jira](configure-workfront-for-jira.md).


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Pro or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><a href="wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Plan</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Jira access</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in Jira and <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For information on <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Before you can link items between *`Workfront`* and Jira, you must



*  Install *`Workfront`* for Jira.


  For instructions on installing *`Workfront`* for Jira, see [Install Adobe Workfront for Jira](install-workfront-for-jira.md).

*  Configure *`Workfront`* for Jira.


  For instructions on configuring *`Workfront`* for Jira, see [Configure Adobe Workfront for Jira](configure-workfront-for-jira.md).

*  Link items between Workfront and Jira.


  For instructions, see [Link items between Adobe Workfront and Jira](link-items-between-wf-jira.md).





## Update linked items in *`Workfront`* {#update-linked-items-in-workfront}

If you work primarily in *`Workfront`*, you can update your work items in *`Workfront`* and their counterparts in Jira also update. This update happens through the integration of *`Workfront`* for Jira which does not require you to have a Jira license.&nbsp;


As long as your *`Workfront administrator`* has configured *`Workfront`* for Jira to synchronize the fields between linked items, certain fields that you update in *`Workfront`* also update for the linked Jira issue. For more information about updating items in *`Workfront`*, see [Edit issues](edit-issues.md) and [Edit tasks](edit-tasks.md).


The following list shows which *`Workfront`* fields synchronize with Jira fields on linked items:&nbsp;

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Updated <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> field&nbsp;</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"><span class="bold">Synchronized Jira field/ update</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue or Task name</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Issue name</p> <p>A comment about the Name change is added to the <span class="bold"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></span> tab of the Jira issue.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Issue or Task Description</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Issue Description</p> <p>A comment about the updated Description is added to the <span class="bold"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></span> tab of the Jira issue.<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p> Uploaded Documents</p> <p>Note: Documents which are linked to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> items from an external server are not transferred&nbsp;to Jira issues. Only documents uploaded directly to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> items are also updated to the linked Jira issues.&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Attachments</p> <p>A comment about the uploaded attachments is added to the <span class="bold"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></span> tab of the Jira issue.<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Planned Completion Date</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Due Date</p> <p>A comment about the Due Date having changed is added to the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> tab of the Jira issue.&nbsp;</p> <p>Note: You must enable <span class="bold">Due Date</span> for your Jira issues to be able to see this field updated in Jira.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Custom Forms and Custom Fields</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Display in the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> right panel of the Jira issue. <br>Only the Custom Fields that have an actual value display in the panel.<br><img src="assets/custom-form-in-workfront-side-panel-274x309.png" alt="custom_form_in_workfront_side_panel.png" style="width: 274;height: 309;"></p> <p>Note: Custom Form sections are displayed with the access level of the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Issue or Task Priority</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Displays in the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> right panel of the Jira issue. <br>It does not update the issue <span class="bold">Priority</span> field in Jira.&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Log time&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>A comment about the logged time is added in the <span class="bold"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></span> tab of the Jira issue. This includes the name of the user who logs the time, as well as the user for whom the time is logged, in case they are different. No time is logged in the <span class="bold">Work log</span> tab in Jira.<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Comments</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>The comment is added to the <span class="bold"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></span> tab of the Jira issue. It is not added to the <span class="bold">Comments</span> tab of the Jira issue</p> <p>Note: When you link two existing items manually, the comments that were added to the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> item before linking it to Jira do not synchronize to the Jira issue.&nbsp;</p> </td> 
  </tr> 
 </tbody> 
</table>



## Update linked items in Jira {#update-linked-items-in-jira}

If you work primarily in Jira, you can update your work items in Jira and their counterparts in *`Workfront`* also update. You do not have to have a *`Workfront`* license for the *`Workfront`* items linked to your Jira issues to receive the updates you are making in Jira.&nbsp;


On condition that your *`Workfront administrator`* has configured *`Workfront`* for Jira to synchronize the fields between linked items, certain fields which you update in Jira also update for the linked *`Workfront`* item.&nbsp;


The following list shows which Jira fields synchronize with *`Workfront`* fields on linked items:&nbsp;

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Updated Jira Field&nbsp;</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"><span class="bold">Synchronized <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Field/ Update</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue Status</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Issue or Task Status</p> <p>Issue status in Jira syncs with the following statuses, or statuses that equate with the following statuses, in Workfront:</p> 
    <ul> 
     <li> <p>New (NEW)</p> </li> 
     <li> <p>In Progress (INP)</p> </li> 
     <li> <p>Closed/Complete (CLS/CPL)</p> </li> 
    </ul> <p>Note: The Jira status syncs with the first Workfront status that equates with the appropriate status.</p> <p>For more information about statuses of items in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, see <a href="create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Issue Assignee</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Issue or Task Assignee</p> <p>Important: When you assign an item in Jira to a user who does not have a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account, the integration creates a new active user in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only when the <span class="bold">Automatically create a user in </span><span style="font-weight: bold;" class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span><span class="bold"> if the Jira user does not have a </span><span style="font-weight: bold;" class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span><span class="bold"> account</span> is set to <span class="bold">Always</span>. This user does not occupy a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> license. Active users can be assigned to work items in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, but cannot be included in updates. For more information about configuring the automatic creation of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> users from Jira, see <a href="configure-workfront-for-jira.md">Configuring <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for Jira</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue Attachments</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> Issue or Task Documents<br>A comment about uploading a new document in Jira is added to the Updates tab of the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> issue or task.&nbsp; </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Due Date</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> A comment about the change of the Due Date in Jira is added to the Updates tab of the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> issue or task.&nbsp;</p> <p>Note: No dates change on the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> issue or task.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Log time in the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> right panel or from the More menu on the Jira issue<br></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Hours<br>In addition to adding the hours logged in Jira to the linked <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> item, a comment about logging time is added to the Updates tab of the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> item.</p> <p>For more information about logging time on linked Jira issues, including updating the Jira user who is logging the time in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, see <a href="#logging-time-for-linked-jira-and-workfront-items" class="MCXref xref">Log time for Linked Jira and Workfront items</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> Comments&nbsp;<br><br></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Comments are added to the Updates tab of the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> issue or task if the <span class="bold">Comments</span> setting in the SYNCHRONIZE FROM JIRA TO WORKFRONT section of the Setup tab to <span class="bold">Always</span>.</p> <p>For information about configuring <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> settings in Jira, see <a href="configure-workfront-for-jira.md">Configuring <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for Jira</a>.</p> <p>For information about commenting on items from linked Jira issues, see <a href="#commenting-from-linked-jira-issues" class="MCXref xref">Comment from a linked Jira issue</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Log time from linked Jira issues {#log-time-from-linked-jira-issues}

The time that you record for a Jira item in Jira will also transfer to the linked *`Workfront`*&nbsp;item, regardless of where in Jira you log the time.  
When you log time in Jira in the *`Workfront`* panel, the time is recorded only in *`Workfront`*.  
The time you record in *`Workfront`* does not affect the time of the linked issue in Jira.&nbsp;


>[!NOTE]
>
>If the time is added to a Jira item linked to a *`Workfront`* task, the Hour Type for the time in *`Workfront`* is Task Time. If the time is added to a Jira item linked to a *`Workfront`* issue, the Hour Type for the time in *`Workfront`* is Issue Time. 


A comment is added to the ` *`Workfront`*` tab in Jira and to the `Updates` tab of the item in *`Workfront`* to record logging the time.  
The time is also displayed in the `Hours` tab of the *`Workfront`* item.&nbsp;



* [Log time for Linked Jira and Workfront items](#logging-time-for-linked-jira-and-workfront-items)&nbsp;
* [Log time from Jira to a Workfront item](#logging-time-for-workfront-items-only) 




### Log time for Linked Jira and *`Workfront`* items {#log-time-for-linked-jira-and-workfront-items}

You can log time from a Jira issue linked to a *`Workfront`* item, and the time is recorded both on the Jira issue as well as the *`Workfront`* item.&nbsp;


>[!IMPORTANT] {type="important"}
>
>If the user logging the time in Jira does not exist in *`Workfront`*, the integration creates a new active user in *`Workfront`* if the `Automatically create a user in` *`Workfront`* `if the Jira user does not have a` *`Workfront`* `account` is set to `Always`. This user does not occupy a *`Workfront`* license. You can assign active users to work items in *`Workfront`*, but you cannot include them in updates. For information about configuring the automatic creation of *`Workfront`* users from Jira, see [Configuring *`Workfront`* for Jira](configure-workfront-for-jira.md).


To log time for an item in Jira and have it recorded both in Jira and *`Workfront`*:



1. Log into Jira.
1. Go to the Jira issue which is linked to the *`Workfront`* item.
1. Expand the `More` menu and click `Log work`.  
   ![log_time_from_More_menu_in_Jira.png](assets/log-time-from-more-menu-in-jira-239x232.png)  

1.  In the `Time Spent` field, specify the amount of time spent working on this issue. You must specify the time using the following time periods:  

    
    
    * Weeks (w)
    * Days (d)
    * Hours (h)
    
    

1. Continue adding information to your time entry, including a `Work Description`, then click `Log`.  
   The time is added to the `Work log` tab of the Jira item, as well as to the *`Workfront`* item linked to it.  
   The work description of the time entry is recorded as a note on the hour entry in *`Workfront`*.&nbsp;





### Log time from Jira to a *`Workfront`* item {#log-time-from-jira-to-a-workfront-item}

You can log time just to the linked *`Workfront`* item from the Jira issue without recording this time to the Jira issue.&nbsp;



1. Log into Jira.
1.  Navigate to a Jira issue which is linked to a *`Workfront`* item.  



   The details of the *`Workfront`* item should display in the *`Workfront`* right panel of the issue.

1.  Click the `Log Time` icon.  



   ![Log_time_in_Jira.png](assets/log-time-in-jira.png)



1. Specify the amount of `Hours` and `Minutes` you want to log for the issue.

1.  Click `Log Time`.  



   The time is added to the *`Workfront`* item.


   This time is not added to the Work Log tab of the Jira issue.&nbsp;





## Comment from a linked Jira issue {#comment-from-a-linked-jira-issue}

When you comment on a Jira item from the *`Workfront`* right panel in Jira, the comment is also added to the Updates tab of the linked item in *`Workfront`*.&nbsp;


To comment from Jira to a *`Workfront`* item:



1. Log into Jira.
1.  Navigate to a Jira issue which is linked to a *`Workfront`* item.  



   The details of the *`Workfront`* item should display in the *`Workfront`* right panel of the issue.

1.  Click the `Comments` icon in the *`Workfront`* panel or n the `Comments` tab. ![Jira_comments_icon.png](assets/jira-comments-icon.png)  

1.  Start typing a comment, then click `Send`.


   The comment is added to the following:

    
    
    * The ` *`Workfront`*` tab of the Jira issue.
    * The `Comments` tab of the Jira issue.
    * The `Updates` tab of the linked item in *`Workfront`*.
    
    
    



