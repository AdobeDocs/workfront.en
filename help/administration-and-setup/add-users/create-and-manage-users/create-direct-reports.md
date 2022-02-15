---
filename: create-direct-reports
title: Create direct reports
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
---



# Create direct reports {#create-direct-reports}

You can designate users as direct reports to another user. This allows you to create an organization chart that displays the management structure of your organization. For more information, see [View the organizational chart](view-the-org-chart.md).


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. For information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings </b><img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if User <b>Admin (Group Users)</b> is enabled, you must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of a group where the user is a member.</p> <p>For more information about the <b>Users</b> setting in an access level, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Create direct reports {#create-direct-reports-1}




1. Begin editing a user as described in [Edit a user's profile](edit-a-users-profile.md).
1.  In the `Organization` section, ensure that a company is selected in the `Company` field. 


   This field cannot be blank.

1. In the `Direct Reports` field, specify any users who report to the user you are editing.  

1. (Optional) In the `Reports To` field, specify the name of the user who this user reports to.
1. Click `Save Changes`.


