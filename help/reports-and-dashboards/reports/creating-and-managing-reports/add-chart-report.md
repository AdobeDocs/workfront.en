---
filename: add-chart-report
product-area: reporting
navigation-topic: create-and-manage-reports
title: Add a chart to a report
description: You can enhance your reports by adding a chart. You can add charts to existing reports or to reports that you are creating.
---

# Add a chart to a report

You can enhance your reports by adding a chart. You can add charts to existing reports or to reports that you are creating.

Before you add a chart to a report, you should create a View and a Grouping for the report. Most charts cannot be added unless the information is grouped in the report. The only chart that can be added without a grouping is a gauge chart.  
For information about how to create a View, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).  
For more information about groupings, see [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

If your report displays too many items, a chart is not created. In this case, you must also add a Filter to the report to reduce the number of results in your report.  
For more information about filters, see [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

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

## Add a chart to a report

<ol> 
 <li value="1">Go to an existing report or create a new report. For more information about creating a new report, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</li> 
 <li value="2">(Conditional) If you went to an existing report, click <span class="bold">Report Actions</span> > <span class="bold">Edit</span>.</li> 
 <li value="3">Ensure that the <span class="bold">Columns (View)</span> tab has been updated to meet the needs of the report.<br>For information about how to create or modify the View for the report, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</li> 
 <li value="4"> <p>Click the <span class="bold">Groupings</span> tab and add a grouping.</p> 
  <div class="tips" data-mc-autonum="<b>Tips: </b>">
   <span class="autonumber"><span><b>Tips: </b></span></span> 
   <ul> 
    <li> <p>You can only add a chart to a report when the report results are grouped.<draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      </MadCap:conditionalText></p> </li> 
    <li> <p>Text-mode groupings are not supported in charts. For more information about text-mode groupings, see<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md" class="MCXref xref">Edit text mode in a grouping</a>. </p> </li> 
    <li> <p> <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        If you add a single grouping that represents one metric, all charts but a pie chart display each result in the grouping as the same color.
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       If you add a single grouping that represents one metric, all charts but a pie chart display each result in the grouping as the same color.
      </MadCap:conditionalText> </p> </li> 
   </ul> 
  </div> <p>For more information about groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p> </li> 
 <li value="5">Select the <span class="bold">Chart</span> tab.</li> 
 <li value="6">Click a chart type to select it.<br><draft-comment>
   <img src="assets/qs-report-builder-chart-350x265.png" style="width: 350;height: 265;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  </draft-comment><img src="assets/qs-report-builder-chart-350x265.png" style="width: 350;height: 265;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></li> 
 <li value="7"> <p>You can add the following types of charts to a <em>Adobe Workfront</em> report:</p> 
  <ul> 
   <li> <p><a href="#column-chart" class="MCXref xref">Column chart</a> </p> </li> 
   <li> <p><a href="#bar-chart" class="MCXref xref">Bar chart</a> </p> </li> 
   <li> <p><a href="#pie-chart" class="MCXref xref">Pie chart</a> </p> </li> 
   <li> <p><a href="#line-chart" class="MCXref xref">Line chart</a> </p> </li> 
   <li> <p><a href="#gauge-chart" class="MCXref xref">Gauge chart</a> </p> </li> 
   <li><a href="#bubble-chart" class="MCXref xref">Bubble chart</a> </li> 
  </ul> </li> 
 <li value="8">Click <span class="bold">Save + Close</span> to save the chart and the report.</li> 
</ol>

### Column chart

To add a `Column` chart to your report:

<ol> 
 <li value="1">Start adding a chart to your report, as described in <a href="#adding-a-chart-to-a-report" class="MCXref xref">Add a chart to a report</a>.</li> 
 <li value="2">In the <span class="bold">Left (Y) Axis</span> field, select the values that you want to include on the Y axis of the chart, as well as how you want the information to be summarized.</li> 
 <li value="3">In the <span class="bold">Bottom (X) Axis</span> field, select the Grouping that you want to include in the chart.</li> 
 <li value="4">(Optional) Select <span class="bold">Custom Colors</span> to assign your preferred colors to each of the columns.<br>For more information about customizing chart colors, see <a href="#using-custom-colors" class="MCXref xref">Customize chart colors</a>.</li> 
 <li value="5">(Optional) Select <span class="bold">Show in 3D</span> to display the chart in a 3-dimensional view.</li> 
 <li value="6">(Optional) <span class="bold">Group Columns</span>: Select this option to define how you want the columns to be grouped.<br>Select from the following options:
  <ul>
   <li>Click one of the following options to select how the grouped columns are going to display:<br><span class="bold">- Side by side</span><br style="font-weight: bold;"><span class="bold">- Stacked</span><br style="font-weight: bold;"><span class="bold">- Stacked to 100%</span></li>
   <li>Select the Grouping that you want to include in the chart.</li>
   <li>(Optional) Select <span class="bold">Custom Colors</span> to customize the colors of the columns.<br>For more information about customizing chart colors, see <a href="#using-custom-colors" class="MCXref xref">Customize chart colors</a>.</li>
  </ul></li> 
 <li value="7">(Optional) Select <span class="bold">Combination Chart</span> to include an additional value in the chart, as well as how you want the information to be summarized.<br>Consider the following options:
  <ul>
   <li><span class="bold">Plot on Secondary Axis</span>: Select this option to plot the data on the right-hand side of the chart.</li>
   <li><span class="bold">Chart Type</span>: Select whether you want this additional value to be displayed as a line or a third column.<br><draft-comment>
     <img src="assets/qs-column-chart-350x163.png" style="width: 350;height: 163;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    </draft-comment><img src="assets/qs-column-chart-350x163.png" style="width: 350;height: 163;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></li>
  </ul></li> 
 <li value="8">Click <span class="bold">Save + Close</span> to save the chart and the report.</li> 
</ol>

### Bar chart

To add a `Bar` chart to your report:

<ol> 
 <li value="1">Start adding a chart to your report, as described in <a href="#adding-a-chart-to-a-report" class="MCXref xref">Add a chart to a report</a>.</li> 
 <li value="2">In the <span class="bold">Bottom (X) Axis</span> field, select the values that you want to include on the X axis of the chart, as well as how you want the information to be summarized.</li> 
 <li value="3">In the <span class="bold">Left (Y) Axis</span> field, select the Grouping that you want to include in the chart.</li> 
 <li value="4">(Optional) Select <span class="bold">Custom Colors</span> to customize the colors of the bars.<br>For more information about customizing chart colors, see <a href="#using-custom-colors" class="MCXref xref">Customize chart colors</a>.</li> 
 <li value="5">(Optional) Select <span class="bold">Show in 3D</span> to display the chart in a 3-dimensional view.</li> 
 <li value="6">(Optional)<span class="bold">Group Bars</span>: Select this option to define how you want the bars to be grouped.<br>Select from the following options:<br>
  <ul>
   <li>Click one of the following options to select how the grouped bars are going to display:<br><span class="bold">- Side by side</span><br style="font-weight: bold;"><span class="bold">- Stacked</span><br style="font-weight: bold;"><span class="bold">- Stacked to 100%</span></li>
   <li>Select the Grouping that you want to include in the chart.</li>
   <li>(Optional) Select <span class="bold">Custom Colors</span> to customize the colors of your columns.<br>For more information about customizing chart colors, see <a href="#using-custom-colors" class="MCXref xref">Customize chart colors</a>.</li>
  </ul></li> 
 <li value="7">(Optional) Select <span class="bold">Combination Chart</span> to include an additional value in the chart, as well as how you want the information to be summarized.<br><draft-comment>
   <img src="assets/qs-bar-chart-350x167.png" style="width: 350;height: 167;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  </draft-comment><img src="assets/qs-bar-chart-350x167.png" style="width: 350;height: 167;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></li> 
 <li value="8">Click <span class="bold">Save + Close</span> to save the chart and the report.</li> 
</ol>

### Pie chart

To add a `Pie` chart to your report:

<ol> 
 <li value="1">Start adding a chart to your report, as described in <a href="#adding-a-chart-to-a-report" class="MCXref xref">Add a chart to a report</a>.</li> 
 <li value="2">In the <span class="bold">Values</span> field, select the values that you want to be displayed on the report, as well as how you want them to be summarized.<br>In the <span class="bold">Wedges</span> field, select the Grouping that you want to include in the chart. The Grouping is represented by the wedges of the chart.</li> 
 <li value="3">(Optional) Select <span class="bold">Custom Colors</span> to customize the colors of the wedges on the chart.<br>For more information about customizing chart colors, see <a href="#using-custom-colors" class="MCXref xref">Customize chart colors</a>.</li> 
 <li value="4">(Optional) Select <span class="bold">Show in 3D</span> to display the chart in a 3-dimensional view.</li> 
 <li value="5"> In the <span class="bold">Show Results As</span> field, select how you want the results to display in the chart. Consider the following options:
  <ul>
   <li><span class="bold">Percentage</span>: The chart results display as a percentage.</li>
   <li><span class="bold">Numbers</span>: The chart results display as a number.<br><draft-comment>
     <img src="assets/qs-pie-chart-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    </draft-comment><img src="assets/qs-pie-chart-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><br></li>
  </ul></li> 
 <li value="6">Click <span class="bold">Save + Close</span> to save the chart and the report.</li> 
</ol>

### Line chart

To add a `Line` chart to your report:

<ol> 
 <li value="1">Start adding a chart to your report, as described in <a href="#adding-a-chart-to-a-report" class="MCXref xref">Add a chart to a report</a>.</li> 
 <li value="2">In the <span class="bold">Left (Y) Axis</span> field, select the values that you want to include on the Y axis of the chart, as well as how you want the information to be summarized.</li> 
 <li value="3">In the <span class="bold">Bottom (X) Axis</span> field, select the Grouping that you want to include in the chart.</li> 
 <li value="4">(Optional) Select a color to customize the color of the line.</li> 
 <li value="5">(Optional) Select <span class="bold">Group Lines</span>, to select an additional grouping for the chart.<br>(Optional) Select <span class="bold">Custom Colors</span> to customize the colors for your new grouping.<br>For more information about customizing chart colors, see <a href="#using-custom-colors" class="MCXref xref">Customize chart colors</a>.</li> 
 <li value="6">(Optional) Select <span class="bold">Combination Chart</span> to combine your lines by an additional value.<br>Consider from the following options:
  <ul>
   <li>Select the value that you want to include in the chart, as well as how you want the information to be summarized.<br></li>
   <li>Select the <span class="bold">Plot on Secondary Axis</span>field to plot the data on the right-hand side of the chart.<br><draft-comment>
     <img src="assets/qs-line-chart-350x172.png" style="width: 350;height: 172;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    </draft-comment><img src="assets/qs-line-chart-350x172.png" style="width: 350;height: 172;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></li>
  </ul></li> 
 <li value="7">Click <span class="bold">Save + Close</span> to save the chart and the report.</li> 
</ol>

### Gauge chart

A `Gauge` chart displays the number of records that meet a certain criteria in a gauge format. The indicator of the gauge points to the number of records that meet the criteria selected in the view and grouping of the report. A report grouping is not required to configure a gauge chart.

To add a `Gauge` chart to your report:

<ol> 
 <li value="1">Start adding a chart to your report, as described in <a href="#adding-a-chart-to-a-report" class="MCXref xref">Add a chart to a report</a>.</li> 
 <li value="2">In the <span class="bold">Values</span> field, select the values that you want to be displayed on the report, as well as how you want them to be summarized. If you select <span class="bold">Record Count</span>, the values displayed are the object of the report.</li> 
 <li value="3">In the <span class="bold">Indicators</span> field, select the Grouping that you want to include in the chart. The Grouping is represented by the indicator line on the chart.<br>If you have a Grouping that contains two items, two indicators are displayed on the chart.<br>For example, if you have a Grouping of Project Status, and there are two project statuses (Current and On Hold), your Gauge chart contains two gauge indicators. They will point to the number of projects that are in that status.<br>(Optional) Select <span class="bold">Total</span> in the <span class="bold">Indicators</span> field to display the total of the objects selected in the <span class="bold">Values</span> field.</li> 
 <li value="4">In the <span class="bold">Value Range</span> field, specify the range of values and the color to represent those values to display on the Gauge chart.</li> 
 <li value="5">(Optional) Click <span class="bold">Add Another Value Range</span> to add additional value ranges to the chart.<br><draft-comment>
   <img src="assets/qs-gauge-chart-350x181.png" style="width: 350;height: 181;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  </draft-comment><img src="assets/qs-gauge-chart-350x181.png" style="width: 350;height: 181;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></li> 
 <li value="6">Click <span class="bold">Save + Close</span> to save the chart and the report.</li> 
</ol>

### Bubble chart

You can display up to three fields of one object in a `Bubble` chart. This means you can display up to four data points in a bubble chart. Each entity with three associated fields is displayed as a circle that expresses two of the fields within its location within the X and Y axes. The third field is represented by the size of the circle.

To add a `Bubble` chart to your report:

<ol> 
 <li value="1">Start adding a chart to your report, as described in <a href="#adding-a-chart-to-a-report" class="MCXref xref">Add a chart to a report</a>.</li> 
 <li value="2">In the <span class="bold">Left (Y) Axis</span> field, select the values that you want to include on the Y axis of the chart. The values come from the view of the report. Specify how you want the information to be summarized.</li> 
 <li value="3">In the <span class="bold">Bottom (X) Axis field</span>, select the values that you want to include on the X axis of the chart. The values come from the view of the report. Specify how you want the information to be summarized.<br><note type="note">
   Ensure that you have at least one column that is summarized for this field to be active.
   <br>For more information about summarizing the information in a report column, see 
   <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.
  </note></li> 
 <li value="4">In the <span class="bold">Bubble Size</span> field, select the values that you want to represent by the size of the bubbles in the chart. The values come from the view of the report. Specify how you want the information to be summarized.<br><note type="note">
    Ensure that you have at least one column that is summarized for this field to be active.
   <br>For more information about summarizing the information in a report column, see 
   <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.
  </note></li> 
 <li value="5">In the <span class="bold">Bubbles</span> field, select the Grouping that you want to include in the chart. The Grouping is represented by the placement of the bubbles on the chart.</li> 
 <li value="6">In the <span class="bold">Bubble Color</span> field, select the field that you want to be represented by the colors of the bubbles. The <span class="bold">Bubble Color</span> can be a Grouping you define in the report, but it can only be fields from the object you selected as <span class="bold">Bubbles</span>. For example, if you selected Task Name, you can add Task Status, but not Project Status as a <span class="bold">Bubble Color</span>.<br><draft-comment>
   <img src="assets/qs-bubble-chart-350x103.png" style="width: 350;height: 103;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  </draft-comment><img src="assets/qs-bubble-chart-350x103.png" style="width: 350;height: 103;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></li> 
 <li value="7">Click <span class="bold">Save + Close</span> to save the changes to the interface builder.</li> 
</ol>

## Export a chart

You can export a chart to a .pdf file.

To export a chart:

1. Click `Export` to export the chart to .pdf.  
   A .pdf file is downloaded to your computer.

1. Open the .pdf file.  
   The exported file includes the following information:

  * An image of the chart.
  * A title which is the name of the report.
  * A unique file name which is the name of the report.
  * A footer with the date and time the report was exported and the page number.

## Customize chart colors

You can let *Workfront* select the colors of the elements in your chart, or you can customize them while you are adding a chart to your reports.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
If your chart contains a single Grouping that represents one metric—such as a task report that shows the amount of tasks grouped by Actual Completion Date—each result in the Grouping is displayed in the same color.
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  If your chart contains a single Grouping that represents one metric—such as a task report that shows the amount of tasks grouped by Actual Completion Date—each result in the Grouping is displayed in the same color.</MadCap:conditionalText>`

You can only choose one color for fields displayed in the View of the report. You can choose several colors—one for each option—for fields displayed in the Grouping of the report.

>[!IMPORTANT]
>
>For date fields, you can only select one color for your chart elements.

To customize chart colors:

<ol> 
 <li value="1">While building a report, go to the <span class="bold">Chart</span> tab in the report builder.</li> 
 <li value="2">Select a chart type to add to your report.<br>For more information about adding a chart to your report, see <a href="#adding-a-chart-to-a-report" class="MCXref xref">Add a chart to a report</a>.</li> 
 <li value="3">Click <span class="bold">Custom Colors</span> when this field is available.<br>The Custom Colors dialog box displays.<br><img src="assets/custom-colors-in-charts-350x286.png" style="width: 350;height: 286;"><br><note type="note">
    You can associate custom colors with any field that you can group by and with some fields that can be displayed in a view, including custom fields. The custom fields or custom options of the fields you choose in the Custom Color dialog box are case sensitive.
   <br>
  </note></li> 
 <li value="4">Consider selecting any of the following options: 
  <ul>
   <li><span class="bold">Use one color</span>: All the elements of the chart will display in the selected color. 
    <ol>
     <li value="1">Start typing the name of a option of the field selected, then select a color. This option displays in the selected color on the chart.</li>
     <li value="2">(Optional) Specify a hexadecimal color value for your color, instead of selecting one from the color samples available<br>Or<br>Click the color picker that displays after clicking the hexadecimal code, and select another color.</li>
    </ol></li>
   <li><span class="bold">Add Color</span>: Continue to add custom colors for all other possible options of the field selected.</li>
   <li><span class="bold">Remove All</span>: Select this option to remove all colors and options of the field selected above.</li>
   <li><span class="bold">Advanced Options</span>: Select from the following choices:
    <ul>
     <li><span class="bold">No Value</span>: Select this field and a custom color to display the column of the chart that groups "no value" items. These are items that cannot be grouped by any of the options of the field selected in your grouping.</li>
     <li><span class="bold">All Other Values</span>: Select this field and a custom color to display all other chart elements whose options are not selected above.<br><note type="note">
        The colors you have used most recently display at the top of the Custom Colors dialog box. When you mouse over a color that has been used recently, the name of the field associated with it displays.
       <br>
      </note></li>
    </ul></li>
  </ul></li> 
 <li value="5">Click the "x" in the upper-right corner of the Custom Colors to close the Custom Colors dialog box. The colors you have selected are automatically saved.</li> 
 <li value="6">Click <span class="bold">Save + Close</span> to save the chart and run the report.</li> 
</ol>

## Remove a chart from a report

To remove a chart from a report:

1. Open the `Chart` tab of the report builder. 
1. Mouse over the icon of the chart type you chose and an "x" button will appear on the upper right corner of the icon. 
1. Click the "x" to remove the chart. 
1. Click `Save + Close`.

## Limitations while working with charts

Be aware of the following limitations as you are working with charts:

* The `Chart Preview` section to the right of the report builder does not contain actual data from your report. You must save the chart and view it from the `Chart` tab in order to see the chart with your data.

* Some chart elements are not editable:
* `<li>You cannot change the font type, nor size on the values of each element.</li>` `<li>You cannot change the names of your axes in the chart.</li>` 

* You cannot edit the legend of the chart.
* When using calculated fields for your groupings, you cannot click the chart elements.
* The most amount of data points you can display in a chart is four, in a bubble chart. All other chart types display two or a maximum of three data points.

