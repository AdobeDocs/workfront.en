---
filename: create-and-modify-a-groups-timesheet-profiles
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
---



# Create and manage a group’s timesheet profiles {#create-and-manage-a-group-s-timesheet-profiles}

When you are viewing a group that you manage in the Groups area, you can view and work with the *`timesheet profiles`* for which the administrators of the group, or one of its subgroups, have administrative access. 


If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for *`Workfront administrators`* (for any group).


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must have administrative access to timesheets. For more information, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions.HIDE">Or, in order to work on <span class="mc-variable Snippet_Variables.Object variable varname">timesheet profiles</span> for a group, you must be an administrator of the group or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref" data-mc-variable-override="">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Create and edit group-level timesheet profiles {#create-and-edit-group-level-timesheet-profiles}

You can create and edit timesheet profiles for use in a group you manage. For instructions, see [Create, edit, and assign timesheet profiles](create-timesheet-profiles.md).


## Delete group-level timesheet profiles {#delete-group-level-timesheet-profiles}

You can delete timesheet profiles in use by a group you manage. For instructions, see [Delete timesheet profiles](delete-timesheet-profiles.md).


## Manually generate group timesheets {#manually-generate-group-timesheets}

To enable changes that you made to group timesheet profiles to reflect&nbsp;in current group timesheets, you have to first delete the existing timesheets and then manually generate new ones. For instructions, see [Manually generate timesheets from the Timesheets area](manually-generate-timesheets.md#manually) in [Manually generate timesheets](manually-generate-timesheets.md).


For information about on deleting group timesheets, see [Delete generated timesheets](delete-timesheets.md).


## Export group-level timesheet profiles {#export-group-level-timesheet-profiles}




1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).
1.  Click **Groups**.


   In the list of groups that displays, *`group administrators`* can see the groups they manage, as well as any subgroups of those groups. *`Adobe Workfront administrators`* can see all groups.

1.  Click the name of the group with the timesheet profiles you want to export.
1.  Click **Timesheet Profiles**.
1.  Click **Export** to export the list of timesheet profiles for the group.


