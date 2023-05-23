---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filter buttons do not display in page headers
description: Read this article to troubleshoot filter buttons not displaying in page headers.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
---
# Filter buttons do not display in page headers

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] license</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

The following filter buttons do not display in their respective areas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] area</strong></td> 
   <td><strong>Filter buttons</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projects] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects I'm On]</p> </li> 
     <li> <p>[!UICONTROL Projects I Own]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Timesheets]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL My Timesheet Approvals]</span> </p> </li> 
     <li> <p><span>[!UICONTROL My Timesheets]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

The filter buttons in the [!UICONTROL Projects and Timesheets] area do not display because the corresponding filters are not included in the layout template applied to the user. The [!DNL Workfront] administrator must assign a layout template that includes the filters.

>[!NOTE]
>
>Sometimes the filters are removed from the [!UICONTROL List Controls] area in [!UICONTROL Setup]. The [!DNL Workfront] administrator must include them in the lists in this area for them to be available in the layout templates.

1. Verify that the layout template displays the following filters:

   * [!UICONTROL Projects I'm On] and [!UICONTROL Projects I Own] in the [!UICONTROL Projects] area
   * [!UICONTROL My Timesheet Approvals] and [!UICONTROL My Timesheets] in the [!UICONTROL Timesheet] area 

   To do this:

   1. Access the layout template.
   1. Select **[!UICONTROL Lists]** under **[!UICONTROL Customize what users see]**.
   1. Select **[!UICONTROL Projects]** or **[!UICONTROL Timesheets]** under **[!UICONTROL Select a list to customize]**.
   1. In the **[!UICONTROL Filter]** section, verify that **[!UICONTROL Projects I'm On]**, **[!UICONTROL Projects I Own]** (for projects) and **[!UICONTROL My Timesheet Approvals]** and **[!UICONTROL My Timesheets]** (for timesheets) are selected.
   1. Click **[!UICONTROL Save]**.

   For more information, see [Customize Filters, Views, and Groupings using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Assign the layout template to the correct users, job roles, teams, or groups. For information, see [Assign users to a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
