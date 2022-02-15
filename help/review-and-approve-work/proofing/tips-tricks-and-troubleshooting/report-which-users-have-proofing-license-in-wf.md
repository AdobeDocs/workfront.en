---
filename: report-which-users-have-proofing-license-in-wf
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
---



# List users with a *`proofing`* license in *`Adobe Workfront`* {#list-users-with-a-proofing-license-in-adobe-workfront}

You can view which users in *`Adobe Workfront`* currently have the option "User can generate *`proofs`*" enabled in either of the following ways below.


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Plan</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or *`Proof Permission Profile`* you have, contact your *`Workfront`* or *`Workfront Proof administrator`*.


## Create a user report {#create-a-user-report}

You can create a user report to view which users can generate *`proofs`*:



1. Navigate to `Reporting` area.
1. Click the  `New Report` drop-down menu, then click  `User Report`.

1. On the `Filters` tab, click `Add a Filter Rule`.

1. In the available field, expand `User`, then click `Has Proof License`.

1.  Select `Equal` > `True`.


   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)



1.  Click `Save+Close`.  



   The report displays all users in *`Workfront`* who have a *`proofing`* license assigned to them.





## Update the People view {#update-the-people-view}

You can add a new column in the People view to view which users can generate *`proofs`*:



1. Go to the `People`&nbsp;area.
1. Click the `People` tab.
1. In the `View` drop-down menu, do either of the following: 
    
    
    * To add this information to an existing view, select the view you want to customize, then click `Customize View`.
    * To add this information to a new view, click `New View`.
    
    

1. Click `Add Column`.
1. In the available field, expand `User`, then click `Has Proof License`.

1.  Click `Done`, then click `Save View` or `Save as New View`.  



   The view displays `True` or `False` depending on whether the user has a *`proofing`* license assigned to them.



