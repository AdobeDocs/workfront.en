---
filename: filter-buttons-do-not-display-in-page-headers
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filter buttons do not display in page headers
description: You must have the following access to perform the steps in this article - EDIT ME.
---

# Filter buttons do not display in page headers

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
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
   <td>Adobe Workfront area</td> 
   <td>Filter buttons</td> 
  </tr> 
  <tr> 
   <td> <p>Projects </p> </td> 
   <td> 
    <ul> 
     <li> <p>Projects I'm On</p> </li> 
     <li> <p>Projects I Own</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>Timesheets</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>My Timesheet Approvals</span> </p> </li> 
     <li> <p><span>My&nbsp;Timesheets</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

The filter buttons in the Projects and ```Timesheets``` area do not display because the corresponding filters are not included in the layout template applied to the user. The Workfront administrator must assign a layout template that includes the filters.

>[!NOTE]
>
>Sometimes the filters are removed from the List Controls area in Setup. The Workfront administrator must include them in the lists in this area for them to be available in the layout templates.&nbsp;For information, see [Edit list controls: filters, views, and groupings](../../administration-and-setup/manage-workfront/configure-reports/edit-list-controls-filters-views-groupings.md).

1. Verify that the layout template displays the following filters:

   * Projects I'm On and Projects I Own in the Projects area
   * My Timesheet Approvals and My&nbsp;Timesheets in the Timesheet area&nbsp;

   To do this:

   1. Access the layout template.
   1. Select **Lists** under **Customize what users see**.
   1. Select **Projects** or ```Timesheets``` under **Select a list to customize**.
   1. In the **Filter** section, verify that **Projects I'm On**, **Projects I Own** (for projects) and ```**My Timesheet Approvals** and **My Timesheets** (for timesheets)``` are selected.
   1. Click **Save**.

   For more information, see [Customize Filters, Views, and Groupings using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Assign the layout template to the correct users, job roles, teams, or groups. For information, see [Assign users to a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

