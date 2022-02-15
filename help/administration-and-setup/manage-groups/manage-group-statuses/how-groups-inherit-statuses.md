---
filename: how-groups-inherit-statuses
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
---



# How groups inherit statuses {#how-groups-inherit-statuses}

When you list the statuses available for a group, you see the following



*  Custom statuses created for the group, as explained in [Create or edit a group status](create-or-edit-a-group-status.md).
*  Statuses inherited from the system and from higher in the group hierarchy, as explained in this article.




## Inheriting statuses {#inheriting-statuses}

Your group inherits statuses when any of the following things happen:



*  You create the group.
* An administrator locks a status in a higher level group.
* An administrator deletes another group and chooses your group to take its place.


The table below explains each of these circumstances.

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">When you create a group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>When you create a new group, it automatically inherits:</p> 
    <ul> 
     <li>Unlocked statuses in the group one level up, if the new group is a subgroup.</li> 
    </ul> 
    <ul> 
     <li>Locked statuses at the system level .</li> 
    </ul> 
    <div class="example" data-mc-autonum="<b>Example: </b>">
     <span class="autonumber"><span><b>Example: </b></span></span> 
     <p>Suppose that a group called Marketing has 2 subgroups called Marketing Communications and Branding.</p> 
     <p>A <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the Marketing group creates a new custom status called Discovery.</p> 
     <p>Later, you create a new subgroup under the Marketing group and call it Advertising.</p> 
     <p>Your subgroup inherits the Discovery status because you created the group after the other administrator created the unlocked Discovery status.</p> 
     <p>Because the subgroups Marketing Communications and Branding already existed below the Marketing group when this happened, they don't inherit the unlocked Discovery status.</p> 
    </div> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">When an administrator locks a status at a higher level</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>When a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> locks a status at the system level, your group inherits it along with all other groups in the system.</p> <p>Similarly, when an administrator locks a status for a group above your group, your group inherits it along with any other subgroups below the higher group.</p> <p>Note: Later, if an administrator unlocks one of these statuses at the system level or in a group above your group, your group retains the status that it inherited earlier. Now it is a separate version of the status and you can customize it just for your group.</p> 
    <div class="example" data-mc-autonum="<b>Example: </b>">
     <span class="autonumber"><span><b>Example: </b></span></span> 
     <p>The Marketing <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> locks the Discovery status mentioned above to make sure that all 3 subgroups have it.</p> 
     <p>Along with your Advertising group, the Marketing Communications and Branding groups have the Discovery status now. They inherited it when it was locked in the Marketing group above them.</p> 
     <p>The Marketing <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> then unlocks the Discovery status so that all 3 subgroups have their own version of the Discovery status. Now you and the administrators of the other 2 groups can customize the Discovery status to meet the needs of your groups.</p> 
    </div> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">When an administrator deletes a group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>When an administrator deletes a group and chooses yours to take its place in the system, your group inherits the custom statuses of the deleted group if they don't already exist in your group.</p> 
    <div class="example" data-mc-autonum="<b>Example: </b>">
     <span class="autonumber"><span><b>Example: </b></span></span> 
     <p>A group called Messaging needs to merge with your Advertising group, so a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> deletes the Messaging group and chooses your group to take its place.</p> 
     <p>The Messaging group had a unique status called In Process. Your Advertising group now has that status available for use.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>



## Inheriting status configurations {#inheriting-status-configurations}

When you create a top-level group, it inherits the following configurations from the system level. When you create a subgroup, it inherits the following configurations from the next higher group.



*  Default status configurations


  For information about these, see [Use custom statuses as default statuses](use-custom-statuses-as-default-statuses.md).  







*  Status display order configurations


  For information about these, see [Reorder system-level and group statuses](reorder-system-statuses.md).



If someone changes these configurations after your group is created, its statuses are not affected.
