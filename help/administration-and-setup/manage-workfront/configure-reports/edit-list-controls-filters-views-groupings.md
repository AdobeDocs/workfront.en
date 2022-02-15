---
filename: edit-list-controls-filters-views-groupings
user-type: administrator
product-area: system-administration;reporting
navigation-topic: configure-reports-administration
---



# Edit list controls: filters, views, and groupings {#edit-list-controls-filters-views-and-groupings}

As an *`Adobe Workfront administrator`*, you use the List Controls area to determine which filters, views, and groupings you want available in your *`Workfront`* instance and listed in all layout templates in the system.


In a layout template, you can then enable the filters, views, and groupings that you want available for the users who are assigned to that layout template. Users can see them as options in their drop-down menus above their lists of objects and reports.


For more information, see [Reporting elements: filters, views, and groupings](reporting-elements-filters-views-groupings.md).


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



## Add filters, views, and groupings {#add-filters-views-and-groupings}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Interface` > `List Controls`.  

1. Click `Edit List Controls`.
1.  In the `Object Type` drop-down `menu`, click the object `type for which you want to filters, views, and groupings`.


   Four columns display, containing the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Filters</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">A list of filters associated with the object type you selected. If the filter is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Views</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">A list of views&nbsp;associated with the object type you selected. If the view&nbsp;is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Groupings</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">list of groupings&nbsp;associated with the object type you selected. If the grouping&nbsp;is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Custom Tabs</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>The tabs you see listed in this column can be found by&nbsp;all users in the system&nbsp;and they can add them to their own interface.&nbsp;</p> <p>Important:  <p>Only custom tabs built before 2012 (prior to the Anaconda release) can be shared with all the users in the system using list controls. Any custom tabs built after that release need to be shared with users using the layout template functionality. For more information about layout templates, see <a href="create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.<br></p> <p>Only the following object types allow for custom tabs to be added to list controls:</p> 
     <ul> 
      <li>Project</li> 
      <li>Task</li> 
      <li>Issue</li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Add Filter`, `Add View`, or `Grouping`.


   If you have custom tabs built before 2012 and the object is a project, a task or an issue, you can also click `Add Custom Tab` to add custom tabs to the list controls.

1.  In the `Search Filters` box that displays, start typing the name of a filter, view, grouping, or custom tab, then click `Search`.


   Or


   Simply click `Search`, to list all existing filters, views, groupings, or custom tabs.&nbsp;


   You must have at least one custom tab built before 2012 in the system before you can see any results when searching for custom tabs.  


1. Click the plus sign to the left of the name of a filter, view, grouping, or custom tab that you want to add in your list controls.
1.  Click `Save`.  



   All the users in the system can find the filters, views, and groupings in their drop-down menus at the top of lists that display the selected object. In the case of custom tabs, they can now add the custom tabs in their interface, for the object specified.&nbsp;





## Remove filters, views, and groupings {#remove-filters-views-and-groupings}

You can remove filters, views, and groupings, including most of the default ones, from your *`Workfront`* instance.


>[!NOTE]
>
>At least one filter, one view, and one grouping must remain in your *`Workfront`* instance at all times. Without at least one, your lists and reports do not display. In order to assure that a *`Workfront administrator`* does not inadvertently delete all of the filters, views, or groupings, the following defaults can’t be removed: Standard view, All filter, and Nothing grouping.





1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Interface` > `List Controls`.  

1. Click `Edit List Controls`.
1.  In the `Object Type` drop-down menu, click your object type.


   Four columns display, containing the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Filters</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">A list of filters associated with the object type you selected. If the filter is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Views</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">A list of views&nbsp;associated with the object type you selected. If the view&nbsp;is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Groupings</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">list of groupings&nbsp;associated with the object type you selected. If the grouping&nbsp;is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Custom Tabs</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>The tabs you see listed in this column can be found by&nbsp;all users in the system&nbsp;and they can add them to their own interface.&nbsp;</p> <p>Important:  <p>Only custom tabs built before 2012 (prior to the Anaconda release) can be shared with all the users in the system using list controls. Any custom tabs built after that release need to be shared with users using the layout template functionality. For more information about layout templates, see <a href="create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.<br></p> <p>Only the following object types allow for custom tabs to be added to list controls:</p> 
     <ul> 
      <li>Project</li> 
      <li>Task</li> 
      <li>Issue</li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click the trash can button to the left of a the name of a filter, view, grouping, or custom tab.
1.  Click `Save` to remove&nbsp;the filter, view, grouping, or custom tab from&nbsp;the list controls for the selected object.


