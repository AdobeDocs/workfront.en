---
title: Group table rows in Reporting Canvas
description: Group table rows in Reporting Canvas
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 355bbe5b-9c66-4b6b-b479-a48a20b53fe6
---
# Group table rows in Reporting Canvas

You can organize the information in a report by displaying it in groups defined by currency, date, percentage, text, and time fields.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta. For more information, see [Reporting Canvas Beta](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>The contents of this article are available as part of a beta program that must be joined by a Workfront administrator. After joining, the Workfront administrator may then grant access to other users in their environment. For more information on participating in the beta and granting access to users, see <a href="/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md" class="MCXref xref">Reporting Canvas beta</a>.</p> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit access to create reports, calendars, and dashboards</p>
    --> <!--
     <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Group rows in a table

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Reporting**.
1. Click **New report**.

   Or

   Go to an existing report, click the **More Menu** icon ![](assets/more-icon.png) in the report header, then select **Edit**.

1. To group rows on a new table, drag or double-click a table block onto the canvas.

   Or

   To group rows on an existing table, click the **Edit** icon ![](assets/edit-icon.png) in the table header.

1. In the right panel, locate a field that you want to group by and drag it to the **Group** section.

   You can use the **Search** box to find a specific group. 

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   For more information, see [Link]
   </MadCap:conditionalText>
   -->

1. In the drop-down menu to the right of the **Group** field, select how you would like the group to be sorted.

   The options vary based on the type of field you are using to group your rows.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Currency</td> 
      <td> 
       <ul> 
        <li> <p>Smallest to largest</p> <p>Largest to smallest</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date</td> 
      <td> 
       <ul> 
        <li> <p>Oldest to newest</p> </li> 
        <li> <p>Newest to oldest</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percent</td> 
      <td> 
       <ul> 
        <li> <p>Smallest to largest</p> </li> 
        <li> <p>Largest to smallest</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Text</td> 
      <td> 
       <ul> 
        <li> <p>A to Z</p> </li> 
        <li> <p>Z to A</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Time</td> 
      <td> 
       <ul> 
        <li> <p>Smallest to largest</p> </li> 
        <li> <p>Largest to smallest</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Do any of the following:

   * To add another group, drag another field from the side panel.
   * To display rows in a group collapsed by default, click the **More menu** icon ![](assets/more-icon.png) next to the group, then click **Collapse group**.

     Each group can be individually configured to display with rows collapsed or expanded. By default, all grouped rows are collapsed.
   
   * To display a count in the group row, click the **More menu** icon ![](assets/more-icon-27x15.png) next to the group, then click **Display count**.
   * To remove a group, click the **More menu** icon ![](assets/more-icon.png) next to the group, then click **Remove group**.
   * To rearrange multiple groups you have created, drag them ![](assets/move-icon---dots.png)into a new order.
