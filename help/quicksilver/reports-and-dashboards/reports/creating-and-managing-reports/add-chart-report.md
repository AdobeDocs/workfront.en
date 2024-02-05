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

You can enhance your reports by adding a chart. You can add charts to existing reports or to reports that you are creating.

Before you add a chart to a report, you should create a View and a Grouping for the report. Most charts cannot be added unless the information is grouped in the report. The only chart that can be added without a grouping is a gauge chart.  
For information about how to create a View, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).  
For more information about groupings, see [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

If your report displays too many items, a chart is not created. In this case, you must also add a Filter to the report to reduce the number of results in your report.  
For more information about filters, see [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Access requirements

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add a chart to a report

1. Go to an existing report or create a new report. For more information about creating a new report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. (Conditional) If you went to an existing report, click **Report Actions** > **Edit**.

1. Ensure that the **Columns (View)** tab has been updated to meet the needs of the report.  
   For information about how to create or modify the View for the report, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Click the **Groupings** tab and add a grouping.

   >[!TIP]
   >
   >* You can only add a chart to a report when the report results are grouped. 
   >* Text-mode groupings are not supported in charts. For more information about text-mode groupings, see [Edit text mode in a grouping](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md). 
   >* If you add a single grouping that represents one metric, all charts but a pie chart display each result in the grouping as the same color. 

   For more information about groupings, see [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Select the **Chart** tab.
1. Click a chart type to select it.  
   ![](assets/qs-report-builder-chart-350x265.png)

1. You can add the following types of charts to an Adobe Workfront report:

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
1. In the **Left (Y) Axis** field, select the values that you want to include on the Y axis of the chart, as well as how you want the information to be summarized.
1. In the **Bottom (X) Axis** field, select the Grouping that you want to include in the chart.
1. (Optional) Select **Custom Colors** to assign your preferred colors to each of the columns.  
   For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Select **Show in 3D** to display the chart in a 3-dimensional view.
1. (Optional) **Group Columns**: Select this option to define how you want the columns to be grouped.  
   Select from the following options:

   * Click one of the following options to select how the grouped columns are going to display:  
     **- Side by side** 
     **- Stacked** 
     **- Stacked to 100%**
   
   * Select the Grouping that you want to include in the chart.
   * (Optional) Select **Custom Colors** to customize the colors of the columns.  
     For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Select **Combination Chart** to include an additional value in the chart, as well as how you want the information to be summarized.  
   Consider the following options:

   * **Plot on Secondary Axis**: Select this option to plot the data on the right-hand side of the chart.
   * **Chart Type**: Select whether you want this additional value to be displayed as a line or a third column.  
     ![](assets/qs-column-chart-350x163.png)

1. Click **Save + Close** to save the chart and the report.

### Bar chart {#bar-chart}

To add a **Bar** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).
1. In the **Bottom (X) Axis** field, select the values that you want to include on the X axis of the chart, as well as how you want the information to be summarized.
1. In the **Left (Y) Axis** field, select the Grouping that you want to include in the chart.
1. (Optional) Select **Custom Colors** to customize the colors of the bars.  
   For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Select **Show in 3D** to display the chart in a 3-dimensional view.
1. (Optional) Group Bars**: Select this option to define how you want the bars to be grouped.  
   Select from the following options:

   * Click one of the following options to select how the grouped bars are going to display:  
     **- Side by side** 
     **- Stacked** 
     **- Stacked to 100%**
   
   * Select the Grouping that you want to include in the chart.
   * (Optional) Select **Custom Colors** to customize the colors of your columns.  
     For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Select **Combination Chart** to include an additional value in the chart, as well as how you want the information to be summarized.  
   ![](assets/qs-bar-chart-350x167.png)

1. Click **Save + Close** to save the chart and the report.

>[!IMPORTANT]
>
>Limit bar charts to 23 or fewer bars, as bar charts that include more than 23 bars will not properly display all bar labels.

### Pie chart {#pie-chart}

To add a **Pie** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).
1. In the **Values** field, select the values that you want to be displayed on the report, as well as how you want them to be summarized.  
   In the **Wedges** field, select the Grouping that you want to include in the chart. The Grouping is represented by the wedges of the chart.

1. (Optional) Select **Custom Colors** to customize the colors of the wedges on the chart.  
   For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Select **Show in 3D** to display the chart in a 3-dimensional view.
1. In the **Show Results As** field, select how you want the results to display in the chart. Consider the following options:

   * **Percentage**: The chart results display as a percentage.
   * **Numbers**: The chart results display as a number.  
     ![](assets/qs-pie-chart-350x171.png)

1. Click **Save + Close** to save the chart and the report.

### Line chart {#line-chart}

To add a **Line** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).
1. In the **Left (Y) Axis** field, select the values that you want to include on the Y axis of the chart, as well as how you want the information to be summarized.
1. In the **Bottom (X) Axis** field, select the Grouping that you want to include in the chart.
1. (Optional) Select a color to customize the color of the line.
1. (Optional) Select **Group Lines**, to select an additional grouping for the chart.  
   (Optional) Select **Custom Colors** to customize the colors for your new grouping.  
   For more information about customizing chart colors, see [Customize chart colors](#customize-chart-colors).

1. (Optional) Select **Combination Chart** to combine your lines by an additional value.  
   Consider from the following options:

   * Select the value that you want to include in the chart, as well as how you want the information to be summarized.  
   * Select the **Plot on Secondary Axis** field to plot the data on the right-hand side of the chart.  
     ![](assets/qs-line-chart-350x172.png)

1. Click **Save + Close** to save the chart and the report.

### Gauge chart {#gauge-chart}

A **Gauge** chart displays the number of records that meet a certain criteria in a gauge format. The indicator of the gauge points to the number of records that meet the criteria selected in the view and grouping of the report. A report grouping is not required to configure a gauge chart.

To add a **Gauge** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).
1. In the **Values** field, select the values that you want to be displayed on the report, as well as how you want them to be summarized. If you select **Record Count**, the values displayed are the object of the report.

