---
title: Configure a Custom Help URL
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: If you create a custom internal help site containing information about how your organization uses Workfront, you can configure the Main Menu Help icon to go to that site.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d2b63508-1943-4f9e-888e-8f1bfb54c33e
TQID: https://experienceleague.adobe.com/sQ0-5jDNs4Pr8icC-mYCp0QFec5g1i-e0XkTz78WEWQ
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
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Configure a custom help URL

If you create a custom internal help site containing information about how your organization uses Workfront, you can configure the Main Menu Help icon to go to that site.

 ![Custom help button](assets/custom-help-with-left-menu.png)

This does not affect the context-sensitive help links throughout Workfront, which take users to the Workfront Help site.

For information about how users access both a custom help URL that you configure in Workfront and the regular Workfront help site, see [Access Adobe Workfront help](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/access-workfront-help.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System Administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure a custom help URL

{{step-1-to-setup}}

1. Click **System** > **Preferences**.
1. In the **General preferences** section, in the **Custom Help URL** field, type the URL where your custom help site is located.

   If your custom help location requires login credentials, those credentials are required for users when they access the site from Workfront. The credentials to your custom help site might need to be managed separately from the Workfront credentials if you are not using Single Sign-On (SSO).

1. Click **Save**.

   Once you have saved a custom help URL, you can return to using the default Workfront help site by deleting the custom URL and clicking **Save**.
