---
filename: create-or-edit-a-group-status
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
---



# Create or edit a group status {#create-or-edit-a-group-status}

As a *`group administrator`*, you can create custom statuses for a group that you manage. This helps to eliminate the need for dozens of company-wide custom statuses and allows more autonomy in your group hierarchies.


You can also edit a system-level status for a group you manage if a *`Workfront administrator`* has unlocked the status. For more information, see [Locking or unlocking a custom system-level status](lock-or-unlock-a-custom-system-level-status.md).


If there are any groups above your group, their administrators can also do these things for your group. The same is true for *`Workfront administrators`* (for any group).


>[!NOTE]
>
>Custom group statuses can't be displayed on a project when viewing the project in an agile view. Only default and custom locked statuses are visible when viewing a project in an agile view. For information about customizing an agile view for a project, see the section [Views overview in Adobe Workfront](views-overview.md#customizing-an-agile-view) in the article [Views overview in Adobe Workfront](views-overview.md).  



For general information about statuses, see [Statuses overview](statuses-overview.md).


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the group or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *`Workfront administrator`*.


## Create or edit a status for a group {#create-or-edit-a-status-for-a-group}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups` ![](assets/groups-icon.png).

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the name of</MadCap:conditionalText>` the group where you want to create or customize statuses.
1.  `In the left panel, click `Statuses`.` 

   If the group you are viewing is a top-level group, the list that displays includes the following:

    
    
    * System-level locked statuses.
    * Custom statuses already created for the group.
    
    
   In addition, if the group you are viewing is a subgroup, the list also includes:

    
    
    * Locked statuses belonging to the groups above the subgroup.
    *  Unlocked statuses that belonged to the groups above the subgroup when it was created.
    
    
      After a subgroup is created, unlocked statuses that are created in the groups above it are not included in the subgroup’s status list. However, if someone locks one of them later, it is then included in the subgroup’s status list. For more information, see [How groups inherit statuses](how-groups-inherit-statuses.md).
    
    
    

1. Select the tab of the object type ( `Project`, `Tasks`, or `Issues`) that you want to associate with the status.

1.  (Conditional) If the status is an issue status, make sure that `Master List` is selected.


   ![](assets/screenshot-2016-05-10-17.29.08-350x185.png)




   For information about customizing the other issue types (Bug Report, Change Order, Issue, Request), see [Customize default issue types](customize-default-issue-types.md).

1.  (Conditional) To create a new status, click `Add a New Status`.


   Or


   To edit an existing status, mouse over the status you want to edit, then click the `Edit` option that displays to the far right.


   ![](assets/group-statuses-edit-350x201.jpg)




   >[!NOTE]
   >
   >
   >    
   >    
   >    * You can edit a status for your group only if:   >    
   >        
   >        
   >        * You manage the group that the status was created for
   >        * A *`Workfront administrator`* unlocked the status at the system level
   >        * A *`group administrator`* of a group above your group unlocked the status
   >        
   >        
   >    * When you are editing an existing status, you can change only its name, description, and color.
   >    *  When you edit a locked status, your changes affect all subgroups that inherited the status from your group.
   >    
   >    
   >      Conversely, editing an unlocked status does not affect the subgroups that inherited the status from your group.  

   >    
   >    
   >    




1.  Specify the following information.


   If you are editing a status, only the first 3 settings can be changed.

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Status Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Type a name for the status. This is a required field.</p> <p>When you create a status name, be aware that others in the system can create a status with the same name. We recommend using a unique name to avoid confusion when selecting statuses in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">(Optional) Type a description of the status. This communicates its purpose to those who use it.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Color</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Customize the color of the status by clicking the color field and selecting a color from the swatch panel. You can also enter a hex number in the field.</p> <p>The status color displays in the upper-right corner of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> when a user views the object.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/status-color-350x211.png" style="width: 350;height: 211;"> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Equates With</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select one of the options from the list that best describes the function of the status. For example, if the status name is Done, the option it equates with should be Complete.</p> <p>Every status must equate with one of these options because this determines how the status functions.</p> <p>This option cannot be modified after the status is created.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Key</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>If you are creating a new status, type a code or abbreviation for the status or use the one generated for you. This key must be unique in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> because it can be used for reporting purposes. If you attempt to specify a key that is already in use in the system, the field turns red.</p> <p>It might be useful to use an abbreviation that is recognizable to those who will use it.</p> <p>This option cannot be modified after the status is created.</p> <p>You cannot change the key code for Planning, Current, and Complete statuses. This is important if you are building a report in text mode.<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Hide Status</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>(Project and Task statuses only)</p> <p>Enable this option if you want the status hidden from users. When it is disabled (the default setting), all <MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
      subgroups below the group
     </MadCap:conditionalText> can use the status.</p> <p>Tip: You can hide an Issue status by disabling all 4 issue types (Bug Report, Change Order, Issue, Request).</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Lock for all groups</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p data-mc-conditions="SnippetConditions-wf-groups.groups">If you leave this option enabled, the users in your group and its subgroups can see and use the status and <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> cannot customize it for lower subgroups.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">When this option is disabled, <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> can customize the status for lower subgroups.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">For more information about locking statuses, see <a href="lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Locking or unlocking a custom group status</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Save`.


   The status is now available for all projects associated with your group or subgroup. If you locked it, it is available for use by any lower subgroups.


   You can configure the status to be a default status for the group. For more information, see [Use a custom status as a default status for a group](use-custom-statuses-as-default-statuses-group.md).





## Create a custom status for multiple groups {#create-a-custom-status-for-multiple-groups}

If you are a *`Workfront administrator`*, you can create a custom status for multiple groups by creating a system-wide status, then hiding that status from any groups that don’t need it.


If you are a *`group administrator`* (or a *`Workfront administrator`*), you can create a custom status for multiple subgroups within a group hierarchy you manage by creating a status for a higher level group, then hiding that status from any lower subgroups that don’t need it.



1.   If you are a *`Workfront administrator`*, create a system-wide unlocked status as described in [Create or edit a status](create-or-edit-a-status.md).


   Or


   If you are a *`group administrator`* (or *`Workfront administrator`*), create an unlocked group status as described in [Create or edit a group status](#).

1.  In the box in the upper-right corner, delete `System Statuses`, begin typing the name of a group where you want to hide the status, then click the name when it appears.
1.  Hover over the status you want to hide from the group, then click `Edit` when it appears.


   ![](assets/hover-click-edit-350x148.jpg)



1.  Enable the `Hide Status` option that appears. 


   ![](assets/hide-group-status-350x114.png)



1.  Click `Save`.


   The status is dimmed and no longer visible to all users in that group.

1. Repeat steps 5 through Step 8 to hide the custom status from any other groups who don't need it.


