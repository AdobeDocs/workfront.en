---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error Message: SAML 2.0 Authentication Failed: User Identifier Not Found"
description: When you are using SAML 2.0, the error "SAML 2.0 Authentication Failed-User Identifier Not Found" means that a UID or NAME ID is not passed from the ADFS Claim rules.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
TQID: https://experienceleague.adobe.com/YxLEE1OvD-Wo3FSd5ewXMfijsTaCjjCjzAx-EWWlBPE
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
# Error message: SAML 2.0 Authentication Failed: User Identifier Not Found

## Problem

I am receiving this error when using SAML 2.0: "SAML 2.0 Authentication Failed: User Identifier Not Found."

## Cause

This happens when a **UID** or **NAME ID** is not passed from the **ADFS Claim rules**.

In ADFS the **Relying Party Trust** needs to have a **Claim rule** that passes either a **UID** or a **NAME ID** value. When you run a **[!DNL Workfront] Test Connection**, it should show this if successful.

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

1. When editing the **[!UICONTROL ADFS INFO]**, in the **[!UICONTROL Relying Party Trusts]** > Select object >**[!UICONTROL Edit Claim Rules]**.

1. The **[!UICONTROL LDAP Attribute]** (left column) should have **[!UICONTROL E-Mail Addresses]** (or any unique identifier).

1. The **[!UICONTROL Outgoing Claim Type]** (right column) should be **[!UICONTROL Name ID]**.

   >[!NOTE]
   >
   >It does not have to have the LDAP Attribute E-Mail Addresses. Any unique identifier that will identify the user can be used but it must be passed into [!DNL Adobe Workfront] as the **NAME ID**.
