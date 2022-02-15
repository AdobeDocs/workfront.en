---
filename: delete-a-group
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
---



# Delete a group {#delete-a-group}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


You can delete a group that you manage. If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for *`Workfront administrators`* (for any group).


For information about deleting a subgroup, see [Manage a group](manage-a-group.md).


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


## Delete a group {#delete-a-group-1}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups` ![](assets/groups-icon.png).

1.  Select the group you want to delete, then click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> the Delete icon  <img src="assets/delete.png"></MadCap:conditionalText>`.


   >[!IMPORTANT] {type="important"}
   >
   >When you delete a group or subgroup, you need to preserve the users, work items, and any subgroups that are currently assigned to it. To help you make sure they are preserved, a prompt requires you to reassign the group’s objects to a different group in the step below.



1.  In the `Delete Group` box that appears, starting typing and then select the name of the group where you want to move the members, work items, and subgroups of the group you are deleting.


   You can make sure you are selecting the right group by hovering over it and clicking the information icon ![](assets/info-icon.png) that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  Depending on the details configured for the group, you might also see its Business Leader and description.</MadCap:conditionalText>`

1. Click `Delete Them`.


