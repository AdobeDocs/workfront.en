---
filename: view-and-manage-a-groups-memberships
user-type: administrator
product-area: system-administration;user-management
keywords: add,users,group,add,another,assign,administrator,remove,user,view,roles,members,export,membership,data
navigation-topic: create-and-manage-groups
---



# View and manage a group’s memberships {#view-and-manage-a-group-s-memberships}

As an *`Adobe Workfront administrator`*, you can view, add, remove, export, activate, and deactivate members of any group that you manage. You can also edit their profiles, add Updates to their profiles, and assign them as additional *`group administrators`* for the group.


If there are any groups above your group, their administrators can also do these things for your group. The same is true for *`Workfront administrators`* (for any group).


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


## View and manage a group’s memberships {#view-and-manage-a-group-s-memberships-1}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  In the left panel, click `Groups`.


   In the list that displays, *`Workfront administrators`* can see all groups and subgroups. *`Group administrators`* can see only the groups and subgroups they administer.

1. Click the name of the group that you want to edit.
1.  On the page that appears, with `Group Members` selected in the left menu, do any of the following:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Add a user to the group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <ol style="list-style-type: lower-alpha;"> 
     <li value="1">Click <span class="bold">Add Members </span><img src="assets/add-icon-plus-in-circle.png">, start typing the user's name, then select it when it appears.</li> 
     <li value="2"> <p>Repeat this for any other users you want to add.</p> <p>You can click the X to the right of a name if you decide not to add that user.</p> </li> 
     <li value="3">Click <span class="bold">Done</span> when you are finished.</li> 
    </ol> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Remove a user from the group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <ol style="list-style-type: lower-alpha;"> 
     <li value="1">Select one or more user name, then click <span class="bold">Remove member</span><img src="assets/remove-icon---x-in-circle.png">.</li> 
     <li value="2"> <p>Click <span class="bold">Remove</span> in the warning message that displays.</p> <p>You can find a user you want to remove from the list by clicking <span class="bold">Search people and groups in the list</span>, typing their name in the box, then clicking the name when it appears.</p> <p>Note:  
       <ul> 
        <li>If this group is the Home Group for a user you want to remove, you must first assign another Home Group in the user's profile. For more information, see <a href="home-groups.md" class="MCXref xref">Home Groups overview</a> and <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</li> 
        <li>If the group has only one <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> and you need to remove him or her from the group, you need to assign another <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> to the group first.</li> 
        <li>A user can belong individually to a subgroup as well as to the parent group. When you remove someone from a subgroup, they remain part of the parent group. Similarly, when you remove them from the parent group, they will remain part of the subgroup. If you do not want a user to have the access allowed for the parent group, you must remove the user both from the subgroups as well as the parent group, if they are listed in both places individually.</li> 
       </ul> </p> </li> 
    </ol> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Edit a user's profile information</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <ol style="list-style-type: lower-alpha;"> 
     <li value="1">Select one or more user name, then click <span class="bold">Edit </span><img src="assets/edit-icon.png">.</li> 
     <li value="2"> <p>Change the user's profile information.</p> <p>For information about the changes you can make, see <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Export user membership data</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <ol style="list-style-type: lower-alpha;"> 
     <li value="1">Select one or more user name, then click <span class="bold">Export </span><img src="assets/export.png">.</li> 
     <li value="2"> <p>Export the data as a PDF, Excel, or tab delimited file.</p> <p>For more information about exporting data, see <a href="export-data.md" class="MCXref xref">Export data</a>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">View and edit members' group roles</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The <span class="bold">Group Role</span> column lists each member's role. As a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span>, you can double-click a member's role to change it.</p> <p>For members of the group who are not <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span>, this column is not editable.</p> <p><span class="mc-variable WFVariables.AdminGroupInitCapPlur variable varname">Group administrators</span> are always at the top of the list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Send a comment to group members</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <ol style="list-style-type: lower-alpha;"> 
     <li value="1">Select one or more user name, then click <span class="bold">Update </span><img src="assets/comment-icon.png">.</li> 
     <li value="2">Type the comment.</li> 
    </ol> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Activate a user in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select one or more inactive users, then click <span class="bold">Activate user</span>, to activate them in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Deactivate a user in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select one or more active users, then click <span class="bold">Deactivate user</span><img src="assets/deactivate-user.png">, to deactivate them in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Sort by column</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Click the heading of a column to sort the list by the contents in that column.</td> 
  </tr> 
 </tbody> 
</table>




