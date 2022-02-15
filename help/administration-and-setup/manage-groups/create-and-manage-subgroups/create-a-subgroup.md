---
filename: create-a-subgroup
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
---



# Create a subgroup {#create-a-subgroup}

You can create a subgroup under a group you manage to organize users and projects and to assign access rights within *`Adobe Workfront`*.


If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for *`Workfront administrators`* (for any group).


Typically, however, *`group administrators`* manage groups and subgroups. They can use the Groups page to manage their groups and subgroups in one place. For information about how groups and subgroups work within *`Workfront`*, see [Groups overview](groups.md) and [Subgroups overview](subgroups.md).


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


## Add a subgroup {#add-a-subgroup}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  Click `Groups`.


   In the list of groups that displays, *`group administrators`* can see the groups they manage, as well as any subgroups of those groups. *`Adobe Workfront administrators`* can see all groups.

1.  Select the existing group or subgroup where you want to add a new subgroup.
1.  Click `New Subgroup`.
1.  In the `New Subgroup` box that appears, type a `Group Name` for the subgroup.
1.  (Optional) specify any of the following information:

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a description for the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span>. You can type up to 512 characters.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Make this group and subgroups public</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span> with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <p>Note:  
     <ul> 
      <li>You can’t make a subgroup public by itself, but you can make it’s top-level parent group public, which also makes all of the parent’s subgroups public.</li> 
      <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
     </ul> </p> <p>If you need information about the access needed to edit users, see <a href="grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Grant access to users</a>. For information about editing users, see <a href="edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Edit a user's profile</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Business Leader </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>You can assign one user as a Business Leader for a <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span> that you manage. A Business Leader is someone who makes business decisions for the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span>. <span>For more information, see </span><a href="business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a><span>.</span></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can also assign a Business Leader for a <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span> on the Groups page header and on the Group Details page.</p> <p>If the person is not already a member of the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span>, adding their name to this field also adds them to the group.</p> <p>Note:  
     <ul> 
      <li>Before you can remove the Business Leader from a <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span>, you must remove their name from the Business Leader field.</li> 
      <li>If you remove the name from the Business Leader field, that user remains a member of the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span> unless you remove them from it. For instructions on removing someone from a group, see the section <a href="manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Manage a group’s memberships</a> in the article <a href="manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Manage a group</a>.</li> 
     </ul> </p> <p>For more information, see <a href="business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group Members and Group Administrators</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <ul> 
     <li> <p>Group members: To add users and groups to the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span>, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> <p>The users and groups that you add have access to all objects shared with the group.</p> </li> 
     <li> <p><span class="mc-variable WFVariables.AdminGroupInitCapPlur variable varname">Group administrators</span>:<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.subgroups">
         A subgroup inherits the 
        <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> of the group above it, so specifying a user as a 
        <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> for a subgroup is optional.
       </MadCap:conditionalText> You can assign a group member as an administrator for the group using the drop-down menu to the right of the user’s name.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Search people and groups in the list</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> If you need to find a user or group already assigned to this <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">subgroup</span>, you can type their name here and select it when it appears.</td> 
  </tr> 
 </tbody> 
</table>


1. Click `Save.`


