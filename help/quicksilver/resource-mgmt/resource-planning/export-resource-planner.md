---
product-area: resource-management
navigation-topic: resource-planning
title: Export Information from the Resource Planner
description: You can export information from any view of the Resource Planner to an Excel (.xlsx) file which is saved on your computer.
author: Lisa
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
---
# Export information from the Resource Planner

You can export information from any view of the Resource Planner to an Excel (.xlsx) file which is saved on your computer.

>[!IMPORTANT]
>
>There are limitations in what information displays and what information you can export from the Resource Planner. For information on these limitations, see [Resource Planner display limitations](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>New: Any</p>
       <p>or</p>
       <p>Current: Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Light or higher</p>
       <p>or</p>
       <p>Current: Review or higher</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View access or higher to Projects, Users, and Resource Management</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher for projects</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Export information from the Resource Planner

{{step1-to-resourcing}}

   The **Planner** displays by default.

1. Select the view for the Planner. You can select one of the following options:

   * View by User 
   * View by Project 
   * View by Role

1. Click **Export**. 

   The Export Options dialog box displays.

   ![](assets/rp-export-options-box-350x421.png)

1. Specify the following information:  
   **Start Date**: The start date of your export. The exported file contains allocation and availability information starting with the first day of the week which contains the day you specify here.   
   **Number of Periods**: The number of time periods you want to include in your file. The default is 4 periods.  
   **Type**: The type of time periods by which you want to display the information in the exported file (weeks, months, or quarters.)   
   The following are the maximum time periods that you can export:

   * 52 weeks 
   * 36 months 
   * 12 quarters

   **Select to Export**: Depending on which view you selected, you can select to export the availability and budgeting information for either all the objects listed on the screen or for specific ones.
   You can select to export the following information:

   * In the Project View, select to export:

      * Projects
      * Projects and Roles
      * Everything (this is the default option)

   * In the User View, select to export:

      * Users
      * Users and Projects
      * Everything (this is the default option)

   * In the Role View, select to export:

      * Roles
      * Roles and Projects
      * Everything (this is the default option)

   **Data Formatting**: Depending on how you want your Excel file to be displayed, select the following options:

   * **Raw**: Select to display the availability and allocation information ungrouped by the objects it belongs to in the Excel file. (this is the default option)
   * **Grouped**: Select to display the availability and allocation information grouped by the objects it belongs to. This displays the exported information as it appears on the screen.

   A sample of how the information looks in the exported file is shown in the Export Options dialog box.

1. Click **Export** to export the information from the Resource Planner.  
   Only the information that you saved is exported.  

1. (Conditional) If you have unsaved Budgeted Hours in the Role or Project views, click **Save and Continue.** 
   An Excel (.xlsx) file is downloaded to your computer.  
   Exporting from the Resource Planner is unavailable while the file is prepared for downloading.  
   (Conditional) If you export a large amount of data, you receive an email with a link where you can download the file.  
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Conditional) When you receive the email with the exported file, click **Download** to download the file.  
   This takes you back to Workfront where you can download the file.   
   You must be logged into Workfront for the download to complete.  
   If you do not download the file when it is delivered, the Download link remains active for 7 days after you initiate the export.
