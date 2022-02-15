



# Create, view, and manage subgroups in `the new Workfront experience` {#create-view-and-manage-subgroups-in-the-new-workfront-experience}

The information on this page refers to functionality available only in the new Workfront experience beta. 


As a `Group Administrator`, you can create, view, edit, copy, export, and delete the subgroups in a group that you manage. For more information, see [Subgroups](subgroups.md).


For information about other ways you can manage a group, see [Create and manage groups](create-manage-groups.md).





1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. Click **Groups** ![](assets/groups-icon.png).

1.  Click the name of the group containing the subgroups you want to create, view, or manage.


   You can create up to 14 levels of subgroups under 1 group. On any one of these levels, you can create an unlimited number of parallel subgroups.

1. Click **Subgroups** to list the subgroups in the parent group you selected.
1.  Do any of the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 353px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Create a new subgroup</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Click <b>New Subgroup</b>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Edit a subgroup</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select a subgroup, then click <b>Edit</b>. In the box that displays, you can edit the group name and description and add and remove members.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Export a subgroup</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">To export the list of subgroups, click <b>Export</b>, then select the file format you want.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Copy a subgroup</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select a subgroup, then click <b>More &gt; Copy</b> to create a new group based on the selected group. In the <b>Copy Group box</b> that appears, do any of the following:</p> 
    <ul> 
     <li value="1">Specify information about the new group.</li> 
     <li value="2"> <p>Add any users or groups to the new group.</p> <p>These will have access to all objects shared with the parent group.</p> </li> 
     <li value="3">Make the new group private or public. For more information, see <a href="view-edit-details-group-subgroup.md" class="MCXref xref">View and edit Details for a group or subgroup in the new Workfront experience</a>.</li> 
     <li value="4">Assign one or more <span class="WFVariablesAdminGroup-plur">Group Administrators</span> to the new group. For more information, see <a href="group-administrators.md" class="MCXref xref">Group Administrators</a>.</li> 
    </ul> <p>For more information, see <a href="#about" class="MCXref xref">About copying a subgroup</a> in this article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">Delete a subgroup</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Select a subgroup, then click <b>More &gt; Delete</b>. In the <b>Delete Group</b> box that appears, use the drop-down list to select the group where you want to move the members of the group you are deleting. Objects (such as projects) that were assigned to the group you are deleting are reassigned to this group.</td> 
  </tr> 
 </tbody> 
</table>






## About copying a subgroup {#about-copying-a-subgroup}

Consider the following when you copy a subgroup:



* When you copy a subgroup, it becomes a parent group.
* When you copy a parent group, all group members and subgroups are copied with it.
*  If a subgroup you copy has its own subgroups, they are included in the copy and their names are formatted as follows:


  *Original subgroup name* (Copy)  


* Any subgroup that belongs to a public group is also public, so any user with edit-user access, in or out of the group, can add users to the subgroup.  



