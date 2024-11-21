---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Add a chart to a report
description: You can enhance your reports by adding a chart. You can add charts to existing reports or to reports that you are creating.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
---
# Add a chart to a report

<!--Audited: 11/2024-->

You can enhance your reports by adding a chart. You can add charts to existing reports or to reports that you are creating.

Before you add a chart to a report, you should create a View and a Grouping for the report. 

You cannot add charts to most reports unless you first group the information in the report. The only chart that can be added without a grouping is a gauge chart.  

For information about views, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).  

For more information about groupings, see [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

If your report displays too many items, a chart is not created. In this case, you must also add a Filter to the report to reduce the number of results in your report. 

For more information about filters, see [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
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
   <td role="rowheader">Access level configuration</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars</p> <p>Edit access to Filters, Views, Groupings</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Add a chart to a report

1. Go to an existing report or create a new report. For more information about creating a new report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. (Conditional) If you went to an existing report, click **Report Actions** > **Edit**.

1. Ensure that the **Columns (View)** tab has been updated to display the information you want to chart in the report.

   For information about how to create or modify the View for the report, see [Create or edit views in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

1. Click the **Groupings** tab and add a grouping.

   >[!TIP]
   >
   >* You can only add a chart to a report when the report results are grouped. 
   >* Text-mode groupings are not supported in charts. For more information about text-mode groupings, see [Edit text mode in a grouping](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md). 
   >* If you add a single grouping that represents one metric, all charts except a pie chart display each result in the grouping as the same color. 

   For more information about creating groupings, see [Create groupings in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-groupings.md). 

1. Select the **Chart** tab.

1. Click a chart type to select it.  
   ![Chart type selection](assets/unshimmed-report-builder-chart.png)

1. Select from the following types of charts:

   * [Column chart](#column-chart) 
   * [Bar chart](#bar-chart) 
   * [Pie chart](#pie-chart) 
   * [Line chart](#line-chart) 
   * [Gauge chart](#gauge-chart) 
   * [Bubble chart](#bubble-chart)

1. Click **Save + Close** to save the chart and the report.

### Column chart {#column-chart}

To add a **Column** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).

1. In the **Left (Y) Axis** field, select the values that you want to include on the Y axis of the chart, then select how you want the information to be summarized in the **Summarized by** field.

1. (Optional) Click **Custom Colors** to assign preferred colors to each of the columns.  
   For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. In the **Bottom (X) Axis** field, select the Grouping that you want to include in the chart.

1. (Optional) Click **Show in 3D** to display the chart in a 3-dimensional view.

1. (Optional) **Group Columns**: Select this option to define how you want the columns to be grouped.  
   Select from the following options:

   * Click one of the following options to select how the grouped columns are going to display: 

      * **Side by side** 
      * **Stacked** 
      * **Stacked to 100%**
   
   * Select the Grouping that you want to include in the chart from the **Group Data by** drop-down menu.
   * (Optional) Click **Custom Colors** to customize the colors of the columns.  
     For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Click **Combination Chart** to include an additional value in the chart, as well as how you want the information to be summarized.  
   Consider the following options:

   * **Plot on Secondary Axis**: Select this option to plot the data on the right-hand side of the chart.
   * **Chart Type**: Select whether you want this additional value to be displayed as a line or a third column.  

1. Click **Save + Close** to save the chart and the report.

### Bar chart {#bar-chart}

To add a **Bar** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).

1. In the **Bottom (X) Axis** field, select the values that you want to include on the X axis of the chart, then select how you want the information to be summarized in the **Summarized by** field.

1. (Optional) Click **Custom Colors** to customize the colors of the bars.  
   For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. In the **Left (Y) Axis** field, select the Grouping that you want to include in the chart.

1. (Optional) Click **Show in 3D** to display the chart in a 3-dimensional view.

1. (Optional) Click **Group Bars** to define how you want the bars to be grouped.  
   Select from the following options:

   * Click one of the following options to select how the grouped bars are going to display: 

      * **Side by side** 
      * **Stacked** 
      * **Stacked to 100%**
   
   * Select how you want to group the information in the chart from the **Group Data by** drop-down menu.
   * (Optional) Click **Custom Colors** to customize the colors of your columns.  
     For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Click **Combination Chart** to include an additional value in the chart, as well as how you want the information to be summarized. 

1. Click **Save + Close** to save the chart and the report.

>[!IMPORTANT]
>
>Limit bar charts to 23 or fewer bars, as bar charts that include more than 23 bars will not properly display all bar labels.

### Pie chart {#pie-chart}

To add a **Pie** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).

1. In the **Values** field, select the values that you want to be displayed on the report, then select how you want the information to be summarized in the **Summarized by** field.  
   In the **Wedges** field, select the Grouping that you want to include in the chart. The Grouping is represented by the wedges of the chart.

1. (Optional) Click **Custom Colors** to customize the colors of the wedges on the chart.  
   For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Click **Show in 3D** to display the chart in a 3-dimensional view.

1. In the **Show Results As** field, select how you want the results to display in the chart. Consider the following options:

   * **Percentage**: The chart results display as a percentage.
   * **Numbers**: The chart results display as a number.

1. Click **Save + Close** to save the chart and the report.

### Line chart {#line-chart}

To add a **Line** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).

1. In the **Left (Y) Axis** field, select the values that you want to include on the Y axis of the chart, then select how you want the information to be summarized in the **Summarized by** field.

1. In the **Bottom (X) Axis** field, select the Grouping that you want to include in the chart.

1. (Optional) Click **Group Lines**, to select an additional grouping for the chart.  
   (Optional) Click **Custom Colors** to customize the colors for your new grouping.  
   For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Click **Combination Chart** to combine your lines by an additional value.  
   Consider from the following options:

   * Select the value that you want to include in the chart, as well as how you want the information to be summarized.  
   * Click the **Plot on Secondary Axis** field to plot the data on the right-hand side of the chart.  

1. Click **Save + Close** to save the chart and the report.

### Gauge chart {#gauge-chart}

A **Gauge** chart displays the number of records that meet a certain criteria in a gauge format. The indicator of the gauge points to the number of records that meet the criteria selected in the view and grouping of the report. A report grouping is not required to configure a gauge chart.

To add a **Gauge** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).

1. In the **Values** field, select the values that you want to be displayed on the report, then select how you want the information to be summarized in the **Summarized by** field. If you select **Record Count**, the values displayed are the object of the report.

1. In the **Indicators** field, select the Grouping that you want to include in the chart. The Grouping is represented by the indicator line on the chart.  
   If you have a Grouping that contains two items, two indicators are displayed on the chart.  
   For example, if you have a Grouping of Project Status, and there are two project statuses (Current and On Hold), your Gauge chart contains two gauge indicators. They will point to the number of projects that are in that status.  
   (Optional) Select **Total** in the **Indicators** field to display the total of the objects selected in the **Values** field.

1. (Optional) Click **Add Another Value Range** to add a value range to the chart.

1. (Optional) In the **Value Range** field, specify the range of values and the color to represent those values to display on the Gauge chart.  

1. Click **Save + Close** to save the chart and the report.

### Bubble chart {#bubble-chart}

You can display up to three fields of one object in a **Bubble** chart. This means you can display up to four data points in a bubble chart. Each entity with three associated fields is displayed as a circle that expresses two of the fields within its location within the X and Y axes. The third field is represented by the size of the circle.

To add a **Bubble** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).

1. In the **Left (Y) Axis** field, select the values that you want to include on the Y axis of the chart. The values come from the view of the report. Specify how you want the information to be summarized in the **Summarized by** field.

1. In the **Bottom (X) Axis field**, select the values that you want to include on the X axis of the chart. The values come from the view of the report. Specify how you want the information to be summarized.

   >[!NOTE]
   >
   >Ensure that you have at least one column that is summarized for this field to be active.  
   >For more information about summarizing the information in a report column, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. In the **Bubble Size** field, select the values that you want to represent by the size of the bubbles in the chart. The values come from the view of the report. Specify how you want the information to be summarized.

   >[!NOTE]
   >
   >Ensure that you have at least one column that is summarized for this field to be active.  
   >For more information about summarizing the information in a report column, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. In the **Bubbles** field, select the Grouping that you want to include in the chart. The Grouping is represented by the placement of the bubbles on the chart.

1. In the **Bubble Color** field, select the field that you want to be represented by the colors of the bubbles. 

   The **Bubble Color** can be a Grouping you define in the report, but the option is only available if you choose a Grouping in the **Bubbles** field that contains the **Name** of a parent object relative to the object of the report, such as **Project Name** for a task report or **Program Name** for a project report. 

   For example, if you selected **Project Name** in a task report, you can add **Task Status** as the **Bubble Color** field.  

   ![](assets/bubbles-field-correct-can-select-bubbles-color-example.png)   

   However, if you selected **Task Status** for the **Bubbles** field, you cannot select a **Bubble Color** field. Also, you cannot select **Project Name** for the **Bubble Color** field, even when you select **Project Name** for the **Bubbles** field. 

   ![](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)
   
1. Click **Save + Close** to save the changes to the interface builder.

## Customize chart colors {#customize-chart-colors}

You can let Workfront select the colors of the elements in your chart, or you can customize them while you are adding a chart to your reports. If your chart contains a single Grouping that represents one metric—such as a task report that shows the number of tasks grouped by Actual Completion Date—each result in the Grouping is displayed in the same color.

You can only choose one color for fields displayed in the View of the report. You can choose several colors—one for each option—for fields displayed in the Grouping of the report.

>[!IMPORTANT]
>
>For date fields, you can only select one color for your chart elements.

To customize chart colors:

1. While building a report, go to the **Chart** tab in the report builder.

1. Select a chart type to add to your report.  
   For more information about adding a chart to your report, see [Add a chart to a report](#add-a-chart-to-a-report).

1. Click **Custom Colors** when this field is available.  
   The Custom Colors dialog box displays.  
   ![](assets/unshimmed-custom-colors-in-charts.png)

   >[!NOTE]
   >
   >You can associate custom colors with any field that you can group by and with some fields that can be displayed in a view, including custom fields. The custom fields or custom options of the fields you choose in the Custom Color dialog box are case-sensitive.

1. Consider selecting any of the following options:

   * **Use one color**: All the elements of the chart will display in the selected color.
   * **Add Color**: Add a custom color for a possible value of the selected field.
   * **Remove All**: Select this option to remove all field values and colors specified above.
   * **No Value**: Select this field and a custom color to display the chart column that groups "no value" items. These are items that cannot be grouped by any of the options of the field selected in your grouping.
   * **All Other Values**: Select this field and a custom color to display all other chart elements whose options are not defined above.

      >[!NOTE]
      >
      >The colors you have edited most recently display to the right of the **Custom Colors** button. When you mouse over a color, the name of the field associated with it displays. You can also click a color to edit it without reopening **Custom Colors**.

1. To choose a color:
   Click inside the color picker to select a color.
   OR
   Specify a hexadecimal color value for your color.

1. Click anywhere outside of the Custom Colors dialog box to close it. The colors you have selected are automatically saved.

1. Click **Save + Close** to save the chart and run the report.

## Export a chart

You can export a chart to a .pdf file.

To export a chart:

1. On the chart tab of a report, click **Export** to export the chart to .pdf.  
   A .pdf file is downloaded to your computer.

1. Open the .pdf file.  
   The exported file includes the following information:

   * An image of the chart.
   * A title which is the name of the report.
   * A unique file name which based on the name of the report.
   * A footer with the date and time the report was exported and the page number.

## Remove a chart from a report

To remove a chart from a report:

1. Open the **Chart** tab of the report builder. 

1. Click the "x" button to the right of the chart types to remove the chart. 

1. Click **Save + Close**.

## Limitations while working with charts

Be aware of the following limitations as you are working with charts:

* The **Chart Preview** section to the right of the report builder does not contain actual data from your report. You must save the chart and view it from the **Chart** tab in order to see the chart with your data.

* Some chart elements are not editable:

   * You cannot change the font type, nor size on the values of each element.
   * You cannot change the names of your axes in the chart.

* You cannot edit the legend of the chart.
* When using calculated fields for your groupings, you cannot click the chart elements.
* The most number of data points you can display in a chart is four, in a bubble chart. All other chart types display two or a maximum of three data points.
