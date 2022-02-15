---
filename: view-the-jira-activity-log
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
---



# View the Jira Activity Log {#view-the-jira-activity-log}

As a Jira administrator, you can view the exceptions and errors that occur during the synchronization or creation of the tickets between *`Adobe Workfront`* and Jira in an Activity Log.&nbsp;


You can see up to 500 items in the Activity Log, and they are listed starting with the most recent ones.  



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



*  Install *`Workfront`* for Jira


  For instructions on installing *`Workfront`* for Jira, see [Install Adobe Workfront for Jira](install-workfront-for-jira.md).





## Access the Jira Activity Log:&nbsp; {#access-the-jira-activity-log}




1. Log into Jira as a system administrator.
1. Click `Settings` in the main Jira menu.
1. Click `Add-ons`, then `Manage add-ons`.

1. Expand the ` *`Workfront`*` add-on.
1. Click `Configure`.
1. Log in to *`Workfront`* as a system administrator.
1.  Select the `Activity Log`&nbsp;tab.


   View information about exceptions and errors that occurred during the creation of items or&nbsp;synchronization of fields between the two applications.


   The log includes the following fields: 

    
    
    * Date of the occurrence
    * The name of the user in Jira
    * Jira issue number
    * A brief description of the error that occurred.  
    
    



