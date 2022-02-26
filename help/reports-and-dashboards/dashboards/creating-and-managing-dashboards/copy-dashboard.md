---
filename: copy-dashboard
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copy a dashboard
description: You can copy a dashboard and all of its contents (reports, calendars, and external pages). When you copy the contents of a dashboard, you can choose to keep them as they appear on the original dashboard, or create new items which are copies of those on the original dashboard. You can also choose to not transfer or copy items on the new dashboard.
---

# Copy a dashboard

You can copy a dashboard and all of its contents (reports, calendars, and external pages). When you copy the contents of a dashboard, you can choose to keep them as they appear on the original dashboard, or create new items which are copies of those on the original dashboard. You can also choose to not transfer or copy items on the new dashboard.

## Access requirements

You must have the following:

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
   <td> <p>Edit access to Reports, Dashboards, and Calendars</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to a dashboard</p> <p>You will obtain Manage access to the copied dashboard</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisites

You must create a dashboard before you can copy it.

For information on creating dashboards, see [Create a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copy a dashboard

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png">, then click 
    <span class="bold">Dashboards</span>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click the 
   <span class="bold">Main Menu</span> icon 
   <img src="assets/main-menu-icon.png">, then click 
   <span class="bold">Dashboards</span>.
  </MadCap:conditionalText> </li> 
 <li value="2"> <p>Select the dashboard that you want to copy, then click <span class="bold">Copy</span> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     <img src="assets/copy-icon.png">
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    <img src="assets/copy-icon.png">
   </MadCap:conditionalText>.<br>Or<br>Open the dashboard that you want to copy, then click <span class="bold">Dashboard Actions</span> > <span class="bold">Copy</span>.<br>The Dashboard Copy dialog box displays. All items on the original dashboard display.</p> <p> <br> </p> </li> 
 <li value="3">In the <span class="bold">Dashboard Name</span> field, specify a new name for the dashboard.</li> 
 <li value="4">To select all the items on the existing dashboard and copy them to the copied dashboard, leave <span class="bold">Select All</span> selected. By default, the reports, calendars, or lists on the existing dashboard are going to be copied to the new dashboard.<br>Or<br>To transfer only specific items from the original dashboard to the new one, deselect the items that you do not want to appear on the new dashboard, then for each selected item, choose from the following options:<br>
  <ul>
   <li><span class="bold">Make a Copy:</span> The item is copied from the original dashboard and a new version of that item is displayed on the new dashboard. Changes made to the item on the new dashboard are not reflected in the item on the original dashboard. Likewise, changes made to the item on the original dashboard are not reflected in the item on the new dashboard.<br>Use this option when you want to modify the original report on the original dashboard.<br>For example, you copy a dashboard called 'Team B' and rename it to 'Team A.' On the 'Team B' dashboard there is a report called 'Team B Report.' Because this report contains data specific to Team B, you select the option to make a copy of this report so you can customize it for Team A and rename it later to 'Team A Report'.<br>With this option, you remove the sharing permissions of the original report from the copied report. The Run this report with the Access Rights of information remains intact on the copied report.</li>
  </ul>
  <ul>
   <li><span class="bold">Use Original:</span> Displays the original item on the new dashboard. Changes made to the item on the new dashboard are also reflected in the item on the original dashboard. Likewise, changes made to the item on the original dashboard are reflected in the item on the new dashboard.<br>With this option, you keep the sharing permissions of the original report. The Run this report with the Access Rights of information remains intact as well.</li>
  </ul></li> 
 <li value="5">(Optional) Rename any items that you selected.</li> 
 <li value="6">Click <span class="bold">Copy Dashboard</span>.</li> 
 <li value="7">(Optional) If you want to edit any of the copied reports, calendars, external pages on the copied dashboard, do any of the following:<br>
  <ul>
   <li><p>To edit any information for any of the copied reports, click the report name on the dashboard, and then <span class="bold">Report Actions</span> > <span class="bold">Edit</span>.</p><p>For example, you might want to edit the View, Filter, Grouping, Prompt, or Chart or a copied report.</p></li>
   <li><p>To reinstate permissions on the copied reports, click the report name in the new dashboard, and then click <span class="bold">Report Actions</span> > <span class="bold">Sharing</span> and update the permissions on the report.</p><p>When you copy a report while copying a dashboard, the permissions on that report are removed.</p></li>
   <li><p>To modify the Run this report with the Access Rights of information, click the name of the report on the new dashboard, then <span class="bold">Report Actions</span> > <span class="bold">Edit</span> > <span class="bold">Report Options</span>.<br>After copying a report, the Run this report with the Access Rights of permissions are maintained only in the following circumstances:</p><p>(If none of these conditions are true, then Run this report with the Access Rights of permissions are removed, and the new Run this report with the Access Rights of is changed to the user who created&nbsp;the copied report.)</p><p>If the user copying the dashboard and its reports has Administrator access rights.</p>
    <ul>
     <li>If the user copying the dashboard and its reports has Administrator access rights.</li>
     <li><p>If the user copying the dashboard and its reports is currently set as the Run this report with the Access Rights of for the reports being copied.</p></li>
     <li><p>If the user copying the report has Manage permissions on the report.</p></li>
    </ul></li>
  </ul></li> 
</ol>

