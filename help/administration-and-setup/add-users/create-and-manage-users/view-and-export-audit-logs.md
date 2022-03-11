---
filename: view-and-export-audit-logs
title: Manage audit logs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: View and export audit logs
description: You can view all audit logs in the system, or those that meet certain filtering criteria. You can also export audit logs.
---

# View and export audit logs

You can view all audit logs in the system, or those that meet certain filtering criteria. You can also export audit logs.

Audit logs list user-changes triggered in the system during the past 90 days.

For information about all the audit log types and what generates them, see [Audit logs](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> <p>You must be a <span>Workfront administrator</span>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## View audit logs

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> In the left panel, click <span class="bold">System > Audit Logs</span>.</li> 
 <li value="3"> <p> In the <span class="bold">Log Type</span> drop-down menu, select the type of audit log you want to view.<br></p> <p><span class="bold">All Log Types</span> is selected by default. </p> <p>For a list of all the audit log types you can view and the information they include, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md" class="MCXref xref">Audit logs</a>.</p> </li> 
 <li value="4"> <p> (Optional) Set any of the available filters.</p> <note type="note">
    The options in the Action Type drop-down menu vary depending on the audit log selected.
  </note> <p> <img src="assets/audit-logs-350x276.jpg" style="width: 350;height: 276;"><![CDATA[      ]]><br></p> </li> 
 <li value="5">Click <span class="bold">Apply</span>.</li> 
 <li value="6">(Optional) Click <span class="bold">Clear Filters</span> to reset changes made to the filters.</li> 
</ol>

## Export audit logs

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2"> In the left panel, click <span class="bold">System > Audit Logs</span>.<br></li> 
 <li value="3"> <p> In the <span class="bold">Log Type</span> drop-down menu, select an audit log.</p> <p><span class="bold">All Log Types</span> is selected by default.</p> </li> 
 <li value="4"> <p> Set any of the available filters, then click <span class="bold">Apply</span>.</p> <note type="important">
   You can’t export more than 50,000 logs at one time. 
   <span>Workfront</span> exports logs based on the filters you set, not the number of logs showing on the page. You can view the total number of filtered logs in the bottom-right corner of the page.
  </note> </li> 
 <li value="5"> <p>Click <span class="bold">Export</span>.</p> </li> 
</ol>

