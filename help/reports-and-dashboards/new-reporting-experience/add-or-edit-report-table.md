

# Add or edit a report table in *Reporting Canvas*

You can add a table to a report. 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
A table ...
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode"> A table ...</MadCap:conditionalText>`

##  

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
   <td role="rowheader"><em>Workfront</em> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to create reports, calendars, and dashboards</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>Manage access to the report</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the report</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

Before you begin, you must enroll in the *Reporting Canvas* beta program.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For more information, see [link to Beta enrollment info].
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">  For more information, see [link to Beta enrollment info].</MadCap:conditionalText>`

## Add or edit a table in a report

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Reports</span>.</p> </li> 
 <li value="2"> <p>Click <span class="bold">New report</span>.</p> <p>Or</p> <p>Go to an existing report, click the <span class="bold">More</span> icon <img src="assets/more-icon-27x15.png" style="width: 27;height: 15;"> in the report header, then select <span class="bold">Edit</span>.</p> </li> 
 <li value="3"> <p>In the report builder that opens, on the right side of the screen, double-click the <span class="bold">Table</span> icon <img src="assets/table-icon.png"> or drag it onto the canvas.</p> <p>If you double-click the icon, the table displays at the top of the canvas in its default size<draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
     , which you can change by dragging its corner handles
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
    , which you can change by dragging its corner handles
   </MadCap:conditionalText>.</p> </li> 
 <li value="4"> <p>Click <b>Untitled table</b> in the table header, then type a title for the table.</p> <p> <img src="assets/table-name-350x142.png" style="width: 350;height: 142;"> </p> </li> 
 <li value="5"> <p>Click <span class="bold">Edit</span> on the table block to configure the table.</p> <note type="note"> 
   <p>If the table was already added when you opened the report, the Edit button does not display. To edit the table, click the Edit icon <img src="assets/edit-icon.png"> in the table header.</p> 
   <p> <img src="assets/edit-icon-table-header-350x71.png" style="width: 350;height: 71;"> </p> 
  </note> </li> 
 <li value="6"> <p>In the right panel, locate a field that you want to add as a column to the table, then drag it to the table to add it where you want it, or double-click it to add it as the last column in the table.</p> <p>You can type text in the <span class="bold">Search</span> box to find a field. You can also use the 2 drop-down menus under this box to narrow the list of displayed fields to one or both of the following:</p> 
  <ul> 
   <li>The object type associated with the field you want, such as Project or Task</li> 
   <li>The field type you want, such as Date or Currency</li> 
  </ul> <p>If you don't see the field you want, click <span class="bold">More fields</span> to display more.</p> </li> 
 <li value="7"> <p>Repeat Step 6 for each field that you want to add as a column.</p> <note type="tip">
   You can change the order of columns in a table by dragging a selected column to a new position.
  </note> </li> 
 <li value="8"> <p>To create a formula field to add as a column, click <b>New</b> at the top of the <b>Fields</b> list.</p> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
     A formula field [briefly describe what it is].
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
    A formula field [briefly describe what it is].
   </MadCap:conditionalText> For instructions on creating a formula field, see <a href="../../reports-and-dashboards/new-reporting-experience/create-formula-field.md" class="MCXref xref">Create a formula field in Reporting Canvas</a>.</p> </li> 
 <li value="9"> <p>Do any of the following to configure the table further:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Filter the information in the table</td> 
     <td> <p>Drag the field that you want to filter by to the <span class="bold">Filter</span> section above the table.</p> <p>For information about setting up filter rules, see <a href="../../reports-and-dashboards/new-reporting-experience/configure-filter-rules-for-table.md" class="MCXref xref">Configure filter rules in Reporting Canvas</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group the table information based on attributes</td> 
     <td> <p>Drag the field that you want to group by to the <span class="bold">Group</span> section above the table.</p> <p>For more information on creating row groups, see <a href="../../reports-and-dashboards/new-reporting-experience/group-rows-in-table.md" class="MCXref xref">Group rows in a table in Reporting Canvas</a>.</p> </td> 
    </tr> <draft-comment>
     <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <td role="rowheader">Resize the table</td> 
      <td>Click the bottom-right corner and adjust the table to the width and height that you want.</td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
     <td role="rowheader">Resize the table</td> 
     <td>Click the bottom-right corner and adjust the table to the width and height that you want.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

