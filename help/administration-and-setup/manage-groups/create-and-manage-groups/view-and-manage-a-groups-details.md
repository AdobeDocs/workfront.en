


# View and manage a group’s details {#view-and-manage-a-group-s-details}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


You can view and edit the Group Details page for a group or subgroup that you manage. This page includes a description of the group, the names of the Business Leader and *`group administrators`*, and an option that allows you to make the group and all of its subgroups public or private.


For information about other ways you can manage a group, see [Create a group](create-a-group.md).


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


## View and manage a group’s details {#view-and-manage-a-group-s-details-1}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  Click `Groups`.


   In the list of groups that displays, *`group administrators`* can see the groups they manage, as well as any subgroups of those groups. *`Adobe Workfront administrators`* can see all groups.

1. Click the name of the top-level group that you want to edit.
1.  In the left menu, click `Group Details`, then do any of the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>You can type up to 512 characters.</p> <p>If the field is blank, click <span class="bold">Add</span> to type a description.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group accessibility</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>(Available only if you are viewing Details for a group, not a subgroup.) Enable or disable the option <span class="bold">Make this group and subgroups private</span>.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Group stakeholders</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <ul> 
     <li><span class="bold">Group Administrators</span>: Add or remove users with a Planner license as <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> for the group. Begin typing the name of a user, then click the name when it appears in the drop-down menu.</li> 
     <li><span class="bold">Business Leader</span>: Do one of the following:
      <ul>
       <li>If you have not yet assigned a Business Leader for the group, click <span class="bold">Add</span>, start typing the name of the user you want to assign, then click the person’s name when it appears.</li>
       <li>If the group already has a Business Leader and you want to change it, double-click the name of the existing Business Leader. Delete the name, start typing the name of the user you want to assign, then click the person’s name when it appears.</li>
      </ul></li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="preview">Add custom form</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"><span class="preview">If your access level allows you to manage custom forms, add a custom form to the group. For more information, see </span><a href="_create-and-manage-custom-forms.md" class="preview MCXref xref xrefpreview">Custom forms</a><span class="preview">.</span> </td> 
  </tr> 
 </tbody> 
</table>




