---
filename: customize-fvg-list-controls-layout-template
title: Customize Filter, View, and Grouping list controls using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
---



# Customize Filters, Views, and Groupings using a layout template {#customize-filters-views-and-groupings-using-a-layout-template}

As an *`Adobe Workfront administrator`*, you can use a layout template to specify which list controls appear in the Filter, View, and Grouping drop-down menus. These menus appear above lists throughout *`Workfront`*, such as the list of tasks for a project:


![](assets/filter-view-grouping---layout-templates-350x98.png)




For more information about layout templates, see [Create and manage layout templates](create-and-manage-layout-templates.md).


For information about layout templates for groups, see [Create and modify a group’s layout templates](create-and-modify-a-groups-layout-templates.md).


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



## Customize Filter, View, and Grouping list controls: {#customize-filter-view-and-grouping-list-controls}




1. Begin working on a layout template, as described in [Create and manage layout templates](create-and-manage-layout-templates.md).
1.  Click the down arrow ![](assets/down-arrow-blue.png) under `Customize what users see`, then click `Lists` in the drop-down menu that displays.


   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding-350x180.png)



1.  Click the down arrow ![](assets/down-arrow-blue.png) under `Select a list to customize`, then select the type of *`Workfront`* object for which you want to customize the Filter, View, and Grouping list controls.


   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding-350x161.png)




   >[!NOTE]
   >
   >If you select Projects as the list to customize, then disable Projects I'm On or Projects I Own in the Filter section, users will no longer see or be able to use that filter:
   >
   >    
   >    
   >    *  In the list of filters that displays when they click the filter icon ![](assets/filter-nwepng.png) above a list:
   >    
   >    
   >      ![](assets/disable-filters-projects-im-on-or-own-350x249.png)   >    
   >    

   >    
   >    *  In the header on the Projects area header:
   >    
   >    
   >      ![](assets/disable-filter-pills-350x115.png)   >    
   >    

   >    
   >    
   >      For more information about these filters in the Projects area header, see the section [Project lists under a Portfolio](subtabs-removed.md#project) in the article [Subtabs replaced by new main areas or filters in the new Adobe Workfront experience](subtabs-removed.md).
   >    
   >    
   >    




1.  (Optional) If you want to change the default filter, view, or grouping for the layout template, hover over the filter, view, or grouping, then click `Set as default`.


   The defaults you choose determine which Filter, View, and Grouping users will see in lists throughout *`Workfront`* when the layout template is assigned to them. If you don’t change these defaults, users see all lists as follows:

    
    
    * `Filters`: All
    * `View`: Standard (where applicable; some lists do not have this view)
    *  `Grouping`: Nothing
    
    
   You can hide the options All, Standard, and Nothing after selecting different defaults (see Step 5), but they can’t be deleted.


   You can delete any other option being used as a default, but you have to select a different default first.


   For information about deleting filters, views, and groupings, see [Create, edit, and share default filters, views, and groupings](create-and-share-default-fvgs.md).

1.  Hide and add list controls as follows:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 227px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Hide a list control</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Clear or check the box next to the list control you want to hide or show.</p> <p>If a checkbox is dimmed, you cannot hide that list control. The Default <img src="assets/default-pill.png"> setting for each list control is dimmed because you can’t hide the setting that is currently configured as the default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Add a custom list control</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p> 
     <ol> 
      <li value="1"> Click <span class="bold">Add Filter</span>, <span class="bold">Add View</span>, or <span class="bold">Add Grouping</span> at the bottom of the Filter, View, or Grouping list. In the box that displays, start typing the name of an existing custom list control previously created for your organization, then click the name when it appears.</li> 
      <li value="2"> If you want the new custom list control set as the default filter, view, or grouping for the layout template, click <span class="bold">Set as Default</span>. </li> 
      <li value="3"> <p>Click <span class="bold">Add</span> when you are finished.</p> <p>Note:  <p>Users can add custom list controls to their own lists. If you add custom list controls in a layout template, your list controls are added and theirs move to the bottom of the panel; yours do not replace theirs.</p> <p>This is also true if you assign the user to a new layout template that has custom list controls. </p> <p>For information about customizing list controls, see <a href="filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>, <a href="views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>, and <a href="groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p> </p> </li> 
     </ol> </p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Continue customizing the layout template.


   Or


   If you are finished customizing, click `Save`.


   >[!TIP] {type="tip"}
   >
   >You can `Save` your progress at any time, then continue to modify the template later.






