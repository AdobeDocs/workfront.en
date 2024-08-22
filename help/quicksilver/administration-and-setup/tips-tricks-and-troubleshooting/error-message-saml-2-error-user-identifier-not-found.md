---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error Message: SAML 2.0 Error: User Identifier Not Found"
description: You are unable to establish a successful connection to ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
---
# Error Message: SAML 2.0 Error: User Identifier Not Found

## Problem

You are unable to establish a successful connection to ADFS.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>If you establish a successful test connection and you are still experiencing issues, you might have incorrect attribute mappings or issues with the federation IDs. Contact customer support with questions.

## Cause:

Claims on the ADFS server are incorrect.

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

On the ADFS server, make sure there is a claim for name ID:

1. In Windows, click **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0 Management]**.\
   The ADFS 2.0 Management dialog box is displayed.

1. Select **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trusts]** in the left-hand pane.

1. Right-click on the relying party trust related to Adobe Workfront, and select **[!UICONTROL Edit Claim Rules]**.
1. Verify the claim has an **[!UICONTROL Outgoing Claim Type]** of **[!UICONTROL Name ID]**.

![1.png](assets/1-350x287.png)
