---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Groupings overview in Adobe Workfront
description: You can add groupings to manage the layout of the information in your reports and lists.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
---
# Groupings overview in Adobe Workfront

<!-- Audited: 11/2024 -->

<!--(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.)-->

You can add groupings to manage the layout of the information in your reports and lists.

You can add groupings to reports in the following ways:

* You can create groupings by editing existing groupings.

  For information about customizing an existing Grouping, see [Edit existing groupings](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* You can create groupings from scratch.

  For information about creating a grouping from scratch, see [Create groupings in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

By default, groupings are shown in a gray highlight in your report or list. The results of the report or list are listed under their individual grouping, with no highlight.

![Groupings example](assets/grouping-example-blue.png)

You can add up to three groupings to a report. You can organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see [Create a matrix report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

The number in parentheses after the name of the grouping represents the number of results under that grouping. If your report spans multiple pages, ensure that you display *All* the results in the report or list to get an accurate count for your results under each grouping.

Consider the following when working with groupings:

* You can customize the information in existing groupings. All users who can view the groupings can also see your changes.
* Your Workfront administrator must grant you access to Edit Filters, Views, and Groupings to create groupings.

  For information about granting access to Filters, Views, and Groupings, see [Grant access to filters, views, and groupings](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Your level of permissions to a grouping dictates how a grouping is saved. If you created the grouping originally, you can save the changes, otherwise you are prompted to save a version of the grouping. If you make changes to a grouping you have shared with others it impacts them as well.
* You can customize a grouping that was shared with you only if the user who shared it granted you Manage access. For information about sharing a grouping, see [Share a filter, view, or grouping](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* You cannot edit a grouping inline.
* You cannot group by multi-select custom fields (for example, check boxes), or by fields that can have multiple values (for example, Resource Manager).

## Additional information about groupings

You can further manage report information when using Groupings by aggregating the values in each column on the Grouping row, as well as sort your information by the field of your Grouping. You can also remove a Grouping when it is no longer needed.

* [Aggregate values in groupings](#aggregate-values-in-groupings) 
* [Sort by a grouping](#sort-by-a-grouping) 
* [Remove a grouping](#remove-a-grouping)

### Aggregate values in groupings {#aggregate-values-in-groupings}

You can aggregate the data displayed in your report in your grouping line by summarizing the values in each column of the report. For more information about summarizing column data in a grouping, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).


>[!NOTE]
>
>The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in >groupings:
>
>* All number, currency, and date fields, except for Actual Hours, aggregate values only for children tasks and standalone tasks. They do not aggregate values for parent tasks or parents of parents. Aggregating on number, currency, and date fields on a list that includes only parent tasks will not display an aggregated value in the grouping bar.
>
>* Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks. 
>
>* Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks.


### Sort by a grouping {#sort-by-a-grouping}

Groupings cannot be sorted. Views can be sorted. In order to sort a list by the value captured in the grouping, you must include that same value in one of the columns of the view and apply the sorting in the view. This way, the list sorts by the value in the grouping indirectly (it sorts by the value in the view which is also captured in the grouping). For more information about creating views and sorting by values inside the views, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Remove a grouping {#remove-a-grouping}

How you remove a grouping depends on whether you initially created the grouping, or the grouping was shared with you. You cannot remove a default grouping.

* **If you created the grouping and you remove it**, the grouping is removed from the Workfront system. The grouping is no longer available to any users who you previously shared it with.
* **If the grouping was shared with you and you remove it**, the grouping is removed only for you. The user who originally created it and any other users it has been shared with still have access to the grouping.

For information about removing a grouping, see the article [Remove filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
