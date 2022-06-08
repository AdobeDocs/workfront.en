---
title: Configure a KPI visualization in Reporting Canvas
description: Configure a KPI visualization in Reporting Canvas
draft: Probably
---
# Configure a KPI visualization in Reporting Canvas

A Key Performance Indicator (KPI) visualization can help you convey the current performance of your organization at a glance.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta. For more information, see [Reporting Canvas Beta](../../../product-announcements/betas/reporting-canvas-beta.md).

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

## Configure a KPI visualization

>[!TIP]
>
>All of your changes are saved automatically as you build and edit the blocks in your report.

1. Begin by adding a visualization block with the **KPI** visualization type to a report, as explained in [Add or edit a visualization block in Reporting Canvas](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

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
         <td role="rowheader">Source field</td>
         <td>Select the data that you want represented in the visualization.</td>
        </tr>
        <tr>
         <td role="rowheader">Aggregation type</td>
         <td><p> Indicate how you want the values summarized:</p>
          <ul>
           <li><p><b>Count</b>: The number of values</p></li>
           <li><p><b>Sum</b>: The total of all values </p></li>
           <li><p><b>Average</b>:&nbsp;The average of all values</p></li>
           <li><p><b>Minimum</b>:&nbsp;Only the lowest value</p></li>
           <li><p>Maximum:&nbsp;only the highest value</p></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

   1. On the **Data** tab:

      | Data source (drop-down menu) |Change the data source for the visualization to another table on the report canvas. |
      |---|---|
      | Show Data Source |Enable this option to show the source table for the visualization on the report canvas, or disable the option to hide it. |

      {style="table-layout:auto"}

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
      </tbody>   
      </table></li>   
      -->

1. Click anywhere outside the menu of visualizations settings to close it.

