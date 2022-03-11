

# Configure a bubble visualization in the `Reporting Canvas`

<!--
10/7/21: UI isn't started
-->

A bubble visualization can help you quickly tell a story about your data by highlighting relationships between 3 or more numeric variables.

You can display up to 3 fields of one object in a bubble chart. This means you can display up to 4 data points in a bubble chart. Each entity with 3 associated fields is displayed as a circle that expresses two of the fields within its location within the X and Y axes. The third field is represented by the size of the circle.

##  

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Workfront</span> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to create reports, calendars, and dashboards</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> Object permissions Manage access to the report For information on requesting additional access, see Request access to objects in Adobe Workfront. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

Before you begin, you must enroll in the `Reporting Canvas` beta program.

<!--
For more information, see [link to Beta enrollment info].
-->

## Configure a bubble visualization

Your changes save automatically as you go.

<ol> 
 <li value="1">Begin adding a visualization to your report, as explained in <a href="../../reports-and-dashboards/new-reporting-experience/add-or-edit-report-visualization.md" class="MCXref xref">Add or edit a visualization in a report in Reporting Canvas</a>, choosing <b>Bubble</b> as the visualization type.</li> 
 <li value="2">Click the Edit visualization icon <img src="assets/edit-icon.png"> in the upper-right corner of the visualization, then do any of the following.
  <ol>
   <li value="1"><p>On the <b>Settings</b> tab:</p>
    <table cellspacing="0">
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
         The values come from the view of the report Also, specify how you want the information to be aggregated/summarized.
        --></td>
      </tr>
      <tr>
       <td role="rowheader">Horizontal axis</td>
       <td><p>Select the values that you want to include along the bottom (X axis). <!--
          The values come from the view of the report. Also, specify how you want the information to be aggregated/summarized.
         --> </p><note type="important">
         Ensure that you have at least one column that is aggregated for this field to be active. For more information about summarizing the information in a report column, see 
         <a href="../../reports-and-dashboards/new-reporting-experience/modify-columns-table.md" class="MCXref xref">Modify table columns in Reporting Canvas</a>.
        </note></td>
      </tr>
     </tbody>
    </table></li><!--
    On the Data source tab: Data source (drop-down menu) Change the data source for the visualization to another table on the report canvas Show Data Source On the report canvas, show (enable) or hide (disable) the table that powers the visualization
   --><!--
    On the Style tab:
   -->
  </ol></li> 
 <li value="3"> <p>Click anywhere outside the menu of visualizations settings to close it.</p> </li> 
</ol>

