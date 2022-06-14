---
title: Configure a bubble visualization in the Reporting Canvas
description: Configure a bubble visualization in the Reporting Canvas
draft: Probably
feature: Reports and Dashboards
---
# Configure a bubble visualization in the Reporting Canvas

A bubble visualization can help you quickly tell a story about your data by highlighting relationships between 3 or more numeric variables.

You can display up to 3 fields of one object in a bubble chart. This means you can display up to 4 data points in a bubble chart. Each entity with 3 associated fields is displayed as a circle that expresses two of the fields within its location within the X and Y axes. The third field is represented by the size of the circle.

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
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>The contents of this article are available as part of a beta program that must be joined by a Workfront administrator. After joining, the Workfront administrator may then grant access to other users in their environment. For more information on participating in the beta and granting access to users, see <a href="../../../product-announcements/betas/reporting-canvas-beta.md" class="MCXref xref">Reporting Canvas beta</a>.</p> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit access to create reports, calendars, and dashboards</p>
    --> <!--
     <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta. For more information, see [Reporting Canvas Beta](../../../product-announcements/betas/reporting-canvas-beta.md).

## Configure a bubble visualization

>[!TIP]
>
>All of your changes are saved automatically as you build and edit the blocks in your report.

1. Begin adding a visualization to your report, as explained in [Add or edit a visualization block in Reporting Canvas](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md), choosing **Bubble** as the visualization type.

1. Click the Edit visualization icon ![](assets/edit-icon.png) in the upper-right corner of the visualization, then do any of the following.

   1. On the **Settings** tab:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Visualization type</td>
         <td><p>Switch to a different type of visualization. If you do this, the subsequent options on the menu might change.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Vertical axis</td>
         <td>Select the values that you want to include on the left edge (Y axis). <!--
           <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
            The values come from the view of the report Also, specify how you want the information to be aggregated/summarized. 
            <span style="color: #ff1493;">Nolan, I took all of this (for both options) and the Important note from existing bubble chart documentation (Content/Reports and Dashboards/Reports/Creating and Managing Reports/add-chart-report.html). Add rows for the 3 other bubble chart types.</span>
           </MadCap:conditionalText>
          --></td>
        </tr>
        <tr>
         <td role="rowheader">Horizontal axis</td>
         <td><p>Select the values that you want to include along the bottom (X axis). <!--
            <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
             The values come from the view of the report. Also, specify how you want the information to be aggregated/summarized.
            </MadCap:conditionalText>
           --> </p><p>Important: Ensure that you have at least one column that is aggregated for this field to be active. For more information about summarizing the information in a report column, see <a href="../../../reports-and-dashboards/reporting-canvas/table-blocks/modify-columns-table.md" class="MCXref xref">Configure a table column in Reporting Canvas</a>.</p></td>
        </tr>
       </tbody>
      </table>

      <!--   
      <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>On the <b>Data</b> tab:</p>   
      <table style="table-layout:auto">   
      <col>   
      <col>   
      <tbody>   
      <tr>   
      <td role="rowheader">Data source (drop-down menu)</td>   
      <td>Change the data source for the visualization to another table on the report canvas.</td>   
      </tr>   
      <tr>   
      <td role="rowheader">Show Data Source</td>   
      <td>Enable this option to show the source table for the visualization on the report canvas, or disable the option to hide it.</td>   
      </tr>   
      </tbody>   
      </table></li>   
      -->

      <!--   
      <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>On the <b>Style</b> tab:</p>   
      <table style="table-layout:auto">   
      <col>   
      <col>   
      <tbody>   
      <tr>   
      <td role="rowheader">&nbsp;</td>   
      <td>&nbsp;</td>   
      </tr>   
      <tr>   
      <td role="rowheader">&nbsp;</td>   
      <td>&nbsp;</td>   
      </tr>   
      <tr>   
      <td role="rowheader">&nbsp;</td>   
      <td>&nbsp;</td>   
      </tr>   
      </tbody>   
      </table></li>   
      -->

1. Click anywhere outside the menu of visualizations settings to close it.

