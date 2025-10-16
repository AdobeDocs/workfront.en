---
navigation-topic: use-the-gantt-chart
title: Export the Gantt Chart to PDF
description: You can export the Gantt chart to a PDF. Afterward, you can print or attach it to an email to share it with other users.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
---
# Export the [!UICONTROL Gantt Chart] to PDF

<!--Audited: 08/2025-->

You can export the [!UICONTROL Gantt chart] to a PDF. Afterward, you can print or attach it to an email to share it with other users. 

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] license</td> 
   <td> <p>[!UICONTROL Light] or higher</p>
   <p>[!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project and tasks</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] license</td> 
   <td> <p>New:[!UICONTROL Light] or higher</p>
   <p>Current:[!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Export the [!UICONTROL Gantt chart]

1. Access the [!UICONTROL Gantt chart] that you want to export to PDF, as described in [Get started with the [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Configure the [!UICONTROL Gantt chart] to display the appropriate information you want to export.

   >[!NOTE]
   >
   >If you export the [!UICONTROL Gantt chart] from a list of projects, the PDF file contains just the projects in the list, not the tasks on each project. If you want to export a list of tasks, you can do so from the project they are associated with, or by building a task report and displaying the results of the report in the [!UICONTROL Gantt View]. 

   Configure any of the following information:

   * Click the **Filters**, **View**, and **Grouping** icons above the [!UICONTROL Gantt chart] and add or edit the existing filter, view, or grouping applied to the list of items in the [!UICONTROL Gantt chart]. 
   
      Any filters and groupings that are selected in the list view are maintained when viewing the [!UICONTROL Gantt chart]. Views are reflected on the exported [!UICONTROL Gantt chart] only within the list that displays next to the [!UICONTROL Gantt chart] on the first page. Views are not displayed on the [!UICONTROL Gantt chart] itself.

      >[!TIP]
      >
      >To allow more room for the [!UICONTROL Gantt chart], apply a view that contains as few columns as possible.

   * Select the **Switch to Projected Dates** option to view Projected rather than Planned Dates. By default, Planned Dates display.  

   * Click the **Settings** icon ![Settings icon](assets/settings-icon.png) in the upper-right corner of the Gantt chart and select what information you want to view. Once selected, this information is included in the exported Gantt PDF file. 
   
      Select from the following options: 

      * Actual Dates
      * Assignments
      * Baseline
      * Commit Date
      * % Complete
      * Critical Path
      * Milestone Diamonds
      * Milestone Lines
      * Predecessors
      * Progress Status
      * (Conditional) Planned Dates
      * (Conditional) Projected Dates

      For more information, see   [Configure how information displays on the [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

      >[!NOTE]
      >
      > Assignments are not displayed on the [!UICONTROL Gantt chart] when the [!UICONTROL Gantt chart] is exported to PDF. Once exported, assignments are displayed only in the list view.

   * The time period that is displayed on the [!UICONTROL Gantt chart]. The way this displays in the export file depends on whether you select **[!UICONTROL What I see]** or **[!UICONTROL Multiple pages]** in a later step.

      For more information, see [Viewing Information in the [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

 

1. (Optional) To include only certain tasks in the exported PDF, select the tasks that you want to include. If you do not select any tasks, all tasks are included in the exported PDF.

   For example, if you are viewing the [!UICONTROL Gantt chart] for a project that contains 50 tasks, but you want to display only 10 tasks on the exported [!UICONTROL Gantt chart], select the 10 tasks that you want to display.

1. Click the printer icon ![Printer icon](assets/printer-icon.png) in the upper-right corner of the Gantt chart.
   The **[!UICONTROL Export to PDF]** dialog box displays.

   ![Exprot to PDF dialog box](assets/exported-gantt-ui-350x225.png)

1. In the **Export** section, select from the following options to indicate whether you want to export only what you see or the entire [!UICONTROL Gantt chart]:

   * **[!UICONTROL What I see]:** Exports all tasks (including any subtasks) that are displayed on the screen prior to exporting up to 500 items. (This is not what is displayed in the **[!UICONTROL Preview]** section; the **Preview** section only contains sample data.)

      Subtasks are included in the exported PDF even if the parent task is collapsed and the subtasks are not visible. To include only parent tasks, select the parent tasks you want to include and leave any subtasks unselected.

      >[!TIP]
      >
      >You can use the zoom or slider tool to display only a portion of the [!UICONTROL Gantt chart], as described in [Viewing Information in the [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md). Select a more granular option to display more pages to export or select a less granular option to display fewer pages to export.


   * **[!UICONTROL Multiple pages]:** Exports the entire [!UICONTROL Gantt chart] (up to 500 items), including items that aren't visible on the current screen.

      >[!NOTE]
      >
      >* If you need to export a [!UICONTROL Gantt chart] that contains more than 500 items, apply a filter to the list before viewing the [!UICONTROL Gantt chart] so that fewer than 500 items or 250 pages are displayed. For information about how to apply a filter, see  [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
      >
      >
      >* You can't export the entire Gantt chart in the following circumstances: 
      >   
      >   * When it spans more than 250 pages.
      >   * When it contains more than 500 items.


1. If the PDF will be printed after it is exported to PDF, select the size of paper you want to print to in the **[!UICONTROL Page Size]** drop-down menu.
   You can select from the following options:
   
      * **[!UICONTROL Letter]**
      * **[!UICONTROL Legal]**
      * **[!UICONTROL Ledger]**
      * **[!UICONTROL A1]**
      * **[!UICONTROL A2]**
      * **[!UICONTROL A3]** (available only for some languages)
      * **[!UICONTROL A4]**
1. In the **[!UICONTROL Page Orientation]** section, select whether you want the PDF to be exported in landscape or portrait orientation.
1. Select **[!UICONTROL Show Legend]** if you want to include the Legend in your exported PDF. 
1. Click **[!UICONTROL Export]**. The pdf is created and downloads to your computer.

   The legend at the bottom of the exported file explains only the options that you have enabled in your [!UICONTROL Gantt chart] and that are available in your task list. For example, milestones are displayed in the legend only if you have at least one task associated with a milestone.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png) 
