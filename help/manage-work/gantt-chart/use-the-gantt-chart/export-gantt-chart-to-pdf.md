---
filename: export-gantt-chart-to-pdf
navigation-topic: use-the-gantt-chart
title: Export the Gantt Chart to PDF
description: You can export the Gantt chart to PDF.
---

# Export the Gantt Chart to PDF

You can export the Gantt chart to PDF.

After exporting the Gantt chart to PDF, you can print or attach it to an email, to share it with other users.&nbsp;

## Access requirements

You must have the following to follow the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Review</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Export the Gantt chart

<ol> 
 <li value="1">Access the Gantt chart that you want to export to PDF, as described in <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md" class="MCXref xref">Get started with the Gantt Chart</a>.</li> 
 <li value="2">Ensure that you have configured the Gantt chart to display the appropriate information before you export it. <note type="note">
   If you export the Gantt chart from a list of projects, the PDF file contains just the projects in the list, not the tasks on each project. If you want to export a list of tasks, you can do so from the project they are associated with, or by building a task report and displaying the results of the report in the Gantt View.&nbsp;
  </note><p>You can configure the following information:</p> 
  <ul> 
   <li>Filters, Views, and Groupings as desired in the list of tasks. Any Filters and Groupings that are selected in the list view are maintained when viewing the Gantt chart. Views are reflected on the exported Gantt chart only within the list that is displayed next to the Gantt chart on the first page. Views are not displayed on the Gantt chart itself.<note type="tip">
      To allow more room for the Gantt chart itself, apply a view that contains&nbsp;as few columns as possible.
    </note></li> 
   <li><p>Configuration options on the Gantt chart. For example, you can enable milestones, dates, baselines, or percent complete to appear on the Gantt chart.</p><p>For more information, see &nbsp;<a href="../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md" class="MCXref xref">Configure how information displays on the Gantt Chart </a>.</p><note type="note">
     &nbsp;Assignments are&nbsp;not displayed on the Gantt chart when the Gantt chart is exported to PDF. When the Gantt chart is exported to PDF, assignments are displayed only in the list view.
    </note></li> 
   <li><p>The time period that is displayed on the Gantt chart.<br>For more information, see <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md">Viewing&nbsp;Information in the Gantt Chart</a>. </p><p>The way the time period is displayed in the export file depends on whether you select <span class="bold">What I see</span>&nbsp;or <span class="bold">Multiple pages</span>&nbsp;in a later step.</p></li> 
  </ul></li> 
 <li value="3"> <p>(Optional) To include&nbsp;only certain tasks&nbsp;in the exported PDF, select the tasks&nbsp;that you want to include.</p> <p>If you do not select any tasks, all tasks&nbsp;are included in the exported PDF.</p> <p>For example, if you are viewing the Gantt chart for a project that contains 50 tasks, but you want to display only 10 tasks on the exported Gantt chart, select the 10 tasks that you want to display.</p> </li> 
 <li value="4"> <p>Click the printer icon.<br>The <span class="bold">Export to PDF</span> dialog box is displayed.<br> <img src="assets/exported-gantt-ui-350x225.png" alt="exported_gantt_UI.png" style="width: 350;height: 225;"></p> </li> 
 <li value="5"> <p>Select&nbsp;whether you want to export only what you see or the entire Gantt chart:</p> 
  <ul> 
   <li> <p><span class="bold">What I see:</span>&nbsp;Exports all tasks (including any subtasks) that are displayed on the screen prior to exporting up to 500 items. (This is not what is displayed in the <span class="bold">Preview</span> section; the Preview section contains only sample data.)</p> <p>Subtasks are included in the exported PDF even if the parent task is collapsed and the subtasks are not visible. To include only parent tasks, select the parent tasks you want to include and leave any subtasks unselected.</p> <p>You can use the <span class="bold">Zoom To</span> drop-down menu or the slider tool to display only a portion of the Gantt chart, as described in <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md">Viewing&nbsp;Information in the Gantt Chart</a> .</p> </li> 
   <li><span class="bold">Multiple pages:</span>&nbsp;Exports the entire Gantt chart, even that which is not visible on the current screen up to 500 items.<br>You can use the <span class="bold">Zoom To</span> drop-down menu or the slider tool to determine how much information is displayed on each page, as described in <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md" class="MCXref xref">Configure how information displays on the Gantt Chart </a>.&nbsp;Select a more granular option to display more pages to export, or&nbsp;select a less granular option to display fewer pages to export.<br> <note type="note">  
     <p>If you need to export a Gantt chart that contains more than 500 items, apply a Filter to the list before viewing the Gantt chart so that fewer than 500 items or 250 pages are displayed. For information about how to apply a filter, see&nbsp;<a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</p> 
     <p>You cannot export the entire Gantt chart&nbsp;in the following circumstances:&nbsp;</p> 
     <ul> 
      <li>When it spans more than 250 pages</li> 
      <li>When it contains more than 500 items</li> 
     </ul> 
    </note></li> 
  </ul> </li> 
 <li value="6"> <p>If&nbsp;the PDF will be printed after it is exported to PDF, in the <span class="bold">Page Size</span>&nbsp;drop-down menu, select the size of paper you want to print to. <br>You can select <span class="bold">Letter</span>, <span class="bold">Legal</span>, <span class="bold">Ledger</span>, <span class="bold">A1</span>, <span class="bold">A2</span>,&nbsp;<span class="bold">A3</span> (available only for some languages), or <span class="bold">A4</span>.</p> </li> 
 <li value="7"> <p>In the&nbsp;<span class="bold">Page Orientation</span> section, select whether you want the PDF to be&nbsp;exported in landscape or portrait orientation.</p> </li> 
 <li value="8"> <p>Select <span class="bold">Show Legend</span> if you want to include the Legend in your exported PDF.&nbsp;</p> </li> 
 <li value="9"> <p>Click <span class="bold">Export</span>.</p> <p>The pdf of the Gantt chart is created and downloaded to your computer.</p> <p>Notice the legend&nbsp;at the bottom of the exported file. It explains only&nbsp;the options that you have enabled in your Gantt chart&nbsp;and that are available in your task list. </p> <p>For example, milestones are displayed in the legend&nbsp;only if you have at least one&nbsp;task associated with a milestone.</p> <p> <img src="assets/gantt-chart-with-updated--limited--legend-350x271.png" alt="gantt_chart_with_updated__limited__legend.png" style="width: 350;height: 271;">&nbsp;</p> </li> 
</ol>

