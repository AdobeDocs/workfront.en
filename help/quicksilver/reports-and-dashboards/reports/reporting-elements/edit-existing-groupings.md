---
title: Edit existing groupings
description: Edit existing groupings
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
---
# Edit existing groupings

<!-- Audited: 11/2024 -->

<!--NOTE: This is the third part of a former article split in 3: two how-tos and one reference article about creating and customizing groupings)-->

You can customize an existing grouping that you originally created or that was shared with you. Then, you can save it as a new grouping.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</strong></td> 
   <td> 
    <p>Contributor or higher</p>
    <p>Request or higher</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to Reports, Dashboards, Calendars to edit a grouping in a report</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
    <td> <p>Manage permissions to a report to edit a grouping in a report</p> <p>Manage permissions to a grouping</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Prerequisites

You must create a grouping before you can edit it.

For information on creating a grouping, see [Create groupings in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## How-to steps

1. Go to a list of objects that contains the grouping that you want to customize.
1. Click the **Grouping** icon.
1. Select the grouping that you want to customize, then click the **Edit** icon ![Edit icon](assets/edit-icon.png).

   ![Select the edit icon.](assets/customizegrouping-nwe-standard-350x291.png)

   The interface builder for customizing the grouping opens.

1. In the **Grouping Preview** section, click **Add Grouping** to define how you want information in the report to be organized. A preview of what the grouping looks like in the report is shown below.

1. Begin typing the name of the field that represents the way that you want to organize information in the report, then click it when it appears in the drop-down list.
1. (Optional and conditional) When viewing an updated list, select **Collapse this grouping by default** if you want the results in the grouping to display collapsed rather than expanded. This setting is disabled by default and the results of the grouping always display in the expanded list.

   For information about updated and legacy lists, see the section "The difference between updated and legacy lists" in the article [Get started with lists in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* When you manually adjust groupings when viewing a list, Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting.
   >* The results of a grouping always display expanded after accessing them from a chart element or in a legacy list. In these cases, this setting is ignored.

1. Repeat Steps 4, 5, and 6 to define additional groupings.  
   You can define up to three groupings for organizing information. You can further organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see [Create a matrix report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Click **Save Grouping** to replace the current grouping with your changes.
