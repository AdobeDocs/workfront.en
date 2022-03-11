---
filename: projects-filter-buttons-not-appearing
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projects I'm On and Projects I Own filter buttons do not appear on the Projects page header
description: The Projects I'm On and Projects I Own filter buttons do not appear in the page header of the Projects list.
---

# Projects I'm On and Projects I Own filter buttons do not appear on the Projects page header

## Problem

The `Projects I'm On` and `Projects I Own` filter buttons do not appear in the page header of the Projects list.

## Access requirements

You must have the following access to perform the steps in this article:

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
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

The project filter buttons are not included in the default layout template. The `Workfront administrator` must assign a layout template that includes the buttons.

1. Verify that the layout template displays the filter buttons:

  1. Access the layout template.
  1. Select `Lists` under `Customize what users see`.
  
  1. Select `Projects` under `Select a list to customize`.
  
  1. In the Filter section, verify that `Projects I'm On` and `Projects I Own` are selected.
  
  1. Click `Save`.  
     For more information, see [Customize Filters, Views, and Groupings using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Assign the layout template to the correct users, job roles, teams, or groups. For information, see [Assign users to a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

