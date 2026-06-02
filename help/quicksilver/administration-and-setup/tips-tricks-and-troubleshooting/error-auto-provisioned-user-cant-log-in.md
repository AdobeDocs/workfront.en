---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error: Auto-Provisioned User Can't Log In"
description: If an auto-provisioned user tries to log in for the first time and receives an error saying that the system is not assigning them an access level, this might be because your system lacks access levels that are associated with the Request license.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
TQID: https://experienceleague.adobe.com/jUBGb9lqH9QL34Rw-oEhjty3l3wAf8avcLgtVe1-VSg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Error: Auto-provisioned user can't log in

When an auto-provisioned user tries to log in for the first time, they receive the following error:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problem

The system is not assigning the new user an access level.

By default, auto-provisioning uses the Request license type. When no access levels with a Request license exists, the system cannot assign the user an access level.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

Create a basic access level with a Request license:

1. Go to **[!UICONTROL Setup]** > **[!UICONTROL Access Levels]**.

1. Click **[!UICONTROL New Access Level]**.
1. Enter a **[!UICONTROL Name]**.
1. In the **[!UICONTROL License Type]** drop-down menu, select Request.
1. Click **[!UICONTROL Save Changes]**.

After you create an access level with a Request license, have the user log in with their SSO credentials.


