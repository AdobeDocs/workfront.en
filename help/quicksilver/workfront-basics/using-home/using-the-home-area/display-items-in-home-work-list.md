---
product-area: projects
navigation-topic: use-the-home-area
title: Display items in the [!UICONTROL Work List] in the Home area
description: The [!UICONTROL Work List] in the [!UICONTROL Home] area displays all work items that are assigned to you. You can control which items display in your [!UICONTROL Work List], by using filters and by grouping and sorting your work items.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
---
# Display items in the [!UICONTROL Work List] in the [!UICONTROL Home] area

<!-- Audited: 1/2024 -->


The [!UICONTROL Work List] in the [!UICONTROL Home] area displays all work items that are assigned to you. You can control which items display in your [!UICONTROL Work List], by using filters and by grouping and sorting your work items.

## Access requirements

 +++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license</strong></td> 
   <td> <p>New:</p><ul><li>[!UICONTROL Contributor] for approvals only</li> <li>[!UICONTROL Standard] or higher for all other objects</li> <p>Or</p> 
  </ul><p>Current:</p><ul><li>[!UICONTROL Review] for approvals only</li> <li>[!UICONTROL Work] or higher for all other objects</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>[!UICONTROL View] or higher access to Projects, Tasks, Issues, and Documents</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>Contribute permissions or higher to the tasks and issues you need to work on</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filter your work

You can filter items in the [!UICONTROL Work List] to see only specific types of items. For example, you can filter the [!UICONTROL Work List] to display only issues or requests.

>[!NOTE]
>
>The filter options are stored in the browser. If you consistently use the same browser on the same computer (and do not clear the site data) the selected filters do not change. If you switch browsers or computers then the filters revert to the default option, which is with all filters deselected.

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Home]**.
1. Click the **[!UICONTROL Filter]** ![](assets/filter-nwepng.png) drop-down menu. If you have any filters selected, the number of selected filters shows in place of the icon.
1. Select from the following filter options to specify the type of items you want to display:


   >[!TIP]
   >
   >* Filter options are based on objects (Tasks, Issues, Approvals, Personal tasks).
   >* Tasks and issues are further filtered by their state in relationship with our readiness to work on them ([!UICONTROL Working On], [!UICONTROL Ready to Start], [!UICONTROL Not Ready] for tasks, and [!UICONTROL Working On] and [!UICONTROL Requested] for issues). You can select to display tasks or issues in a specific state or click Tasks or Issues to select and display all states.
   >* There is a separate filter for completed items and it includes both tasks and issues. This does not include approvals. The [!UICONTROL Completed] filter includes Personal tasks.
   >* You can select to display only one state at a time. For example, you can display only [!UICONTROL Working On] tasks and only [!UICONTROL Requested] issues. You can also select multiple states at a time.
   >* You cannot apply filters for items assigned to one of your teams, and team assignments are not included in the items that are assigned directly to you.


1. (Optional) Further organize the [!UICONTROL Work List], as described in the section [Group and sort by Date, Project, and Priority](#group-and-sort-by-date-project-and-priority) in this article.

## Group and sort by [!UICONTROL Date], [!UICONTROL Project], and [!UICONTROL Priority] 

You can group and sort the [!UICONTROL Work List] by [!UICONTROL Planned Completion Date], [!UICONTROL Commit Date], [!UICONTROL Project], or [!UICONTROL My Priority]. The option you choose determines how items are grouped in the [!UICONTROL Work List].

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Home]**.
1. Click the **[!UICONTROL Group by]** ![Group by](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png) drop-down menu.

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. Select from the following options:


>[!NOTE]
>
>The default sorting is ascending. If you change the sorting to descending, the selected sorting options are stored in the browser. If you consistently use the same browser on the same computer (and do not clear the site data) the sorting does not change, but if you switch browsers or computers then the sorting changes to the default sorting.

## View late items

[!DNL Adobe Workfront] uses the following dates to determine if work requests are late:

* **Tasks**: [!UICONTROL Planned Completion Date]
* **Issues**: [!UICONTROL Planned Completion Date]
* **Documents**: [!UICONTROL Submitted date]
* **Timesheets**: [!UICONTROL Submitted date]
* **Approvals**: [!UICONTROL Submitted date]
* **Proof approvals**: [!UICONTROL Proof deadline]

## Search the [!UICONTROL Work List]

When you search the [!UICONTROL Work List], any items assigned to you are returned in the search (even items that are not currently loaded on the screen). If the [!UICONTROL Show complete] option is selected, any items you marked complete within the past two weeks are also returned.

In addition, only the names of the work items are searched (information within the work item are not searched, nor are the names of the projects where the work item resides).

To search the [!UICONTROL Work List]:

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Home]**.
1. (Optional) Filter and group the [!UICONTROL Work List], as described in [Filter the [!UICONTROL Work List]](#filter-the-work-list) and [Group and sort by Date, Project, and Priority](#group-and-sort-by-date-project-and-priority).

1. (Optional) If you are searching for a work item that is already complete, you must configure the [!UICONTROL Work List] to display completed items before searching.

1. Click the Search icon ![Search](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png). 
1. Begin typing the name of the item name you are searching for.\
   The [!UICONTROL Work List] is automatically filtered as to include items with a matching name.


## Collapse and expand groupings

Items in the [!UICONTROL Work List] are displayed within groupings. You can collapse and expand groupings to control how much information is displayed on the page at a given time.

You can collapse and expand groupings within the [!UICONTROL Work List] to better control what information is visible.\
By default, the [!UICONTROL This Week] grouping is expanded and all other groupings are collapsed. Any changes you make are remembered the next time you access the Home area.

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Home]**.
1. Click the **[!UICONTROL Expand]** or **[!UICONTROL Collapse]** arrow next to any grouping you want to expand or collapse.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Or\
   To expand or collapse all groupings simultaneously, click the **[!UICONTROL Expand]** or **[!UICONTROL Collapse]** arrow next to any grouping while holding down the [!UICONTROL Shift] key.
