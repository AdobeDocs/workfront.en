---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Create a matrix report
description: Matrix reports present summary information in an aggregated table format, making it easier to view than if it were displayed in a list like in a traditional report.
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
---
# Create a matrix report

Matrix reports present summary information in an aggregated table format, making it easier to view than if it were displayed in a list like in a traditional report.

## When to use a matrix report

You can create a matrix report for any report that contains 2 or more Groupings. A traditional report can contain up to 3 Groupings, and a matrix report can contain up to 4 Groupings.

For example, you want to create an Hour report that displays the hours logged during a 3-month period, and you want the report to be organized according to who entered the hours, as well as by month and week.

![](assets/report-matrix-overview-350x123.png)

## How data displays in a matrix report

Information in the matrix report is always displayed as a numerical value. In most cases, columns that contain a numerical value are best for displaying in a matrix report (such as hours logged and actual cost).

However, other columns (such as Status) can still be displayed in the matrix report as shown in the following graphic:  
![](assets/report-matrix-status-350x73.png)

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
      <td> 
      <p>New:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Current:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td><p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p></td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Set up a matrix report

1. Create a traditional report that contains numerical data in the report output.  
   For information about how to create a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Go to the report that you created in Step 1, click **Report Actions**, then select **Edit**.

1. (Conditional) If you already created a View and you want o apply it to this report, click **Apply an Existing View**, then select the View from the drop-down list.
1. (Conditional) If you want to create a new View for the report, complete the following steps:

   1. Click the **Columns (View)** tab, then select a column that you want to be summarized in the matrix report.
   1. In the **Column Settings** area, click the **Summarize this column by** drop-down list, then select one of the available options for summarizing the information.

      >[!IMPORTANT]
      >
      >If this option is not selected, the information from the column is not displayed correctly in the matrix report.

      ![](assets/qs-report-matrix-summarized-350x392.png)

   1. Repeat this process for each column in the Columns (View) tab, then click **Done**.

1. Click the **Groupings** tab.
1. (Conditional) If you already created a Grouping and you want to apply it to this report, click **Apply an Existing Grouping**, then select the Grouping from the drop-down list.
1. (Conditional) If you want to create a new matrix Grouping for the report,complete the following steps:

   1. Select **Switch to Matrix Grouping** in the upper-right corner of the builder interface. 
   1. In the **Row Groupings** section, identify the row grouping, which establishes the horizontal groupings of the table.
   1. (Optional) To add an additional row grouping, click **Add secondary Row Grouping**.
   1. In the **Column Groupings** section, identify the column grouping, which establish the vertical groupings of the table.
   1. (Optional) To add an additional column grouping, click **Add secondary Column Grouping**.
   1. (Conditional) If you add a grouping by date, also specify whether the results are grouped by day, week, month, quarter or year.  
      ![](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)  
   
   1. (Conditional) If you selected to group by date and to show results by quarter, for example, specify whether you want to show quarters with no data by selecting the **Show quarters with no results** checkbox.  
      ![](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >The **Show quarters with no results** field is only available for matrix groupings, and not for standard groupings.   
      >Only the quarters with no data that are located in-between two quarters with valid data will display zero for the data values in the matrix tab. The quarters that have no data that are located at the beginning and the end of the timeframe selected by your filter do not appear at all in the matrix grouping. The quarters with no results will not display in a grouping on the Details tab of the report.

1. (Optional and conditional) Click **Matrix Settings**, then select from the following options:  
   **Show Record Counts:** Select this option to display a row with the total number of entries for the given field.  
   **Show Value Column:** Select this option to display the following information in the matrix:

   * Record Counts
   * The Value column

     >[!NOTE]
     >
     >This column contains information that describes what the data in each row represents.   
     >The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings:   
     >
     >   
     >   
     >   * All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents.
     >   * Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks.
     >   * Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks. If you created the matrix report to display Planned Hours or Actual Hours in the **Value** column, be aware that hours or cost information for any parent objects (such as parent tasks) are not displayed in the matrix report. To view hours on parent objects, you must view the **Details** tab.
     >   
     >   
     >

   **Conditional Rules:** Set up any formatting rules for values that are aggregated.  
   After you add a rule, you can define field and text styles for how fields that match that rule are displayed. Click **Add Rule** after you have finished defining the rule, then **Done** to save the rule.

1. Click the **Filters** tab to define what information will display in the report.
1. (Conditional) If you already created a Filter and you want to apply it to this report, click **Apply an Existing Filter**, then select the Filter from the drop-down list.
1. (Conditional) If you want to create a new Filter for this report, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   for information about the various qualifiers that you can use when building filters.

1. Click **Save+Close** to save and view the matrix report.
