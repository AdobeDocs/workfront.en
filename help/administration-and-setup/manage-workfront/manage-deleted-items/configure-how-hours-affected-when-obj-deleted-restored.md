---
filename: configure-how-hours-affected-when-obj-deleted-restored
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
---



# Configure affect on hours when an object is deleted and restored {#configure-affect-on-hours-when-an-object-is-deleted-and-restored}

You can configure what happens to hours when someone deletes a project, task, or issue that the hours are logged against. The option you choose also determines what happens to the hours if the project, task, or issue is restored at a later time. (For more information about restoring items in *`Workfront`*, see [Restore deleted items](restore-deleted-items.md).)


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Configure how hours are managed when an item is deleted and restored {#configure-how-hours-are-managed-when-an-item-is-deleted-and-restored}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).  

1. Expand  `Timesheets & Hours`, then click `Preferences`.

1. Locate the `Project, Task or Issue Deletion Preferences` section.
1. (Conditional) To configure how hours are managed when a project is deleted, select one of the following options in the `When deleting projects` section:
1.  `<li>Keep logged hours already added to timesheets as general hours (If this project is restored at a later time, the hours remain on the timesheet)<br>This option is selected by default.</li>` `<li>Delete any logged hours (If this project is restored at a later time, logged hours are restored to the project)</li>` 

1. (Conditional) To configure how hours are managed when a task or issue is deleted, select one of the following options in the `When deleting tasks or issues`&nbsp;section:
1.  `<li>Move any logged hours to the project where the task or issue resides (If this task or issue is restored at a later time, the hours remain on the project)<br>This option is selected by default.</li>` `<li>Delete any logged hours (If this task or issue is restored at a later time, logged hours are restored to the task or issue)</li>` 

1. Click `Save`.


