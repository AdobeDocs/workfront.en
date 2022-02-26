---
filename: create-matrix-report
product-area: reporting
navigation-topic: create-and-manage-reports
title: Create a matrix report
description: Matrix reports present summary information in an aggregated table format, making it easier to view than if it were displayed in a list like in a traditional report.
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

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Set up a matrix report

<ol> 
 <li value="1">Create a traditional report that contains numerical data in the report output.<br>For information about how to create a report, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</li> 
 <li value="2">Go to the report that you created in Step 1, click <span class="bold">Report Actions</span>, then select <span class="bold">Edit</span>.</li> 
 <li value="3">(Conditional) If you already created a View and you want o apply it to this report, click <span class="bold">Apply an Existing View</span>, then select the View from the drop-down list.</li> 
 <li value="4">(Conditional) If you want to create a new View for the report, complete the following steps:<br> 
  <ol> 
   <li value="1">Click the <span class="bold">Columns (View)</span> tab, then select a column that you want to be summarized in the matrix report.</li> 
   <li value="2"><p>In the <span class="bold">Column Settings</span> area, click the <span class="bold">Summarize this column by</span> drop-down list, then select one of the available options for summarizing the information.</p><note type="important">
     If this option is not selected, the information from the column is not displayed correctly in the matrix report.
    </note><p>
     <draft-comment>
      <img src="assets/qs-report-matrix-summarized-350x392.png" style="width: 350;height: 392;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     </draft-comment><img src="assets/qs-report-matrix-summarized-350x392.png" style="width: 350;height: 392;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li> 
   <li value="3">Repeat this process for each column in the Columns (View) tab, then click <span class="bold">Done</span>.</li> 
  </ol></li> 
 <li value="5">Click the <span class="bold">Groupings</span> tab.</li> 
 <li value="6">(Conditional) If you already created a Grouping and you want to apply it to this report, click <span class="bold">Apply an Existing Grouping</span>, then select the Grouping from the drop-down list.</li> 
 <li value="7">(Conditional) If you want to create a new matrix Grouping for the report,complete the following steps:<br> 
  <ol> 
   <li value="1">Select <span class="bold">Switch to Matrix Grouping</span> in the upper-right corner of the builder interface. </li> 
   <li value="2">In the <span class="bold">Row Groupings</span> section, identify the row grouping, which establishes the horizontal groupings of the table.</li> 
   <li value="3">(Optional) To add an additional row grouping, click <span class="bold">Add secondary Row Grouping</span>.</li> 
   <li value="4">In the <span class="bold">Column Groupings</span> section, identify the column grouping, which establish the vertical groupings of the table.</li> 
   <li value="5">(Optional) To add an additional column grouping, click <span class="bold">Add secondary Column Grouping</span>.</li> 
   <li value="6">(Conditional) If you add a grouping by date, also specify whether the results are grouped by day, week, month, quarter or year.<br><draft-comment>
     <img src="assets/qs-grouping-by-date-options-for-matrix-report-350x450.png" style="width: 350;height: 450;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    </draft-comment><img src="assets/qs-grouping-by-date-options-for-matrix-report-350x450.png" style="width: 350;height: 450;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><br></li> 
   <li value="7">(Conditional) If you selected to group by date and to show results by quarter, for example, specify whether you want to show quarters with no data by selecting the <span class="bold">Show quarters with no results</span> checkbox.<br><draft-comment>
     <img src="assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png" style="width: 350;height: 175;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    </draft-comment><img src="assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png" style="width: 350;height: 175;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><br> <note type="note">  The 
     <span class="bold">Show quarters with no results</span> field is only available for matrix groupings, and not for standard groupings. 
     <br>Only the quarters with no data that are located in-between two quarters with valid data will display zero for the data values in the matrix tab. The quarters that have no data that are located at the beginning and the end of the timeframe selected by your filter do not appear at all in the matrix grouping. The quarters with no results will not display in a grouping on the Details tab of the report. 
    </note></li> 
  </ol></li> 
 <li value="8">(Optional and conditional) Click <span class="bold">Matrix Settings</span>, then select from the following options:<br><span class="bold">Show Record Counts:</span> Select this option to display a row with the total number of entries for the given field.<br><span class="bold">Show Value Column:</span> Select this option to display the following information in the matrix: 
  <ul> 
   <li>Record Counts</li> 
   <li><p>The Value column</p> <note type="note"> This column contains information that describes what the data in each row represents. 
     <br>The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings: 
     <br> 
     <ul> 
      <li>All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents.</li> 
      <li>Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks.</li> 
      <li>Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks. If you created the matrix report to display Planned Hours or Actual Hours in the <span class="bold">Value</span> column, be aware that hours or cost information for any parent objects (such as parent tasks) are not displayed in the matrix report. To view hours on parent objects, you must view the <span class="bold">Details</span> tab.</li> 
     </ul> 
    </note></li> 
  </ul><p><span class="bold">Conditional Rules:</span> Set up any formatting rules for values that are aggregated.<br>After you add a rule, you can define field and text styles for how fields that match that rule are displayed. Click <span class="bold">Add Rule</span> after you have finished defining the rule, then <span class="bold">Done</span> to save the rule.</p></li> 
 <li value="9">Click the <span class="bold">Filters</span> tab to define what information will display in the report.</li> 
 <li value="10">(Conditional) If you already created a Filter and you want to apply it to this report, click <span class="bold">Apply an Existing Filter</span>, then select the Filter from the drop-down list.</li> 
 <li value="11">(Conditional) If you want to create a new Filter for this report, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a><draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
     and 
    <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a> 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
    and 
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a> 
  </MadCap:conditionalText> for information about the various qualifiers that you can use when building filters.</li> 
 <li value="12">Click <span class="bold">Save+Close</span> to save and view the matrix report.</li> 
</ol>

