---
filename: view-user-personal-time-off
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: View: user personal time off
description: You can build a Time Off report to capture users' time off information.
---

# View: user personal time off

You can build a Time Off report to capture users' time off information.

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
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## View user personal time off

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp;
    <span class="bold">Reports >&nbsp;New Report</span>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click the 
   <span class="bold">Main Menu</span> icon 
   <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp;
   <span class="bold">Reports >&nbsp;New Report</span>.
  </MadCap:conditionalText> </li> 
 <li value="2"> <p>From the drop-down menu, select <span class="bold">Time Off</span>.</p> </li> 
 <li value="3"> <p>Click <span class="bold">Save +&nbsp;Close</span>.</p> <p>The report displays the following fields in the view by default:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">User</td> 
     <td>The name of the user who indicated the time off in their profile.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Start Date</td> 
     <td>The Start&nbsp;Date of the period of time off that the user indicated.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">End Date</td> 
     <td>The End Date of the period of time off that the user indicated.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4">(Optional) Finish creating the report by editing any of the following tabs:
  <ul>
   <li>Columns (View)</li>
   <li>Groupings</li>
   <li>Filters</li>
   <li>Chart</li>
  </ul><p>For information about creating reports, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p><note type="tip">
   We recommend adding a grouping for the User object, to make the report easier to read.
  </note></li> 
</ol>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="Add"></a>Add Time Off information to a user report</h2>
-->

## Add Time Off information to a user report

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To add a column to a user view or report to display a list of future days which have been marked for time off by users:</p>
-->

To add a column to a user view or report to display a list of future days which have been marked for time off by users:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/time-off-report-350x61.png" alt="time_off_report.png" style="width: 350;height: 61;"> </p>
-->

![time_off_report.png](assets/time-off-report-350x61.png)

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Click the 
     <span class="bold">Main Menu</span> icon 
     <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp;
     <span class="bold">Reports >&nbsp;New Report.</span>
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp;
    <span class="bold">Reports >&nbsp;New Report.</span>
   </MadCap:conditionalText> </li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
   <span class="bold">Main Menu</span> icon 
   <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp;
   <span class="bold">Reports >&nbsp;New Report.</span>
  </MadCap:conditionalText> </li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the&nbsp;<span class="bold">New Report</span> drop-down menu, select&nbsp;<span class="bold">User Report</span>.</li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the&nbsp;<span class="bold">New Report</span> drop-down menu, select&nbsp;<span class="bold">User Report</span>.</li> <draft-comment>
  <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Add Column</span>.</li>
 </draft-comment>
 <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Add Column</span>.</li> <draft-comment>
  <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the <span class="bold">View</span> drop-down menu, select <span class="bold">New View</span>.</li>
 </draft-comment>
 <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the <span class="bold">View</span> drop-down menu, select <span class="bold">New View</span>.</li> <draft-comment>
  <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the header of the new column, then click<span class="bold"> Switch to Text Mode</span>.</li>
 </draft-comment>
 <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the header of the new column, then click<span class="bold"> Switch to Text Mode</span>.</li> <draft-comment>
  <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Mouse over the text mode area, and click <span class="bold">Click to edit text</span>.</li>
 </draft-comment>
 <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Mouse over the text mode area, and click <span class="bold">Click to edit text</span>.</li> <draft-comment>
  <li value="7" data-mc-conditions="QuicksilverOrClassic.Draft mode">Remove the text you find in the <span class="bold">Text Mode</span> box, and replace it with the following code:<br><draft-comment>
    <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">displayname=Personal Time Off<br>listdelimiter=<span><br>listmethod=nested(reservedTimes).lists<br>name=Upcoming Time Off<br>stretch=0<br>textmode=true<br>type=iterate<br>valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),'')<br>valueformat=HTML<br>width=150</pre>
   </draft-comment><pre data-mc-conditions="QuicksilverOrClassic.Draft mode">displayname=Personal Time Off<br>listdelimiter=<span><br>listmethod=nested(reservedTimes).lists<br>name=Upcoming Time Off<br>stretch=0<br>textmode=true<br>type=iterate<br>valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),'')<br>valueformat=HTML<br>width=150</pre></li>
 </draft-comment>
 <li value="7" data-mc-conditions="QuicksilverOrClassic.Draft mode">Remove the text you find in the <span class="bold">Text Mode</span> box, and replace it with the following code:<br><pre data-mc-conditions="QuicksilverOrClassic.Draft mode">displayname=Personal Time Off<br>listdelimiter=<span><br>listmethod=nested(reservedTimes).lists<br>name=Upcoming Time Off<br>stretch=0<br>textmode=true<br>type=iterate<br>valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),'')<br>valueformat=HTML<br>width=150</pre></li> <draft-comment>
  <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click <span class="bold">Save</span>+<span class="bold">Close</span>.</li>
 </draft-comment>
 <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click <span class="bold">Save</span>+<span class="bold">Close</span>.</li> 
</ol>

