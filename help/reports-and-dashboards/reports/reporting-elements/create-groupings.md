---
filename: create-groupings
product-area: reporting
navigation-topic: reporting-elements
title: Create groupings
description: The results of a report or a list can be organized with a grouping. Groupings categorize information based on a particular piece of information.
---

# Create groupings

The results of a report or a list can be organized with a grouping. Groupings categorize information based on a particular piece of information.

You can create a custom grouping from scratch or customize an existing grouping. Follow the steps below to create a grouping from scratch.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to create a grouping in a report</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to edit a grouping in a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Walk-through

View the following video to learn how to create groupings to organize the information in your reports.
This video was recorded in Adobe Workfront Classic. However, the content also applies to the new Workfront experience. 

[ ![](assets/video-create-a-grouping-350x199.png)](https://workfront-video.wistia.com/medias/f9kdcqy520)

## How-to steps

1. Go to the report or the list where you want to create your custom grouping.
1. Click the `Grouping`icon.

1. Click `New Grouping`.  
   The interface builder for creating the grouping launches.

1. In the `Grouping Preview` section, click `Add Grouping` to define how you want information in the report to be organized. A preview of what the grouping looks like in the report is shown below.

1. Begin typing the name of the field that represents the way that you want to organize information in the report, then click it when it appears in the drop-down list.
1. (Optional and conditional) When building a grouping in an updated list, select Collapse this grouping by default if you want the results in the grouping to display collapsed rather than expanded. This setting is disabled by default and the results of the grouping always display in the expanded list. For information about updated and legacy lists, see the section The difference between the updated and the legacy lists in the article Get started with lists in Adobe Workfront. Tips: When you manually adjust groupings when viewing a list, Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting. The results of a grouping always display expanded after accessing them from a chart element or in a legacy list. In these cases, this setting is ignored. 
1. Repeat Steps 4, 5, and 6 to define additional groupings.  
   You can define up to three groupings for organizing information. You can further organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see [Create a matrix report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Click `Save Grouping`.

## Additional information

See also:

* [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md) 
* [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md) 
* [Edit existing groupings](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md)

<!--
Create or edit groupings in Adobe Workfront The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment. You can organize the results of a report or list with a grouping. Groupings categorize data based on a particular piece of information. For more information on groupings, see Groupings overview in Adobe Workfront. You can create groupings in lists and reports in the following ways: From scratch Edit an existing grouping that you originally created or that was shared with you Copy an existing grouping To copy an existing grouping, you can edit it and save it as a new grouping. Types of grouping-building interfaces You can create groupings using the types of grouping builders described in the table below. Builder type Grouping object Where available Standard builder All objects Reports and lists Beta builder Projects Tasks Issues Lists Note: Beta builders for groupings are not available in reports. Consider the following when creating groupings using the different builders: You can switch back and forth between the standard builder and the beta builder, where the beta option is available. After you have enabled the beta builder in one area, it is the default experience for all areas where it is available. Example: If you enable the beta builder in a project list, it is the default experience for building task and issue groupings in lists as well. Groupings are available in both builders, regardless of which experience you used to originally build them. Example: If you created a grouping using the standard builder, you can find and modify it in the beta builder interface as well. Access requirements You must have the following access to perform the steps in this article: Adobe Workfront plan* Any Adobe Workfront license* Request or higher Access level configurations* Edit access to filters, views, and groupings Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see Create or modify custom access levels. Object permissions Manage access to a grouping to be able to modify or copy it For information on requesting additional access, see Request access to objects in Adobe Workfront. *To find out what plan, license type, or access you have, contact your Workfront administrator. Create a grouping in the standard builder Regardless of the method you use to create groupings, creating a grouping from scratch or from an existing grouping is similar. Go to a list or a report where you want to create a grouping or that contains the grouping that you want to customize. Click the Groupingicon. Click New Grouping at the top of the list of groupings. Or Hover over the grouping you want to modify and click the Edit icon . The builder for customizing the grouping opens. In the Grouping Preview section, click Add Grouping to define how you want information in the report to be organized. A preview of what the grouping looks like in the report is shown below. Begin typing the name of the field that represents the way that you want to organize information in the report, then click it when it appears in the drop-down list. (Optional and conditional) When customizing a grouping in an updated list, select Collapse this grouping by default if you want the results in the grouping to display collapsed rather than expanded. This setting is disabled by default and the results of the grouping always display in the expanded list. For information about updated and legacy lists, see the section The difference between the updated and the legacy lists in the article Get started with lists in Adobe Workfront. Tips: When you manually adjust groupings when viewing a list, Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting. The results of a grouping always display expanded after accessing them from a chart element or in a legacy list. In these cases, this setting is ignored. Repeat Steps 4, 5, and 6 to define additional groupings. You can define up to three groupings for organizing information. You can further organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see Create a matrix report. (Optional) Click Switch to Text Mode to add a grouping using the Text Mode interface. For more information about creating a grouping using the text mode interface, see Edit text mode in a grouping. Click Save Grouping to create a new grouping. Or Click Save as New Grouping to create a new grouping from the selected one. The new grouping displays in the list of groupings. (Optional) Remove groupings you no longer want to display in the list. For information, see Remove filters, views, and groupings. Create a grouping in the beta builder Enable the beta builder The beta builder toggle is disabled by default. You must enable it to use the beta builder. Go to a project, task, or issue list. Click the Grouping icon , then enable the beta builder toggle. The beta builder interface opens. Tip: The header of the grouping builder interface is blue when the beta builder is enabled. This enables the beta builder for all areas of Workfront where it is available. Continue with Create a grouping in the beta builder, below. Create a grouping in the beta builder Go to a project, task, or issue list where you want to create a grouping, and click the Grouping icon . Click New Grouping to create a new grouping. Or Hover over an existing grouping in the My groupings area, then click the Edit icon to edit an existing grouping. Or Hover over an existing grouping in the My groupings area, select the More icon , and select Duplicate to copy a grouping. Start typing the name of a field in the Group by area, then select it when it displays in the list. You can also select Search all fields to view a list of all fields to group by. The fields in the advanced search are grouped by object category. Tip: As you build the grouping, the results appear immediately in the list. (Optional) Click Add grouping to add a second or third grouping. (Optional) To reorder the groupings, select a grouping and drag it to the new position. Or Select a grouping and use the keyboard arrow keys to change the order. (Optional) Make other selections for the groupings as needed: When grouping by date you must choose a date option such as week, month, or quarter. Select to set a grouping to be expanded by default. Select to delete a grouping. (Optional) Select Text Mode to continue building the grouping using the Text Mode interface. For more information about creating a grouping using the text mode interface, see Edit text mode in a grouping. (Optional) To use the grouping as an ad hoc grouping without saving it: When working in a new grouping, close the beta builder. When editing an existing grouping, select Apply. Select Save as new for a new grouping, or Save for an existing grouping. Type a name for the grouping. (Optional) Select an icon for the grouping to represent the field type. (Optional) Type a description of the grouping. Select Save. The grouping is saved in the My groupings list.
-->

