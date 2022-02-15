---
filename: link-items-between-wf-jira
product-area: workfront-integrations
navigation-topic: workfront-for-jira
---



# Link items between *`Adobe Workfront`* and Jira {#link-items-between-adobe-workfront-and-jira}

You can link Jira issues to *`Adobe Workfront`* tasks or issues either automatically or manually.&nbsp;


Only one item in *`Workfront`* can be linked to one item in Jira. You can never link one *`Workfront`* item to multiple Jira issues, nor one Jira issue to multiple *`Workfront`* items.


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
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



*  Install *`Workfront`* for Jira


  For instructions on installing *`Workfront`* for Jira, see [Install Adobe Workfront for Jira](install-workfront-for-jira.md).

*  Configure *`Workfront`* for Jira


  For instructions on configuring *`Workfront`* for Jira, see [Configure Adobe Workfront for Jira](configure-workfront-for-jira.md).





## Automatically link *`Workfront`* items to Jira issues {#automatically-link-workfront-items-to-jira-issues}

As a *`Workfront administrator`*, you can define triggers that can automatically create an issue in Jira every time certain conditions are met on a task or an issue in *`Workfront`*. The *`Workfront`* and Jira items become linked.


After you have completed the configuration of *`Workfront`* for Jira, when an item is either created or updated in *`Workfront`* to match your triggers, a new item is automatically created in Jira.   
*`Workfront`* users that create and update *`Workfront`* items do not need a Jira license to trigger the creation of items in Jira.


For more information about defining triggers for creating Jira issues automatically, see&nbsp; [Configure Adobe Workfront for Jira](configure-workfront-for-jira.md).


>[!NOTE]
>
>You can create Jira items automatically by attaching a template to a project. If the template contains tasks with assignments&nbsp;that meet the Jira triggers, the new tasks generate new Jira issues.&nbsp;


Automatically linking a *`Workfront`* issue to a Jira issue is identical to automatically linking a *`Workfront`* task to a Jira issue.  



To automatically link a *`Workfront`* task to a Jira issue:



1.  Ensure that your Jira system administrator has configured triggers for automatically creating Jira issues when *`Workfront`* items are assigned, then log in to *`Workfront`* with an access level that allows you to create a task.  



   For more information about access to tasks, see [Grant access to tasks](grant-access-tasks.md).

1. Go to a project and select `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold">Tasks </span> <img src="assets/tasks-icon-in-left-panel-14x14.png" style="width: 14;height: 14;"> in the left panel</MadCap:conditionalText>`.  

1.  Click `New Task`


   Or


   Select an existing task, then click `Edit`.&nbsp;

1. Specify or update any of the fields available for the task.&nbsp;
1. Click `Assignments` and assign the task to a user, role, or team which is specified as a trigger in the Jira integration.  

1.  Click `Save Changes`.  



   A new task is created in *`Workfront`*.   



   In the `Updates` `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> area</MadCap:conditionalText>` of the new task, there is a comment to indicate that a new issue has also been created in Jira.  



   ![WF_confirmation_that_Jira_issue_was_created.png](assets/wf-confirmation-that-jira-issue-was-created-350x43.png)   


