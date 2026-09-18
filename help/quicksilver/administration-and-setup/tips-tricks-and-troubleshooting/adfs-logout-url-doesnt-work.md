---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS Logout URL Doesn't Work
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
TQID: https://experienceleague.adobe.com/RRaLL70JcSBcvoS6EUFuWj5Ejwljekt4QuQ3kXDx-44
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
# ADFS logout URL doesn't work

<!-- Audited: 1/2024 -->

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>The procedure described on this page applied only to organizations that were not yet onboarded to the [!UICONTROL Adobe Admin Console].
>
>Because all organizations have now been onboarded to the Adobe Admin Console, this article will be removed in the near future.
>
>If your organization has been onboarded to the [!UICONTROL Adobe Admin Console], see [Platform-based administration differences ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problem

When using the ADFS logout URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), you receive a message page with the error: "There was a problem accessing the site. Try to browse to the site again."

If the problem persists, contact the administrator of this site and provide the following reference number to identify the problem: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] package</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td>  
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

1. In your ADFS manager server, go to **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trusts]** > `<your party trust>` properties.

1. Under the **[!UICONTROL Endpoints]** tab, click **[!UICONTROL Add]**.

1. **[!UICONTROL Endpoint Type]** = SAML Logout, Binding = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   You can set a response URL if you want it to redirect to another page. But we recommend the ADFS site because it warns that you are logged off, but you should still close your browser.
