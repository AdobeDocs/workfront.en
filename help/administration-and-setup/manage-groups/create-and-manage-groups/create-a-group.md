---
filename: create-a-group
user-type: administrator
product-area: system-administration;user-management
keywords: create,group,subgroup,new
navigation-topic: create-and-manage-groups
---



# Create a group {#create-a-group}

As an *`Adobe Workfront administrator`*, you can create groups to organize users and projects and to assign access rights within *`Workfront`*. For more information, see [Groups overview](groups.md).


Every subgroup needs at least one *`group administrator`*. *`Group administrators`* can use the Groups page to manage their groups in one place.


If you are a *`group administrator`* or a *`Workfront administrator`*, you can also create subgroups under a group. For instructions, see [Create a subgroup](create-a-subgroup.md). 


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


## Create a top-level group from scratch {#create-a-top-level-group-from-scratch}

These steps explain how to create a new group from scratch. For information about creating a group or subgroup by copying an existing one, see [Create a top-level group by copying an existing group or subgroup](#copying-an-existing-group-and-sub-group) in this article.


You must be a *`Workfront administrator`* to create a top-level group.



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups` ![](assets/groups-icon.png).

1.  Above the list of groups, click `New Group`.


   >[!TIP] {type="tip"}
   >
   >At the bottom of the list of groups, you can also click `Add More Groups`to add a group in-line, then click `Enter`when you are finished adding the group information.



1.  In the `New Group` box that displays, type a name for the group.
1.  Specify the following information:

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a description for the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>. You can type up to 512 characters.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Make this group and subgroups public</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span> with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <p>Note:  
     <ul> 
      <li>You can’t make a subgroup public by itself, but you can make it’s top-level parent group public, which also makes all of the parent’s subgroups public.</li> 
      <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
     </ul> </p> <p>If you need information about the access needed to edit users, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>. For information about editing users, see <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Business Leader </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>You can assign one user as a Business Leader for a <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span> that you manage. A Business Leader is someone who makes business decisions for the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>. <span>For more information, see </span><a href="business-leader-overview.md" class="MCXref xref">Business Leader overview</a><span>.</span></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can also assign a Business Leader for a <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span> on the Groups page header and on the Group Details page.</p> <p>If the person is not already a member of the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>, adding their name to this field also adds them to the group.</p> <p>Note:  
     <ul> 
      <li>Before you can remove the Business Leader from a <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>, you must remove their name from the Business Leader field.</li> 
      <li>If you remove the name from the Business Leader field, that user remains a member of the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span> unless you remove them from it. For instructions on removing someone from a group, see the section <a href="manage-a-group.md#manage" class="MCXref xref">Manage a group’s memberships</a> in the article <a href="manage-a-group.md" class="MCXref xref">Manage a group</a>.</li> 
     </ul> </p> <p>For more information, see <a href="business-leader-overview.md" class="MCXref xref">Business Leader overview</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group Members and Group Administrators</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <ul> 
     <li> <p>Group members: To add users and groups to the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> <p>The users and groups that you add have access to all objects shared with the group.</p> </li> 
     <li> <p><span class="mc-variable WFVariables.AdminGroupInitCapPlur variable varname">Group administrators</span>: You can assign a group member as an administrator for the group using the drop-down menu to the right of the user’s name.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">A top-level group must have at least 1 <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Search people and groups in the list</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> If you need to find a user or group already assigned to this <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>, you can type their name here and select it when it appears.</td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Create Group`.




## Create a top-level group by copying an existing group or subgroup {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

As a *`Workfront administrator`*, you can create a new top-level group by copying an existing group or subgroup.


Keep the following in mind when you want to do this:



* All of the members and any subgroups belonging to the existing group are copied to the new top-level group.
* The members of the copied group retain the assignments they had in the original group. Therefore, the *`group administrators`* of the original group are also designated as the *`group administrators`* in the copied group.



To create a new top-level group by copying a group or subgroup:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  In the left panel, click `Groups` ![](assets/groups-icon.png).


   In the list of groups that displays, *`group administrators`* can see the groups they manage, as well as any subgroups of those groups. *`Adobe Workfront administrators`* can see all groups.  


1. Select the group you want to copy, then click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> the Copy icon  <img src="assets/copy-icon.png"></MadCap:conditionalText>`.
1. In the `Copy Group` box that appears, type a `Group Name` for the copied group.  

1.  Specify the following information:

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a description for the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>. You can type up to 512 characters.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Make this group and subgroups public</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span> with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <p>Note:  
     <ul> 
      <li>You can’t make a subgroup public by itself, but you can make it’s top-level parent group public, which also makes all of the parent’s subgroups public.</li> 
      <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
     </ul> </p> <p>If you need information about the access needed to edit users, see <a href="grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Grant access to users</a>. For information about editing users, see <a href="edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Edit a user's profile</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Business Leader </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>You can assign one user as a Business Leader for a <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span> that you manage. A Business Leader is someone who makes business decisions for the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>. <span>For more information, see </span><a href="business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a><span>.</span></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can also assign a Business Leader for a <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span> on the Groups page header and on the Group Details page.</p> <p>If the person is not already a member of the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>, adding their name to this field also adds them to the group.</p> <p>Note:  
     <ul> 
      <li>Before you can remove the Business Leader from a <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>, you must remove their name from the Business Leader field.</li> 
      <li>If you remove the name from the Business Leader field, that user remains a member of the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span> unless you remove them from it. For instructions on removing someone from a group, see the section <a href="manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Manage a group’s memberships</a> in the article <a href="manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Manage a group</a>.</li> 
     </ul> </p> <p>For more information, see <a href="business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group Members and Group Administrators</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <ul> 
     <li> <p>Group members: To add users and groups to the <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> <p>The users and groups that you add have access to all objects shared with the group.</p> </li> 
     <li> <p><span class="mc-variable WFVariables.AdminGroupInitCapPlur variable varname">Group administrators</span>:<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.copied groups">
         Any 
        <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> of the original group are also designated as the 
        <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> in the copied group.
       </MadCap:conditionalText> You can assign a group member as an administrator for the group using the drop-down menu to the right of the user’s name.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">A top-level group must have at least 1 <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Search people and groups in the list</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> If you need to find a user or group already assigned to this <span class="mc-variable snippet-variables-wf-groups.group-subgroup-copiedgroup variable varname">group</span>, you can type their name here and select it when it appears.</td> 
  </tr> 
 </tbody> 
</table>



   >[!NOTE]
   >
   >
   >    
   >    
   >    * If the original group has subgroups, the subgroups are added to the new group, and their names are, by default, "The original subgroup name (Copy)".
   >    * You can eliminate any user or subgroup from the original group by clicking the X to the right of the user’s or subgroup’s name.
   >    
   >    




1.  Click `Create Group`.




##  

