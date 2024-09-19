---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: List users with a proofing license in Adobe Workfront
description: You can view which users in Adobe Workfront currently have the option "User can generate proofs" enabled in either of the following ways below.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
---
# List users with a proofing license in Adobe Workfront

You can view which users in Adobe Workfront currently have the option "User can generate proofs" enabled in either of the following ways below.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

+++

## Create a user report

You can create a user report&nbsp;to view which users can generate proofs:

1. Navigate to **Reporting** area.
1. Click the&nbsp;**New Report**&nbsp;drop-down menu, then click&nbsp;**User Report**.

1. On the **Filters** tab, click **Add a Filter Rule**.

1. In the available field, expand **User**, then click **Has Proof License**.

1. Select **Equal** > **True**.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Click **Save+Close**.

   The report displays all users in Workfront who have a proofing license assigned to them.

## Update the People view

You can add a new column in the People view to view which users can generate proofs:

1. Go to the **People**&nbsp;area.
1. Click the **People** tab.
1. In the **View** drop-down menu, do either of the following:

   * To add this information to an existing view, select the view you want to customize,&nbsp;then click **Customize View**.
   * To add this information to a new view, click **New View**.

1. Click **Add Column**.
1. In the available field, expand **User**, then click **Has Proof License**.

1. Click **Done**, then click **Save View** or **Save as New View**.

   The view displays **True** or **False** depending on whether the user has a proofing license assigned to them.