1.  (Optional) Click the link to the Jira issue to open it in Jira.


   Or


   In the `Integrations` area on the Details panel of the task, click the `Go to Jira` link to open the Jira issue.


   Any Jira user can immediately start working on items automatically created from *`Workfront`* and their updates will transfer to *`Workfront`* without needing a license for *`Workfront`* to do so.


   Only the fields that you as a *`Workfront administrator`* configured during the setup of the *`Workfront`* add-on are updated.


   For more information about synchronizing fields between *`Workfront`* and Jira, see the&nbsp; [Configure Workfront for Jira](configure-workfront-for-jira.md#configuring-the-add-on-for-jira)&nbsp;section in&nbsp; [Configure Adobe Workfront for Jira](configure-workfront-for-jira.md).


   >[!NOTE]
   >
   >The Jira issue is not assigned to anyone in Jira when it is automatically created from *`Workfront`*.  








## Manually link Jira issues to *`Workfront`* items {#manually-link-jira-issues-to-workfront-items}

After items have been created in Jira and *`Workfront`*, independent of each other, you can manually link a Jira issue to an existing *`Workfront`* task or issue.  
You cannot manually link a *`Workfront`* item from *`Workfront`* to an existing Jira item.&nbsp;


>[!NOTE]
>
>If the Jira issue is not on a project which is not identified as a trigger in the *`Workfront`* Integration you cannot manually link it to a *`Workfront`* item when using the integration with Jira On-Premise.&nbsp;&nbsp;  
>For more information about setting up triggers for the *`Workfront`* to Jira workflow, see [Automatically link Workfront items to Jira issues](#automatically-linking).


When *`Workfront`* and Jira items are linked, certain fields from one item can be automatically updated on the other.  
For more information about updating linked items, see [Update linked items between Jira and Adobe Workfront](update-linked-items-between-jira-wf.md).


To manually link Jira issues to *`Workfront`* items:



1. (Conditional) Log in to *`Workfront`* and find an issue or a task that you want to link to Jira issue.&nbsp;
1. (Conditional) From the address bar of the item, copy the `URL` of the item in *`Workfront`*.  
   Or

1.  From the Details `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> area  <img src="assets/details-icon-in-left-panel.png"></MadCap:conditionalText>`, copy the `Reference Number` of the item in *`Workfront`*.&nbsp;


   >[!NOTE]
   >
   >You must have a *`Workfront`* license to log in to *`Workfront`*. Otherwise, a *`Workfront`* user must supply this information to you.&nbsp;



1. In Jira, navigate to an issue that you want to manually link to the *`Workfront`* item.
1. In the *`Workfront`* right panel, paste the `URL` or the `Reference Number` of the *`Workfront`* item which you want to link to it.  
   ![manually_link_items_Jira_WF.png](assets/manually-link-items-jira-wf-350x174.png)


1.  Click `Link`.


   The two items become linked and the *`Workfront`* right panel is populated with information from the *`Workfront`* item.


   The following *`Workfront`* fields are visible in Jira, by default, in the *`Workfront`* right panel:

    
    
    * The `Name` of the item: You can access the *`Workfront`* item by clicking the name in the panel.&nbsp;
    
    * `Project Name` 
    * The `Status` of the item
    * The `Priority` of the item
    * The date on which it was created in *`Workfront`*
    * The `Planned Hours` of the item
    * The `Reference Number`: You can access the *`Workfront`* item by clicking the Reference Number in the panel.
    
    
    



For more information about enabling additional fields to display in the right panel, see [Configure field synchronization between Jira and Workfront Items](configure-workfront-for-jira.md#setting-up-field-synchronization) section in [Configure Adobe Workfront for Jira](configure-workfront-for-jira.md). A comment from the *`Workfront administrator`* associated with the integration is posted in the ` *`Workfront`*` tab of the Jira issue to confirm that a new Jira item has been created. The comment contains a link to the Jira issue.


![Jira_confirmation_of_the_Jira_issue_created_Workfront_tab.png](assets/jira-confirmation-of-the-jira-issue-created-workfront-tab-350x84.png)




## Unlink items between Jira and *`Workfront`* {#unlink-items-between-jira-and-workfront}

Linked items between Jira and *`Workfront`* can be manually unlinked from Jira.  
You cannot unlink a *`Workfront`* item from their Jira counterpart in *`Workfront`*.&nbsp;


You need the following access to unlink manually linked item:



* You are the user who manually linked the items
* You are the Jira system administrator


Only a *`Workfront administrator`* can unlink items that were automatically linked.&nbsp;


To unlink a Jira issue from a *`Workfront`* item:



1. In Jira, navigate to an issue which is linked to a *`Workfront`* task or issue.
1. Go to the *`Workfront`* right panel, and click the `Unlink` icon, then click `Unlink`.  
   ![Jira_WF_unlink_icon.png](assets/jira-wf-unlink-icon-350x222.png)  
   The previously linked Jira and *`Workfront`* items are now unlinked. Any fields, comments, or documents that might be updated on them individually in the future are not updated on their previous counterpart in the other application.&nbsp;



