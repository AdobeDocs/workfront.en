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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, and Calendars</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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

1. Go to **Reporting**, then click the **Dashboards** subtab. 

1. Select the dashboard that you want to copy, then click **Copy** .  
   Or  
   Open the dashboard that you want to copy, then click **Dashboard Actions** > **Copy**.  
   The Dashboard Copy dialog box displays. All items on the original dashboard display.

   ![](assets/copy-dashboard-350x348.png)

1. In the **Dashboard Name** field, specify a new name for the dashboard.
1. To select all the items on the existing dashboard and copy them to the copied dashboard, leave **Select All** selected. By default, the reports, calendars, or lists on the existing dashboard are going to be copied to the new dashboard.  
   Or  
   To transfer only specific items from the original dashboard to the new one, deselect the items that you do not want to appear on the new dashboard, then for each selected item, choose from the following options:

   * **Make a Copy:** The item is copied from the original dashboard and a new version of that item is displayed on the new dashboard. Changes made to the item on the new dashboard are not reflected in the item on the original dashboard. Likewise, changes made to the item on the original dashboard are not reflected in the item on the new dashboard.  
     Use this option when you want to modify the original report on the original dashboard.  
     For example, you copy a dashboard called 'Team B' and rename it to 'Team A.' On the 'Team B' dashboard there is a report called 'Team B Report.' Because this report contains data specific to Team B, you select the option to make a copy of this report so you can customize it for Team A and rename it later to 'Team A Report'.  
     With this option, you remove the sharing permissions of the original report from the copied report. The Run this report with the Access Rights of information remains intact on the copied report.

   * **Use Original:** Displays the original item on the new dashboard. Changes made to the item on the new dashboard are also reflected in the item on the original dashboard. Likewise, changes made to the item on the original dashboard are reflected in the item on the new dashboard.  
     With this option, you keep the sharing permissions of the original report. The Run this report with the Access Rights of information remains intact as well.

1. (Optional) Rename any items that you selected.
1. Click **Copy Dashboard**.
1. (Optional) If you want to edit any of the copied reports, calendars, external pages on the copied dashboard, do any of the following:

   * To edit any information for any of the copied reports, click the report name on the dashboard, and then **Report Actions** > **Edit**.

     For example, you might want to edit the View, Filter, Grouping, Prompt, or Chart or a copied report.
   
   * To reinstate permissions on the copied reports, click the report name in the new dashboard, and then click **Report Actions** > **Sharing** and update the permissions on the report.

     When you copy a report while copying a dashboard, the permissions on that report are removed.
   
   * To modify the Run this report with the Access Rights of information, click the name of the report on the new dashboard, then **Report Actions** > **Edit** > **Report Options**.  
     After copying a report, the Run this report with the Access Rights of permissions are maintained only in the following circumstances:

     (If none of these conditions are true, then Run this report with the Access Rights of permissions are removed, and the new Run this report with the Access Rights of is changed to the user who created&nbsp;the copied report.)

     If the user copying the dashboard and its reports has Administrator access rights.

      * If the user copying the dashboard and its reports has Administrator access rights.
      * If the user copying the dashboard and its reports is currently set as the Run this report with the Access Rights of for the reports being copied.
      * If the user copying the report has Manage permissions on the report.

