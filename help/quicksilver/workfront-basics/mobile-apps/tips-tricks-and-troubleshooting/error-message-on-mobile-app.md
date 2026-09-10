---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: "Error Message on the [!DNL Adobe Workfront] Mobile App: 'Your account is not API enabled.'"
description: "Error Message on the [!DNL Adobe Workfront] Mobile App: 'Your account is not API enabled.'"
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
TQID: https://experienceleague.adobe.com/t-ANxgXpzPBSM8cGUipyAIczqSEUJGXTthbaVP5dh2E
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
---
# Error Message on the [!DNL Adobe Workfront] Mobile App: "[!UICONTROL Your account is not API enabled.]"

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] license</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>[!UICONTROL System administrator] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

When trying to log in to the [!DNL Adobe Workfront] mobile app, you receive the following error: *[!UICONTROL Your account is not API enabled. Let your system admin know and they'll get you set up. Sorry about that.]*

## Cause

Your [!DNL Workfront] administrator has not enabled your [!DNL Workfront] environment to be accessed from a mobile device.

## Solution

1. Log into the [!DNL Workfront] web application as a [!DNL Workfront] Administrator.
1. Go to the **[!UICONTROL Setup]** area.
1. Expand the **[!UICONTROL System]** menu, then click **[!UICONTROL Preferences]**.

1. Under the **[!UICONTROL Security]** section, select the **[!UICONTROL Let people use [!DNL Workfront]'s mobile applications]** option to enable it. 

1. Click **[!UICONTROL Save]**.\
   All users in the system can now access [!DNL Workfront] from their mobile apps.
