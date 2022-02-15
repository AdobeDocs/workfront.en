



# Manage group memberships in `the new Workfront experience` {#manage-group-memberships-in-the-new-workfront-experience}

The information on this page refers to functionality available only in the new Workfront experience beta. 


As a `Group Administrator`, you can view a list of members of any group you manage and add, remove, export, activate, and deactivate them. You can also change their roles in the group, edit their profiles, and send them Update comments.


`Workfront administrators` can also do these things (for any group).


For information about other ways you can manage a group, see [Create and manage groups](create-manage-groups.md).


To manage group memberships:



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. Click **Groups** ![](assets/groups-icon.png).

1.  In the left panel, click** Group Members**.
1.  On the **Group Members** tab, do any of the following to manage user memberships in your group:

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Add a user to the group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Click <b>Add Members</b> <img src="assets/add-icon-plus-in-circle.png">, start typing the user's name, then select it when it appears.</p> <p> <p>Repeat this for any other users you want to add. You can click the X to the right of a name if you decide not to add that user.</p> </p> <p>Click <b>Done</b> when you are finished.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Remove a user from the group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select one or more user name, click <b>Remove member</b> <img src="assets/remove-icon---x-in-circle.png">, then click <b>Remove</b> in the warning message that displays.</p> <p>Note:  
     <ul> 
      <li value="1">If this group is the Home Group for a user you want to remove, you must first assign another Home Group in the user's profile. For more information, see <a href="home-groups.md" class="MCXref xref">Home Groups</a> and <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</li> 
      <li value="2">If the group has only one <span class="WFVariablesAdminGroup">Group Administrator</span> and you need to remove him or her from the group, you need to assign another <span class="WFVariablesAdminGroup">Group Administrator</span> to the group first.</li> 
      <li value="3">A user can belong individually to a subgroup as well as to the parent group. When you remove someone from a subgroup, they remain part of the parent group. Similarly, when you remove them from the parent group, they will remain part of the subgroup. If you do not want a user to have the access allowed for the parent group, you must remove the user both from the subgroups as well as the parent group, if they are listed in both places individually.</li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Edit a user's profile information</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select one or more user name, click <b>Edit</b> <img src="assets/edit-ojbect-icon.png">, then change the user's profile information. For information about the changes you can make, see <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Export user membership data</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select one or more user name, click <b>Export</b> <img src="assets/export.png">, then export the data as a PDF, Excel, or tab delimited file. For more information about exporting data, see <a href="export-data.md" class="MCXref xref">Export data</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">View and edit members' roles in the group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The <b>Role</b> column lists each member's role. As a <span class="WFVariablesAdminGroup">Group Administrator</span>, you can double-click a member's role to change it.</p> <p>For members of the group who are not <span class="WFVariablesAdminGroup-plur">Group Administrators</span>, this column is not editable.</p> <p><span class="WFVariablesAdminGroup-plur">Group Administrators</span> are always at the top of the list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Send a comment to group members</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select one or more user name, click <b>Update</b> <img src="assets/comment-icon.png">, then type the comment.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Activate a user in <span class="WFVariablesProdNameWF">Workfront</span></td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select one or more inactive users, then click <b>Activate user</b>, to activate them in <span class="WFVariablesProdNameWF">Workfront</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Deactivate a user in <span class="WFVariablesProdNameWF">Workfront</span></td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select one or more active users, then click <b>Deactivate user</b> <img src="assets/deactivate-user.png">, to deactivate them in <span class="WFVariablesProdNameWF">Workfront</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">Sort by Role or Name column</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Click the heading of the <b>Group Role</b> or <b>Name</b> column to sort the list by that column.</td> 
  </tr> 
 </tbody> 
</table>




