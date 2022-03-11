---
filename: edit-list-controls-filters-views-groupings
user-type: administrator
product-area: system-administration;reporting
navigation-topic: configure-reports-administration
title: Edit list controls: filters, views, and groupings
description: As an Adobe Workfront administrator, you use the List Controls area to determine which filters, views, and groupings you want available in your Workfront instance and listed in all layout templates in the system.
---

# Edit list controls: filters, views, and groupings

As an Adobe Workfront administrator, you use the List Controls area to determine which filters, views, and groupings you want available in your Workfront instance and listed in all layout templates in the system.

In a layout template, you can then enable the filters, views, and groupings that you want available for the users who are assigned to that layout template. Users can see them as options in their drop-down menus above their lists of objects and reports.

For more information, see [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Add filters, views, and groupings

<ol data-mc-continue="false"> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Interface</span> > <span class="bold">List Controls</span>.<br></li> 
 <li value="3">Click <span class="bold">Edit List Controls</span>.</li> 
 <li value="4"> <p>In the <span class="bold">Object Type</span> drop-down <span class="bold-not-uitext">menu</span>, click the object <span class="bold-not-uitext">type for which you want to filters, views, and groupings</span>.</p> <p>Four columns display, containing the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Filters</td> 
     <td>A list of filters associated with the object type you selected. If the filter is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Views</td> 
     <td>A list of views&nbsp;associated with the object type you selected. If the view&nbsp;is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Groupings</td> 
     <td>list of groupings&nbsp;associated with the object type you selected. If the grouping&nbsp;is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Custom Tabs</td> 
     <td> <p>The tabs you see listed in this column can be found by&nbsp;all users in the system&nbsp;and they can add them to their own interface.&nbsp;</p> <note type="important"> 
       <p>Only custom tabs built before 2012 (prior to the Anaconda release) can be shared with all the users in the system using list controls. Any custom tabs built after that release need to be shared with users using the layout template functionality. For more information about layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.<br></p> 
       <p>Only the following object types allow for custom tabs to be added to list controls:</p> 
       <ul> 
        <li>Project</li> 
        <li>Task</li> 
        <li>Issue</li> 
       </ul> 
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>Click <span class="bold">Add Filter</span>,<span class="bold"> Add View</span>, or<span class="bold"> Grouping</span>.</p> <p>If you have custom tabs built before 2012 and the object is a project, a task or an issue, you can also click <span class="bold">Add Custom Tab</span> to add custom tabs to the list controls.</p> </li> 
 <li value="6"> <p>In the <span class="bold">Search Filters</span> box that displays, start typing the name of a filter, view, grouping, or custom tab, then click <span class="bold">Search</span>.</p> <p>Or</p> <p>Simply click <span class="bold">Search</span>, to list all existing filters, views, groupings, or custom tabs.&nbsp;</p> <p>You must have at least one custom tab built before 2012 in the system before you can see any results when searching for custom tabs.<br></p> </li> 
 <li value="7">Click the plus sign to the left of the name of a filter, view, grouping, or custom tab that you want to add in your list controls.</li> 
 <li value="8"> <p>Click <span class="bold">Save</span>.<br></p> <p>All the users in the system can find the filters, views, and groupings in their drop-down menus at the top of lists that display the selected object. In the case of custom tabs, they can now add the custom tabs in their interface, for the object specified.&nbsp;</p> </li> 
</ol>

## Remove filters, views, and groupings

You can remove filters, views, and groupings, including most of the default ones, from your Workfront instance.

>[!NOTE]
>
>At least one filter, one view, and one grouping must remain in your Workfront instance at all times. Without at least one, your lists and reports do not display. In order to assure that a Workfront administrator does not inadvertently delete all of the filters, views, or groupings, the following defaults can’t be removed: Standard view, All filter, and Nothing grouping.

<ol data-mc-continue="false"> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Interface</span> > <span class="bold">List Controls</span>.<br></li> 
 <li value="3">Click <span class="bold">Edit List Controls</span>.</li> 
 <li value="4"> <p>In the <span class="bold">Object Type</span> drop-down menu, click your object type.</p> <p>Four columns display, containing the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Filters</td> 
     <td>A list of filters associated with the object type you selected. If the filter is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Views</td> 
     <td>A list of views&nbsp;associated with the object type you selected. If the view&nbsp;is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Groupings</td> 
     <td>list of groupings&nbsp;associated with the object type you selected. If the grouping&nbsp;is displayed in the list, it shows for every user in the system, when they are viewing a list of objects of the type you selected.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Custom Tabs</td> 
     <td> <p>The tabs you see listed in this column can be found by&nbsp;all users in the system&nbsp;and they can add them to their own interface.&nbsp;</p> <note type="important"> 
       <p>Only custom tabs built before 2012 (prior to the Anaconda release) can be shared with all the users in the system using list controls. Any custom tabs built after that release need to be shared with users using the layout template functionality. For more information about layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.<br></p> 
       <p>Only the following object types allow for custom tabs to be added to list controls:</p> 
       <ul> 
        <li>Project</li> 
        <li>Task</li> 
        <li>Issue</li> 
       </ul> 
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>Click the trash can button to the left of a the name of a filter, view, grouping, or custom tab.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Save</span> to remove&nbsp;the filter, view, grouping, or custom tab from&nbsp;the list controls for the selected object.</p> </li> 
</ol>

