---
filename: configure-workfront-for-jira
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
---



# Configure *`Adobe Workfront`* for Jira {#configure-adobe-workfront-for-jira}

You can use *`Adobe Workfront`* for Jira to integrate your Jira and *`Workfront`* systems.


After installing the add-on, you can define workflows that create Jira issues automatically when *`Workfront`* work items are created. The items in both applications become linked, and some of their information automatically updates in both systems.


All users in *`Workfront`* and Jira can benefit from this integration. They only need a license for the system in which they work the most, and not for both systems.&nbsp;


This add-on is available for both the Server and OnDemand (or Cloud) versions of Jira Software.


For a list of Jira versions that *`Workfront for Jira`* currently supports, see [ *`Workfront for Jira`*](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) at the Atlassian Marketplace.



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

Before you can configure *`Workfront`* for Jira, you must



* Install *`Workfront`* for Jira  
  For instructions on installing *`Workfront`* for Jira, see [Install Adobe Workfront for Jira](install-workfront-for-jira.md).





## Configure *`Workfront`* for Jira {#configure-workfront-for-jira}

By configuring *`Workfront`* for Jira you can:



* Define triggers that will create Jira items when *`Workfront`* items are created.
* Specify which fields should synchronize between items linked between Jira and *`Workfront`*.




