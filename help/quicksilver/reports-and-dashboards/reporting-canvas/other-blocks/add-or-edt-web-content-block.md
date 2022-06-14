---
product-area: reporting
navigation-topic: other-blocks
title: Add or edit a web content block in Reporting Canvas
description: Web content blocks allow you to display information from external websites directly within your report.
feature: Reports and Dashboards
---

# Add or edit a web content block in Reporting Canvas

Web content blocks allow you to display information from external websites directly within your report.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta. For more information, see [Reporting Canvas Beta](../../../product-announcements/betas/reporting-canvas-beta.md).

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
   <td> <p>The contents of this article are available as part of a beta program that must be joined by a Workfront administrator. After joining, the Workfront administrator may then grant access to other users in their environment. For more information on participating in the beta and granting access to users, see <a href="../../../product-announcements/betas/reporting-canvas-beta.md" class="MCXref xref">Reporting Canvas beta</a>.</p> <!--
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

## Add or edit a web content block

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click**Reporting**.
1. Click **New report**.

   Or

   Go to an existing report, click the **More** icon ![](assets/more-icon-27x15.png) in the report header, then click **Edit**.

1. On the right side of the screen, under **Add a Block**, either:

   Drag the **Web content** icon onto the canvas directly to your desired location.

   Or

   Double-click the **Web content** icon to add a block to the top of the canvas.

   >[!TIP]
   >
   >You can change the size of the block after it is placed by dragging its corner handles.

1. Click **Untitled web content** in the block header, then type a title for the block.
1. Click the **Edit** icon ![](assets/edit-icon.png) in the block header.

   ![](assets/web-content-block-header-350x76.png)

1. In the **Settings** panel that opens, enter the complete URL for the page that you would like to display (including "https://") in the **URL** field.

   >[!IMPORTANT]
   >
   >Currently, only sites from select domains are able to be displayed. The domains that can currently be used are:
   >
   >   
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com
   >   
   >

   A warning displays below your entered URL if it is unable to be embedded. These warnings include:

   | Warning name |Reason |
   |---|---|
   | Invalid URL |The entered URL does not return a valid site. |
   | Provider site restrictions |The site that you are trying to embed is not allowed. |

   {style="table-layout:auto"}

1. (Optional) Click the **Pass Parameters** toggle to open a list of available pass parameters.

   >[!IMPORTANT]
   >
   >Pass parameters are currently disabled.

1. Click **Embed URL** to save your selections and return to your report.

