---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: External User License Type Missing from Access Levels
description: I can no longer see External User license type under Access Levels in Setup.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
---
# External user license type missing from access levels

## Problem

I can no longer see External User license type under Access Levels in Setup.

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

1. Go to **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Preferences]**.

1. In the **[!UICONTROL Security]** section, ensure the option **[!UICONTROL Collaborate with people without Workfront accounts by using their email address]** is enabled.

   If this option is not enabled, the external user does not appear in Access Level Setup.
