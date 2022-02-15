---
filename: create-and-manage-layout-templates
title: Layout Templates overview
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
---



# Create and manage layout templates {#create-and-manage-layout-templates}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

As a *`Workfront administrator`* or a *`group administrator`*, you can create and modify layout templates to customize the following layout elements in *`Workfront`* for your users: 



* Main Menu ![](assets/main-menu-icon.png)

* Left navigation panel
* Home area 
* Views, filters, and groupings people use with lists and reports.
* On-screen terminology


After you create or modify a layout template, you can assign it to individual users, teams, groups, or job roles.


Every user's default *`Workfront`* layout depends on their access level and license type. For example, some users might not see some areas in the Main Menu. For more information, see [About the default Adobe Workfront layout](about-the default-wf-layout.md).


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Considerations for creating and managing layout templates {#considerations-for-creating-and-managing-layout-templates}




* Users can customize a few areas of their own layout. When you change a layout template, your changes merge with any customizations they have made, without overwriting or resetting them. This is also true if you assign users to a new layout template.
*  Your older layout templates created in *`Adobe Workfront Classic`* have been automatically available in your instance of *`the new Adobe Workfront experience`* since they were migrated in early Fall 2019. Layout templates created in *`Adobe Workfront Classic`* after that time were migrated in April 2020. We recommend that you update these layout templates in *`the new Adobe Workfront experience`* to take advantage of new functionality and to make them even more useful in that environment.


  If you created a layout template recently in *`Workfront`* Classic and want it available for your users in *`the new Adobe Workfront experience`*, you can migrate it there. For instructions, see [Migrate your layout templates to the new Adobe Workfront experience](migrate-layout-templates-to-nwe.md).


  Keep in mind that the migrated version and the original version of each layout template are separate because they serve two different environments, so if you edit one version, your changes don't affect the other version.

* *`Group administrators`* and users with a Plan license who can edit other users can add system-level and group-level layout templates to the users they can manage when editing their profile.
* *`Group administrators`* cannot assign layout templates to job roles or teams.


For more information about layout templates, see [Layout templates](_use-layout-templates-customize-ui.md).


## Create or modify a layout template {#create-or-modify-a-layout-template}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Interface` > `Layout Templates`.

1.  Click `New Layout Template`.


   Or


   Click the name of the layout template you want to modify.

1. If you are creating a new layout template, type a `Layout template name` and (optional) a `Description` for it.

1.  Customize areas of the user interface, as described in the following articles:

    
    
    * [Customize the Main Menu using a layout template](customize-main-menu.md) 
    * [Customize the left panel using a layout template](customize-left-panel.md) 
    * [Customize pinned pages using a layout template](customize-pinned-pages.md) 
    * [Customize the Details view using a layout template](customize-details-view-layout-template.md) 
    * [Customize Home and Summary using a layout template](customize-home-summary-layout-template.md) 
    * [Customize the landing page using a layout template](customize-landing-page.md) 
    * [Customize Filters, Views, and Groupings using a layout template](customize-fvg-list-controls-layout-template.md) 
    * [Customize user interface terminology using a layout template](customize-terminology.md) 
    
    

1.  Continue on to test your layout template and make it available to users, as described in the articles below:

    
    
    * [Testing a new layout template](test-a-layout-template.md) 
    * [Grant administrative access for a layout template](grant-admin-access-layout-template.md) 
    * [Assign users to a layout template](assign-users-to-layout-template.md) 
    
    



You can also create a new layout template by copying it and changing the copy. For more information, see [Copy a layout template](copy-a-layout-template.md).
