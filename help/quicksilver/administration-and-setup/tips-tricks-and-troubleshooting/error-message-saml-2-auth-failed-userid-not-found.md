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
---
# Error message: SAML 2.0 Authentication Failed: User Identifier Not Found

## Problem

I am receiving this error when using SAML 2.0: "SAML 2.0 Authentication Failed: User Identifier Not Found."

## Cause

This happens when a **UID** or **NAME ID** is not passed from the **ADFS Claim rules**.

In ADFS the **Relying Party Trust** needs to have a **Claim rule** that passes either a **UID** or a **NAME ID** value. When you run a **[!DNL Workfront] Test Connection**, it should show this if successful.

## Access requirements

You must have the following access to perform the steps in this article:

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>You must be a [!DNL Workfront] administrator. </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

1. When editing the **[!UICONTROL ADFS INFO]**, in the **[!UICONTROL Relying Party Trusts]** > Select object >**[!UICONTROL Edit Claim Rules]**.

1. The **[!UICONTROL LDAP Attribute]** (left column) should have **[!UICONTROL E-Mail Addresses]** (or any unique identifier).

1. The **[!UICONTROL Outgoing Claim Type]** (right column) should be **[!UICONTROL Name ID]**.

   >[!NOTE]
   >
   >It does not have to have the LDAP Attribute E-Mail Addresses. Any unique identifier that will identify the user can be used but it must be passed into [!DNL Adobe Workfront] as the **NAME ID**.
