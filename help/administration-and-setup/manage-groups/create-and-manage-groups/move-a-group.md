---
filename: move-a-group
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
---



# Move a group {#move-a-group}

You can move a group under another group that you manage.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the group<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
      s
     </MadCap:conditionalText> or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *`Workfront administrator`*.


## Move a group {#move-a-group-1}

To move a group, you edit the destination parent group.


>[!NOTE]
>
>If the statuses of the moved group are locked, it inherits the statuses of its new parent group.
>
>
>If the statuses of the moved group are unlocked, it does not inherit the statuses of its new parent group, nor does the new parent group take on its statuses.
>
>
>For more information about group statuses, see [Create or edit a status](create-or-edit-a-status.md) and [Create or edit a group status](create-or-edit-a-group-status.md).






1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups` ![](assets/groups-icon.png).

1. Select the destination group where you want to move the group, then click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> the Edit icon  <img src="assets/edit-icon.png"></MadCap:conditionalText>`. 
1.  In the `Edit Group` box that appears, under `Group Members and Group Administrators`, start typing the name of the group you want to move, then click it when it appears.
1. Click `Save`.