1. In the **Indicators** field, select the Grouping that you want to include in the chart. The Grouping is represented by the indicator line on the chart.  
   If you have a Grouping that contains two items, two indicators are displayed on the chart.  
   For example, if you have a Grouping of Project Status, and there are two project statuses (Current and On Hold), your Gauge chart contains two gauge indicators. They will point to the number of projects that are in that status.  
   (Optional) Select **Total** in the **Indicators** field to display the total of the objects selected in the **Values** field.

1. In the **Value Range** field, specify the range of values and the color to represent those values to display on the Gauge chart.
1. (Optional) Click **Add Another Value Range** to add additional value ranges to the chart.  
   ![](assets/qs-gauge-chart-350x181.png)

1. Click **Save + Close** to save the chart and the report.

### Bubble chart {#bubble-chart}

You can display up to three fields of one object in a **Bubble** chart. This means you can display up to four data points in a bubble chart. Each entity with three associated fields is displayed as a circle that expresses two of the fields within its location within the X and Y axes. The third field is represented by the size of the circle.

To add a **Bubble** chart to your report:

1. Start adding a chart to your report, as described in [Add a chart to a report](#add-a-chart-to-a-report).
1. In the **Left (Y) Axis** field, select the values that you want to include on the Y axis of the chart. The values come from the view of the report. Specify how you want the information to be summarized.
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

   ![](assets/qs-bubble-chart-350x103.png)


   The **Bubble Color** can be a Grouping you define in the report, but it is only available when you select the **Name** column for the object of the report in the **Bubbles** field. 

   For example, if you selected **Task Name** in a task report, you can add **Task Status** as the **Bubble Color** field.  

   ![](assets/bubbles-field-correct-can-select-bubbles-color-example.png)   

   However, if you selected **Task Status** for the **Bubbles** field, you cannot select a **Bubble Color** field. Also, you cannot select **Project Name** for the **Bubble Color** field, even when you select **Task Name** for the **Bubble** field. 

   ![](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)
   

1. Click **Save + Close** to save the changes to the interface builder.

## Export a chart

You can export a chart to a .pdf file.

To export a chart:

1. Click **Export** to export the chart to .pdf.  
   A .pdf file is downloaded to your computer.

1. Open the .pdf file.  
   The exported file includes the following information:

   * An image of the chart.
   * A title which is the name of the report.
   * A unique file name which is the name of the report.
   * A footer with the date and time the report was exported and the page number.

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
   ![](assets/custom-colors-in-charts-350x286.png)

   >[!NOTE]
   >
   >You can associate custom colors with any field that you can group by and with some fields that can be displayed in a view, including custom fields. The custom fields or custom options of the fields you choose in the Custom Color dialog box are case-sensitive.

1. Consider selecting any of the following options:

   * **Use one color**: All the elements of the chart will display in the selected color.

      1. Start typing the name of an option of the field selected, then select a color. This option displays in the selected color on the chart.
      1. (Optional) Specify a hexadecimal color value for your color, instead of selecting one from the color samples available  
         Or  
         Click the color picker that displays after clicking the hexadecimal code, and select another color.

   * **Add Color**: Continue to add custom colors for all other possible options of the field selected.
   * **Remove All**: Select this option to remove all colors and options of the field selected above.
   * **Advanced Options**: Select from the following choices:

      * **No Value**: Select this field and a custom color to display the column of the chart that groups "no value" items. These are items that cannot be grouped by any of the options of the field selected in your grouping.
      * **All Other Values**: Select this field and a custom color to display all other chart elements whose options are not selected above.

        >[!NOTE]
        >
        >The colors you have used most recently display at the top of the Custom Colors dialog box. When you mouse over a color that has been used recently, the name of the field associated with it displays.

1. Click the "x" in the upper-right corner of the Custom Colors to close the Custom Colors dialog box. The colors you have selected are automatically saved.
1. Click **Save + Close** to save the chart and run the report.

## Remove a chart from a report

To remove a chart from a report:

1. Open the **Chart** tab of the report builder. 
1. Mouse over the icon of the chart type you chose and an "x" button will appear on the upper right corner of the icon. 
1. Click the "x" to remove the chart. 
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
