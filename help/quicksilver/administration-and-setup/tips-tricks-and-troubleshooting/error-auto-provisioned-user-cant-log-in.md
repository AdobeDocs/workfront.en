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


