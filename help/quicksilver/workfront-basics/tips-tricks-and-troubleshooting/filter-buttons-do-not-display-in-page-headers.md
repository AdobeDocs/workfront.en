---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filter buttons do not display in page headers
description: Read this article to troubleshoot filter buttons not displaying in page headers.
feature: Get Started with Workfront
author: Courtney
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
TQID: https://experienceleague.adobe.com/36hMJKo4unpIxvUOmBk79XlhFvFL5TgqUaoQXxrPd7c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Filter buttons do not display in page headers

## Access requirements 

+++ Expand to view access requirements for the functionality in this article.

<table>
  <tr>
   <td>Adobe Workfront package
   </td>
   <td> <p>Prime or Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront licenses
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Access level configurations
   </td>
   <td>You must be a [!DNL Workfront] administrator.
   </td>
  </tr>
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

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
