---
filename: create-and-edit-companies
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
---



# Create and edit companies {#create-and-edit-companies}

A company is an organizational unit in *`Adobe Workfront`* that can represent your organization, a department within the organization, or a client you work with. You can add companies to *`Workfront`* and use them for financial planning, reporting purposes, to define permissions around objects, and to keep information confidential.


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


## Benefits of adding users to a company {#benefits-of-adding-users-to-a-company}




* You can build a company's organization chart by associating users with direct reports. Only users from the same company can be added as direct reports of another user from that company.
* As a project manager, you can identify available resources within the same company.
* You can keep information private between companies by choosing one or all of the following settings:
*  `<li> <p>Users from the same company can see each others’ requests.</p> <p>For more information about how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can give similar access to requests based on users' company, see the section <a href="set-task-issue-preferences.md#changing-task-and-issue-preferences" class="MCXref xref">Configure task and issues preferences for everyone in Workfront</a> in the article <a href="set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p> <p>For more information about how a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> can give similar access to requests based on users' company, see <a href="configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p> </li>` `<li>Users can see only request queues that are associated with their companies. For more information about restricting visibility of a request queue, see <a href="provide-access-to-request-queues.md" class="MCXref xref">Provide access to request queues</a>.</li>` `<li>You can restrict users to only see users in their company or their company and the primary company. For information about the primary company functionality regarding user privacy, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>` `<li>Users can restrict updates they make on items to be visible by their company users only. For more information about making an update private to a company, see <a href="update-work.md" class="MCXref xref">Update work</a>.</li>` 





## Create or edit a company in *`Workfront`* {#create-or-edit-a-company-in-workfront}

There is no limit to the number of companies you can add. However, we recommend that you use a limited amount of companies, because there are permissions implications linked to companies: too much fragmentation might interfere with users' visibility to work items.


By default, the company associated with your instance of *`Workfront`* is already created in your *`Workfront`* system and is the primary company. Your company has the same name as your customer name. For more information about your customer information in *`Workfront`*, see [Configure basic information for your system](configure-basic-info.md).


To add or edit a company:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  Click `Companies`.
1.   If you are adding a company, click `New Company`.


   Or


   If you are editing an existing company, select the company, then click `Edit`.

1.  Use the options that display to configure the following information:

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
         <li> <p>In their associated company and the primary company<br></p> <p>For information about the primary company functionality within users' access levels, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p>You can have only one or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a></p> </li> 
        </ul> </td> 
      </tr> 
      <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group</td> 
       <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">If there is a group that conducts business with the company, you can add the name of the group here. This is useful for <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> who need to report on and manage all the companies that their groups do business with.</p> <p>Important: If you don’t associate the group that will be working with this company, administrators for the group can’t access unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <span class="bold">Enter</span> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> for the group gain Manage access to the company. For more information, see <a href="#access" class="MCXref xref">Group administrators and companies</a> in this article.</p> </td> 
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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>You can override billing rates associated with your job roles at the company level. For information about creating job roles and associating them with billing rates, see <a href="create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>For more information about overriding billing rates at the company level, see <a href="override-job-role-billing-rates-company-level.md" class="MCXref xref">Override job role billing rates at the company level</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Custom Forms section</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>If there are fields that you want to add to your company that are not available in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, you can build a Custom Form and associate it with your company. You can attach this form to your company by selecting it from the drop-down menu. Only active companies are listed in the drop-down menu. For information about creating Custom Forms, see <a href="create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


1.  If you are creating a new company, click `Create Company`.


   Or


   If you are editing an existing company, click `Save Changes`.





## About sharing objects with companies {#about-sharing-objects-with-companies}

Certain permissions are available to users who are associated with a company, as explained in the section [Benefits of adding users to a company](#benefits) in the article [Create and edit companies](#). In addition to these permissions, you can allow users permissions to view, contribute, or edit objects in *`Workfront`* by sharing the object with their company. 


Rather than sharing an object with one individual user at a time, you can share it with their entire company. Each user in the company has the same permissions on that object.


For more information about sharing objects, see [Overview of sharing permissions on objects in Adobe Workfront](sharing-permissions-on-objects-overview.md).


## *`Group administrators`* and companies {#group-administrators-and-companies}

When a *`Workfront administrator`* assigns a group to a company, the *`group administrators`* for the group gain Manage access to the company in Setup. This includes access to the Companies page in Setup, where they can see and manage the company associated with their group.


With this access to the Companies page, a *`group administrator`* can assign a group to a company, but it must be a company that the *`group administrator`* created. If the *`group administrator`*‘s access level is not configured with administrative access to companies, the Group field is required when the *`group administrator`* creates the company—it’s bolded title indicates this:


![](assets/manage-company-group-field-req-350x273.jpg)




For information about how users gain administrative access to companies in their access level, see [Grant users administrative access to certain areas](grant-users-admin-access-certain-areas.md).


For information about managing a company in the Setup area, see [Create or edit a company in Workfront](#adding-a-company-to-workfront) in this article.
