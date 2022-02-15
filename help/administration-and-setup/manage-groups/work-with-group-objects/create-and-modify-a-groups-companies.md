---
filename: create-and-modify-a-groups-companies
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
---



# Create and modify a group’s companies {#create-and-modify-a-group-s-companies}

When you are viewing a group that you manage in the Groups area, you can view and work with companies associated with the group and any of its subgroups.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the group or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref" data-mc-variable-override="">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *`Workfront administrator`*.


## View, work with, and create companies for your group from the Groups area {#view-work-with-and-create-companies-for-your-group-from-the-groups-area}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups` ![](assets/groups-icon.png).

1. Click the name of the group for which you want to create or modify *`companies`*.
1. In the left panel, click `Companies ![](assets/companies-icon-left-panel-group-pg.png)

   ` to list the companies associated with the group and any subgroups it may have.
1.  (Optional) To add a company, click `Add Company`, then configure the company using the options listed below. When you are finished, click `Create Company`.

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col style="width: 90px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Basic Info section</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
     <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
     <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
     <tbody> 
      <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Company Name</td> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a name for the company.</td> 
      </tr> 
      <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Is Active</td> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> When this option is enabled, users can find the <span class="mc-variable Snippet_Variables.Object variable varname">company</span> and attach it to projects that they create and edit. An inactive <span class="mc-variable Snippet_Variables.Object variable varname">company</span> cannot be attached to projects. </p> <p>This option is enabled by default.</p> </td> 
      </tr> 
      <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">This is the Primary Company</td> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Assigns the company as your organization's primary company. The primary company typically represents your <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account where most of your users work.</p> <p>By modifying their access levels, you can restrict users to see other users:</p> 
        <ul> 
         <li>Only in their primary company</li> 
         <li> <p>In their associated company and the primary company<br></p> <p>For information about the primary company functionality within users' access levels, see <a href="create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> <p>You can have only one or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a></p> </li> 
        </ul> </td> 
      </tr> 
      <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group</td> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p data-mc-conditions="SnippetConditions-wf-groups.groups">The system fills in the <span class="bold">Group </span>field for the new company with the group you are viewing.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">If you have administrative access to companies in your access level, you can remove the group from the company and assign a different one, or leave the company without a group.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">If you don’t have administrative access to companies, the <span class="bold">Group </span>field is required and you can select only the groups you manage or any subgroups under those groups.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">For information about administrative access to companies, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Grant users administrative access to certain areas</a>.</p> </td> 
      </tr> 
      <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Company Members</td> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.<br></p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Billing Rates section</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>You can override billing rates associated with your job roles at the company level. For information about creating job roles and associating them with billing rates, see <a href="create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">Create and manage job roles</a>.</p> <p>For more information about overriding billing rates at the company level, see <a href="override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">Override job role billing rates at the company level</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Custom Forms section</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>If there are fields that you want to add to your company that are not available in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, you can build a Custom Form and associate it with your company. You can attach this form to your company by selecting it from the drop-down menu. Only active companies are listed in the drop-down menu. For information about creating Custom Forms, see <a href="create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Create or edit a custom form</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>



   >[!TIP] {type="tip"}
   >
   >If you have administrative access to companies in your access level, you can also click Add More Companies at the bottom of the list. This adds a row where you can quickly configure the new company. 



1.  (Optional) To edit or delete companies, select at least one company, then use the toolbar buttons to edit ![](assets/edit-icon.png) or delete ![](assets/delete.png) it.


   For information about editing a company, see the section [Create or edit a company in Workfront](create-and-edit-companies.md#adding-a-company-to-workfront) in the article [Create and edit companies](create-and-edit-companies.md).

1. (Optional) To export the list of companies, click `Export`, then select the file format you want for the exported list.


