---
filename: groupings-overview
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Groupings overview in Adobe Workfront
description: You can add groupings to manage the layout of the information in your reports and lists.
---

# Groupings overview in Adobe Workfront

You can add groupings to manage the layout of the information in your reports and lists.

You can add groupings to reports in the following ways:

* You can create groupings by editing existing groupings.

  For information about customizing an existing Grouping, see [Edit existing groupings](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* You can create groupings from scratch.

  For information about creating a grouping from scratch, see [Create groupings in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

By default, groupings are shown in a blue highlight in your report or list. The results of the report or list are listed under their individual grouping, with no highlight.

You can add up to three groupings to a report. You can organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see [Create a matrix report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

In a standard grouping report, the first grouping is darker blue, the second and third groupings are lighter blue. You cannot customize the color of the highlight for your grouping, or the font of the grouping name. The number in parentheses after the name of the grouping represents the number of results under that grouping. If your report spans multiple pages, ensure that you display *All* the results in the report or list to get an accurate count for your results under each grouping.

![](assets/screen-shot-2016-10-11-at-4.05.35-pm-350x43.png)

Consider the following when working with groupings:

* You can customize the information in existing groupings. All users who can view the groupings can also see your changes.
* Your Workfront administrator must grant you access to Edit Filters, Views, and Groupings to create groupings.

  For information about granting access to Filters, Views, and Groupings, see [Grant access to filters, views, and groupings](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Your level of permissions to a grouping dictates how a grouping is saved. If you created the grouping originally, you can save the changes, otherwise you are prompted to save a version of the grouping. If you make changes to a grouping you have shared with others it impacts them as well.
* You can customize a grouping that was shared with you only if the user who shared it granted you Manage access.&nbsp;For information about sharing a grouping, see [Share a filter, view, or grouping in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* You cannot edit a grouping inline.
* You cannot group by multi-select custom fields (for example, Checkboxes), or by fields that can have multiple values (for example, Resource Manager).

## Additional information about groupings

You can further manage report information when using Groupings by aggregating the values in each column on the Grouping row, as well as sort your information by the field of your Grouping. You can also remove a Grouping when it is no longer needed.

* [Aggregate values in groupings](#aggregat) 
* [Sort by a grouping](#sorting-by-a-grouping) 
* [Remove a grouping](#removing-a-grouping)

### Aggregate values in groupings

You can aggregate the data displayed in your report in your grouping line by summarizing the values in each column of the report. For more information about summarizing column data in a grouping, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings:
>
>* All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents. 
>* Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks. 
>* Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks.
>

### Sort by a grouping

Groupings cannot be sorted. Views can be sorted. In order to sort a list by the value captured in the grouping, you must include that same value in one of the columns of the view and apply the sorting in the view. This way, the list sorts by the value in the grouping indirectly (it sorts by the value in the view which is also captured in the grouping). For more information about creating views and sorting by values inside the views, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Remove a grouping

How you remove a grouping depends on whether you initially created the grouping, or the grouping was shared with you. You cannot remove a default grouping.

* `If you created the grouping and you remove it`, the grouping is removed from the Workfront system. The grouping is no longer available to any users who you previously shared it with.
* `If the grouping was shared with you and you remove it`, the grouping is removed only for you. The user who originally created it and any other users it has been shared with still have access to the grouping.

For information about removing a grouping, see the article [Remove filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

<!--
Old content
-->

<!--
The results of a report or a list can be organized with a grouping. Groupings categorize information based on a particular piece of information.
-->

  <!--
  Understanding Groupings
  -->

  <!--
  Creating or Customizing a Grouping
  -->

  <!--
  Aggregating Values in Groupings
  -->

  <!--
  Sort by a grouping
  -->

  <!--
  Remove a grouping
  -->

<!--
Understanding Groupings
-->

<!--
Your access level dictates how a grouping is saved. If you created the grouping originally, you can save the changes, otherwise you are prompted to save a version of the grouping. If you make changes to a grouping you have shared with others it impacts them as well.
-->

<!--
By default, groupings are shown in a blue highlight in your report or list. The results of the report or list are listed under their individual grouping, with no highlight.
-->

<!--
You can add up to three groupings to a report. You can organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see Create a matrix report.
-->

<!--
In a standard grouping report, the first grouping is darker blue, the second and third groupings are lighter blue. You cannot customize the color of the highlight for your grouping, or the font of the grouping name. The number in parentheses after the name of the grouping represents the number of results under that grouping. If your report spans multiple pages, ensure that you display All the results in the report or list to get an accurate count for your results under each grouping.
-->

<!--

-->

<!--
Consider the following when working with groupings:
-->

  <!--
  You can customize the information in existing groupings.
  -->

  <!--
  You can create new groupings based on existing groupings.
  -->

  <!--
  You can create new groupings from scratch.
  -->

  <!--
  You cannot edit a grouping in-line.
  -->

  <!--
  You cannot group by multi-select custom fields (for example, Checkboxes), or by fields that can have multiple values (for example, Resource Manager).
  -->

<!--
Creating or Customizing a Grouping
-->

  <!--
  Customizing an Existing Grouping
  -->

  <!--
  Creating a New Grouping Based on an Existing Grouping
  -->

  <!--
  Creating a New Grouping from Scratch
  -->

<!--
Customizing an Existing Grouping
-->

   <!--
   Navigate to a list of objects that contains the grouping that you want to customize.
   -->

   <!--
   Click the Grouping drop-down list.
   -->

   <!--
   Select the grouping that you want to customize.
   -->

   <!--
   Click the Grouping drop-down list, then click Customize Grouping. The interface builder for customizing the Grouping is launched.
   -->

   <!--
   In the Grouping Preview section, click Add Grouping to define how you want information in the report to be organized. A preview of what the grouping looks like in the report is shown below.
   -->

   <!--
   Begin typing the name of the field that represents the way that you want to organize information in the report, then click it when it appears in the drop-down list.
   -->

   <!--
   Repeat Step 4 and Step 5 to define additional groupings. You can define up to three groupings for organizing information. You can further organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see Create a matrix report.
   -->

   <!--
   Click Save Grouping to replace the current grouping with your changes.
   -->

<!--
Creating a New Grouping Based on an Existing Grouping
-->

   <!--
   Go to the report that contains the grouping that you want to use as a basis for your new grouping.
   -->

   <!--
   Click the Grouping drop-down list.
   -->

   <!--
   Select the Grouping that you want to use as the basis for the new grouping.
   -->

   <!--
   Click the Grouping drop-down list, then click Customize Grouping. The interface builder for customizing the grouping is launched.
   -->

   <!--
   In the Grouping Preview section, click Add Grouping to define how you want information in the report to be organized. A preview of what the grouping looks like in the report is shown below.
   -->

   <!--
   Begin typing the name of the field that represents the way that you want to organize information in the report, then click it when it appears in the drop-down list.
   -->

   <!--
   Repeat Step 4 and Step 5 to define additional groupings. You can define up to three groupings for organizing information. You can further organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see Create a matrix report.
   -->

   <!--
   Click Save as New Grouping to save your changes as a new grouping.
   -->

<!--
Creating a New Grouping from Scratch
-->

   <!--
   Go to the report where you want to create your new grouping.
   -->

   <!--
   Click the Grouping drop-down list.
   -->

   <!--
   Click New Grouping. The interface builder for creating the grouping is launched.
   -->

   <!--
   In the Grouping Preview section, click Add Grouping to define how you want information in the report to be organized. A preview of what the grouping looks like in the report is shown below.
   -->

   <!--
   Begin typing the name of the field that represents the way that you want to organize information in the report, then click it when it appears in the drop-down list.
   -->

   <!--
   Repeat Step 4 and Step 5 to define additional groupings. You can define up to three groupings for organizing information. You can further organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see Create a matrix report.
   -->

   <!--
   Click Save Grouping.
   -->

<!--
Aggregating Values in Groupings
-->

<!--
You can aggregate the data displayed in your report in your grouping line by summarizing the values in each column of the report. For more information about summarizing column data in a grouping, see Views overview in Adobe Workfront.
-->

>[!NOTE]
>
><!-->
>The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings:>
>-->
>  <!-->
>  All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents.>
>  -->
>  <!-->
>  Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks.>
>  -->
>  <!-->
>  Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks.>
>  -->

<!--
Sorting by a Grouping
-->

<!--
Groupings cannot be sorted. Views can be sorted. In order to sort a list by the value captured in the grouping, you must include that same value in one of the columns of the view and apply the sorting in the view. This way, the list sorts by the value in the grouping indirectly (it sorts by the value in the view which is also captured in the grouping). For more information about creating views and sorting by values inside the views, see Views overview in Adobe Workfront.
-->

<!--
Removing a Grouping
-->

<!--
The ability to remove a grouping functions differently depending on whether you initially created the grouping, or the grouping was shared with you. You cannot remove a default filter.
-->

  <!--
  If you created the grouping and you remove it, the grouping is removed from the Workfront system. The grouping is no longer available to any users who you previously shared it with.
  -->

  <!--
  If the grouping was shared with you and you remove it, the grouping is removed only for you. The user who originally created it and any other users it has been shared with still have access to the grouping.
  -->

<!--
To remove a grouping:
-->

   <!--
   In the Grouping drop-down menu, click Remove Grouping. The My Groupings dialog box is displayed. All groupings that you have rights to remove are available to remove. Other groupings are displayed as dimmed.
   -->

   <!--
   Click the (x) next to any groupings you want to remove, then click Done.
   -->

