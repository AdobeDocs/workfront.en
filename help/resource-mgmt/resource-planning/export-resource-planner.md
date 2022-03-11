---
filename: export-resource-planner
product-area: resource-management
navigation-topic: resource-planning
title: Export information from the Resource Planner
description: You can export information from any view of the Resource Planner to an Excel (.xlsx) file which is saved on your computer.
---

# Export information from the `Resource Planner`

You can export information from any view of the `Resource Planner` to an Excel (.xlsx) file which is saved on your computer.

>[!IMPORTANT]
>
>There are limitations in what information displays and what information you can export from the `Resource Planner`. For information on these limitations, see [Resource Planner display limitations](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> and higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Review</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to&nbsp;Projects, Users, and Resource Management</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher for projects</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Export information from the `Resource Planner`<![CDATA[		]]>

<ol> 
 <li value="1"><![CDATA[
				]]><![CDATA[
			]]>Click the Main Menu icon in the upper-right corner of Adobe Workfront.</li> 
 <li value="2"><![CDATA[
			]]> Click Resourcing. The Planner displays by default.</li> 
 <li value="3"> Select the view for the Planner. You can select one of the following options: 
  <ul>
   <li> View by User </li>
   <li> View by Project </li>
   <li> View by Role </li>
  </ul></li> 
 <li value="4"> <p> Click <span class="bold">Export</span>. </p>The Export Options dialog box displays.<span class="preview"><br><img src="assets/rp-export-options-box-350x421.png" style="width: 350;height: 421;"></span><br></li> 
 <li value="5"> Specify the following information:<br><span class="bold">Start Date</span>: The start date of your export. The exported file contains allocation and availability information starting with the first day of the week which contains the day you specify here. <br><span class="bold">Number of Periods</span>: The number of time periods you want to include in your file. The default is 4 periods.<br><span style="font-size: small;" class="bold">Type</span>: The type of time periods by which you want to display the information in the exported file (weeks, months, or quarters.) <br> The following are the maximum time periods that you can export: 
  <ul>
   <li> 52 weeks </li>
   <li> 36 months </li>
   <li> 12 quarters</li>
  </ul><p><span class="bold">Select to Export</span>: Depending on which view you selected, you can select to export the availability and budgeting information for either all the objects listed on the screen or for specific ones.</p>You can select to export the following information:
  <ul>
   <li>In the Project View, select to export:
    <ul>
     <ul>
      <li>Projects</li>
      <li>Projects and Roles</li>
      <li>Everything (this is the default option)</li>
     </ul>
    </ul></li>
   <li>In the User View, select to export:
    <ul>
     <ul>
      <li>Users</li>
      <li>Users and Projects</li>
      <li>Everything (this is the default option)</li>
     </ul>
    </ul></li>
   <li>In the Role View, select to export:
    <ul>
     <li>Roles</li>
     <li>Roles and Projects</li>
     <li>Everything (this is the default option)</li>
    </ul></li>
  </ul><span class="bold">Data Formatting</span>: Depending on how you want your Excel file to be displayed, select the following options:
  <ul>
   <li><span class="bold">Raw</span>: Select to display the availability and allocation information ungrouped by the objects it belongs to in the Excel file. (this is the default option)</li>
   <li><span class="bold">Grouped</span>: Select to display the availability and allocation information grouped by the objects it belongs to. This displays the exported information as it appears on the screen.</li>
  </ul>A sample of how the information looks in the exported file is shown in the Export Options dialog box.</li> 
 <li value="6"> Click <span class="bold">Export</span> to export the information from the <span>Resource Planner</span>.<br>Only the information that you saved is exported.<br></li> 
 <li value="7"> (Conditional) If you have unsaved Budgeted Hours in the Role or Project views, click <span class="bold">Save and Continue.</span> <br>An Excel (.xlsx) file is downloaded to your computer.<br>Exporting from the <span>Resource Planner</span> is unavailable while the file is prepared for downloading.<br>(Conditional) If you export a large amount of data, you receive an email with a link where you can download the file.<br><img src="assets/rp-eamil-with-exported-planner-attached-350x116.png" alt="RP_eamil_with_exported_planner_attached.png" style="width: 350;height: 116;"></li> 
 <li value="8">(Conditional) When you receive the email with the exported file, click <span class="bold">Download</span> to download the file.<br>This takes you back to <span>Workfront</span> where you can download the file. <br>You must be logged into <span>Workfront</span> for the download to complete.<br>If you do not download the file when it is delivered, the Download link remains active for 7 days after you initiate the export.</li> 
</ol>