>[!NOTE]
>
>
>
>
>*  After you configure *`Workfront`* for Jira on your Jira environment, all Jira users see a *`Workfront`* right panel on all Jira items. The panel contains information about the items that might be linked from *`Workfront`* or specifies that no *`Workfront`* items are linked to Jira items.&nbsp;
>
>* When using the Jira Server installation, only the issues that are associated with projects identified as triggers for the *`Workfront`* integration display the *`Workfront`* panel. For more information about setting up triggers for the *`Workfront`* to Jira workflow, see [Configure triggers for automatically linking items between Jira and Workfront](#configuring-triggers).
>
>
>



To configure *`Workfront`* for Jira:



1. Log into Jira as a Jira administrator.
1. Click `Settings` in the main Jira menu.
1. Click `Add-ons`, then click `Manage add-ons`.

1. Expand the ` *`Workfront`*` add-on.
1. Click `Configure`.
1.  Follow the prompts to log in to *`Workfront`* using Enhanced Authentication, OAuth 2.0, or your Security Assertion Markup Language (SAML) URL.


   You must log in to *`Workfront`* as a *`Workfront administrator`* to continue the configuration.


   >[!NOTE]
   >
   >
   >    
   >    
   >    * When you are prompted to enter the *`domain`* of your *`Workfront`* account, type it using this format: *yourCompany'sDomain.my.workfront.com*. Your company's domain is usually the name of your company.
   >    
   >    * Enhanced Authentication is not available until a *`Workfront administrator`* enables it for this integration. 
   >    
   >    




1.  Select the `Triggers` tab to configure the automatic creation of Jira items as new *`Workfront`* items are created.  



   For more information about setting up triggers for the *`Workfront`* to Jira workflow, see [Configure triggers for automatically linking items between Jira and Workfront](#configuring-triggers).

1.  Select the `Setup` tab to configure the synchronization of fields between linked Jira and *`Workfront`* items.


   For more information about setting up the synchronization of fields between Jira and *`Workfront`*, see [Configure field synchronization between Jira and Workfront Items](#setting-up-field-synchronization).


   >[!NOTE]
   >
   >After you defined the triggers and the synchronization of fields between the two applications, any *`Workfront`* user who can create tasks or issues could potentially trigger the creation of an item in Jira. The user can create an item if the criteria on the item they create match the triggers in Jira, even if the user does not have a Jira license. Also, any Jira user can immediately start working on the Jira item, and their updates are visible in *`Workfront`*, without them having a *`Workfront`* license. Any updates in *`Workfront`* are also visible on the Jira items.&nbsp;



1.  (Optional) Select the `Activity Log` tab to review any errors that might have occurred during the integration.


   For more information about the Activity Log, see [View the Jira Activity Log](view-the-jira-activity-log.md).  






## Configure triggers for automatically linking items between Jira and *`Workfront`* {#configure-triggers-for-automatically-linking-items-between-jira-and-workfront}

As the Jira system administrator, you can define triggers that would automatically create issues in Jira when an item in *`Workfront`* meets certain criteria. 


>[!NOTE]
>
>It could take up to 10 minutes for the integration to create new issues in Jira.


Consider the following when configuring triggering the creation of Jira items as *`Workfront`* items are created:



* The integration is unidirectional: You can only trigger items that you create in *`Workfront`* to be automatically created in Jira. You cannot trigger items that you create in Jira to automatically be created in *`Workfront`*.&nbsp;

* There is no limit to how many triggers you can have.&nbsp;
* If an item that you create in *`Workfront`* matches more than one of the triggers, only one item is created in Jira. The item is created in Jira according to the first trigger (in the order that they have been defined in Jira). All other triggers are ignored.&nbsp;
* Only one item in *`Workfront`* can be linked to one item in Jira. You can never link one *`Workfront`* item to multiple Jira issues, or one Jira issue to multiple *`Workfront`* items.&nbsp;



To configure triggers for automatically creating items in Jira:&nbsp;



1. Log into Jira as a system administrator.
1. Click `Settings` in the main Jira menu.
1. Click `Add-ons`, then `Manage add-ons`.

1. Expand the ` *`Workfront`*` add-on.
1. Click `Configure`.
1.  Log in to *`Workfront`* as a system administrator.


   The  `Triggers` tab is selected by default.


   ![Triggers_tab_Jira_WF.png](assets/triggers-tab-jira-wf-350x220.png)



1. Click `Add trigger` to add a new trigger.
1.  In the ` *`Workfront`* team/user/role` field, specify the name of a *`Workfront`* team, user, or job role, then click to select it when it displays in the list.&nbsp;


   >[!NOTE]
   >
   >You cannot have multiple triggers for the same team, user, or role.


   When someone creates a task or an issue and assigns it to one of these entities, an issue is automatically created in Jira.






1.  In the `Jira project` field, start typing the name of a Jira project, then click to select it when it displays in the list.


   When the Jira issue is created, it is placed on the project you specify here.  


1.  Select an `Issue type` from the drop-down menu.


   This indicates the issue type that is created in Jira when the conditions of this trigger are met, based on your settings for that specific project in Jira.  


1.  Click `Save`.&nbsp;


   With this configuration, every time a *`Workfront`* user creates an item that matches the specified triggers, a new issue is created in Jira.  






## Configure field synchronization between Jira and *`Workfront`* Items {#configure-field-synchronization-between-jira-and-workfront-items}

As the Jira administrator, you can define what fields should automatically synchronize on items that are linked between *`Workfront`* and Jira. Certain fields can synchronize from the *`Workfront`* to the Jira item, and others synchronize from Jira to *`Workfront`*.&nbsp;


To define what fields should automatically synchronize on items linked between the two applications:



1. Log into Jira as a Jira administrator.
1. Click `Settings` in the main Jira menu.
1. Click `Add-ons`, then `Manage add-ons`.

1. Expand the ` *`Workfront`*` add-on.
1. Click `Configure`.
1. Log in to *`Workfront`* as a *`Workfront administrator`*.

1.  Click the `Setup` tab.


   ![](assets/jira-newsetuptab-350x273.png)   


1. In the `Synchronize from Jira to Workfront` section, select the fields that you want to update in Jira when they are updated in *`Workfront`*.&nbsp;
    
    
    1. Select any of the following frequencies with which the fields are synchronized: 
    
    
    
    1. Select to synchronize any of the following fields from *`Workfront`* to Jira:&nbsp; 
    
    
    <table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Name</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>The name of a task or an issue in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> becomes the name of the issue to which it is linked in Jira.</p><p>Note: When new items are created in Jira automatically, the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Name always updates on the Jira item, regardless of whether this field is enabled here or not. When a Jira item is manually linked to a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> item, the Name of the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> item only updates in Jira when you select to&nbsp;<span class="bold">Always</span>&nbsp;synchronize this field.&nbsp;For more information about linking items manually or automatically, see <a href="link-items-between-wf-jira.md" class="MCXref xref">Link items between Adobe Workfront and Jira</a>.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Description</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The description of a task or an issue in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> becomes the description of the issue to which it is linked in Jira.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Documents</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Documents attached to a task or an issue in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> are also attached to the issue to which it is linked in Jira. New document versions from <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> are added as separate documents to Jira and are appended with <i>_v&lt;version number&gt;</i> to indicate the numbered version in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. </p><p>For example, if the name of a document in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> is <span class="bold">Main Ad</span>, and you add a new version to it in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the new version is transferred to Jira as a new document with the name <span class="bold">Main Ad_v2</span>.</p><p>Important: <p>Consider the following when syncing documents:</p>
     <ul>
      <li><p>Documents larger than 5MB do not sync. If a document sync fails because the document is too large, an error is logged in the Activity log, </p><p>For more information on the activity log, see <a href="view-the-jira-activity-log.md" class="MCXref xref">View the Jira Activity Log</a>.</p></li>
      <li><p>Documents that are linked to tasks and issues from external servers are not transferred to the Jira items. Only documents uploaded directly on the task or the issue in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> are transferred to the linked issue in Jira.</p></li>
      <li><p>To create a proof from a document, you must generate the proof in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. </p><p>For more information on generating a proof, see <a href="generate-proof-for-a-document.md#create" class="MCXref xref">Create a proof for an existing document </a>in <a href="generate-proof-for-a-document.md" class="MCXref xref">Create a proof for a document</a>.<br></p></li>
     </ul></p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Planned Completion Date</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"><p>The Planned Completion Date of a task or an issue in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> becomes the Due Date of the issue to which it is linked in Jira.</p><p>Note: Ensure that you display <span class="bold">Due Date</span>&nbsp;on Jira issues, for this value to synchronize.</p></td>
  </tr>
 </tbody>
</table>    
    
    
    
    

1. In the `Synchronize from Jira to Workfront` section, select the fields that you want to update in *`Workfront`* when they are updated in Jira.&nbsp;
    
    
    1. Select any of the following frequencies with which the fields are synchronized: 
    
    
    <table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Always</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The fields you specify are always synchronized between the linked <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> and Jira items when the fields are updated in Jira.&nbsp;</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Never</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"><p>The fields you specify are never synchronized between the linked <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> and Jira items. There is no indication in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> that the field was updated in Jira.&nbsp;</p><p>Note: When you select Never, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> fields can still be manually updated from Jira in the left <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> panel of the Jira issue. Those updates appear only on <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> items in Jira and <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> and not on Jira items.</p></td>
  </tr>
 </tbody>
</table>    
    
    
    1. Select to synchronize any of the following fields from Jira to *`Workfront`*: 
    
    
    <table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Status</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The Status of an issue in Jira becomes the Status of the task or issue to which it is linked in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.<br>For more information about <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> statuses, see <a href="create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Assignee</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>The Assignee of an issue in Jira becomes the Assignee of the task or issue to which it is linked in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p><p>Important: When you assign an item in Jira to a user who does not have a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account, the integration creates a new active user in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only when the <span class="bold">Automatically create a user in </span><span style="font-weight: bold;" class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span><span class="bold"> if the Jira user does not have a </span><span style="font-weight: bold;" class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span><span class="bold"> account</span> is set to <span class="bold">Always</span>. This user does not occupy a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> license.&nbsp;Active users can be assigned to work items in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, but cannot be included in updates. </p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Attachments</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Attachments of an issue in Jira are also attached to the task or issue to which it is linked in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.&nbsp;</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Comments</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"><p>A comment on a Jira issue is also posted on the linked <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> item in the Updates area. Conversely, a comment posted in the Updates area for a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> task or issue syncs to Jira's native comment stream for the linked issue. </p><p>This is set to <span class="bold">Always</span> by default. If you select <span class="bold">Never</span> here, you can still post comments manually on a linked item either in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> or in Jira.</p></td>
  </tr>
 </tbody>
</table>    
    
    
    
    

1. In the `OTHER` section, select what additional fields should be updated between linked items.&nbsp; 
    
    
    1. Select an option to determine whether the fields you specify `Always` or `Never` update in Jira or *`Workfront`* when they are modified.
    
    1. Select from the following fields and updates: 
    
    
    <table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Copy <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Custom Data in the right panel in Jira</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Displays the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Custom Data of an item in the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> right panel.</p><p>Note:  Custom Form sections are displayed in the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> right panel with the access level of the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> System Administrator.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Copy <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Priority in the right panel in Jira</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Displays the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Priority of an item in the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> right panel.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Add an update in the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Updates tab about Due Date changes in Jira</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Adds a comment in the Update tab of the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> item when the Due Date changes in linked Jira item.</td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Automatically create a user in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> if the&nbsp;Jira user does not have a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"><p>The following scenarios exist:</p>
    <ul>
     <li>When you select <span class="bold">Always</span> you enable the integration to create a new <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> user every time a Jira user without a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account performs the following actions on a linked Jira issue:
      <ul>
       <li>Is assigned to a Jira issue</li>
       <li><p>Logs time to a Jira issue</p><p>This new user does not occupy a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> license. The default setting is Always.&nbsp;The user created this way in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> has "Jira" added to their name.</p><p><img src="assets/jira-wf-indication-of-user-created-by-jira-350x66.png" style="width: 350;height: 66;"></p></li>
      </ul></li>
     <li>When you select <span class="bold">Never</span>, the following things happen:
      <ul>
       <li>You are not able to see any Jira assignments on the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> items. In this case, only assignments made in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> display on the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> items.</li>
       <li>The time logged to a linked Jira issue by a user without a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account does not automatically transfer to the linked <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> item. You can still log time on the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> item in the right panel of the Jira issue.</li>
      </ul></li>
    </ul></td>
  </tr>
 </tbody>
</table>    
    
    
    
    

1.  Click `Save`.  



   Now, every time a user updates any of the fields specified in this configuration on an item in either Jira or *`Workfront`*, the linked item in the other application is updated as well.&nbsp;





## Troubleshooting {#troubleshooting}



### Items cannot be created in Jira because of trigger fields marked "Couldn't be found" {#items-cannot-be-created-in-jira-because-of-trigger-fields-marked-couldnt-be-found}



#### Problem {#problem}

When an error occurs with our *`Workfront`* for Jira application, *`Workfront`* disables the triggers to prevent further complications. When those triggers are disabled, they display as "Couldn't be found".


#### Solution {#solution}

Locate the error that disabled the triggers. You can find the error in the Workfront for Jira "Activity Log".


The most common cause of this behavior is the error "Field 'duedate' cannot be set. It is not on the appropriate screen, or unknown."


This error means that you are attempting to sync the "planned completion date" from Workfront to Jira. In order to do this, you must ensure that your Jira objects have a field called "Due Date". If they do not have this field, *`Workfront`* is unable to sync the planned completion date from Workfront and disables your triggers.


To resolve this error, try one of the following:



*  Ask your Jira administrator to update the affected Jira objects to ensure that they have a due date field.
*  Disable the synchronization of Workfront's planned completion date in the *`Workfront`* "Setup" page


