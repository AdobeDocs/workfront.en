---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: List users with a proofing license in Adobe Workfront
description: You can view which users in Adobe Workfront currently have the option "User can generate proofs" enabled in either of the following ways below.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
TQID: https://experienceleague.adobe.com/9P5Bp9TrJ1ECSwpK7C4AW4rQlTQOBH4U7-CPYl92RKU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
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
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
