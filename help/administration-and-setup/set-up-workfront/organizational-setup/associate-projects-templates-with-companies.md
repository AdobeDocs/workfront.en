---
filename: associate-projects-templates-with-companies
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
---



# Associate projects and templates with companies {#associate-projects-and-templates-with-companies}

A project or a template cannot be associated with more than one company. But there is no limit to how many projects or templates you associate with one company.  



One of the benefits of associating projects with companies is that you can report on project financials for each company.


## Access requirements {#access-requirements}

You must have the following in order to manage companies in *`Workfront`*:

<table class="TableStyle-TableStyle-List-options-in-steps" style="margin-left: 0;margin-right: auto;caption-side: bottom;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" data-mc-conditions=""> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" data-mc-conditions=""> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Workfront plan*</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span class="mc-variable WFVariables.WFPlan-Team variable varname">Team</span> or higher</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="bold">Access level*</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>In order to manage companies, you must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level, which allows you to edit any company in the system. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p>Administrative access to manage companies, which allows you to edit any company in the system. For more information, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </li> 
    </ul> <p>Note: You can also manage companies associated with any group where you are assigned as a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span>.</p> 
    <div data-mc-conditions="SnippetConditions.HIDE"> 
     <p>In order to add to and remove users from the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> system, you must have one of the following:</p> 
     <ul> 
      <li> <p>The System Administrator access level. For information about this access level, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
      <li> <p>In your access level, Edit must be selected for the Users setting. And, for the Users setting, under Fine-tune your settings <img src="assets/gear-icon-in-access-levels.png"> , the Create option and at least one of the two User Admin options must be enabled. </p> <p>If you are using the User Admin (Group Users) option, you must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of a group where the user is a member.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>For information about the Users setting in an access level, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your *`Workfront administrator`*.


## Associate a template with a company  {#associate-a-template-with-a-company}

We recommend that you associate your project templates with your companies, so you can have designated templates that are specific for each company's projects. For more information about creating projects using a template, see [Create a project using a template](create-project-from-template.md).



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Templates`. ![](assets/templates-icon-in-main-menu.png)


1. Select the template you want to associate with a company, then click `Edit`.
1. In the `Overview` section of the `Edit Template` form, select a `Company` in the drop-down menu.

1. Click `Save Changes`.




## Associate a project with a company  {#associate-a-project-with-a-company}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Projects`. ![](assets/projects-in-main-menu.png)


1. Select the project you want to associate with a company, then click `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> the Edit icon. <img src="assets/edit-icon.png"></MadCap:conditionalText>`
1. In the `Overview` section of the `Edit Project` box, select a `Company` in the drop-down menu.

1. Click `Save Changes`.


