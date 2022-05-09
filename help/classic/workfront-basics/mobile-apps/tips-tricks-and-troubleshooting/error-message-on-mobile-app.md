---
filename: error-message-on-mobile-app
content-type: tips-tricks-troubleshooting
product: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: "Error Message on the Adobe Workfront Mobile App: "Your account is not API enabled.""
description: You must have the following access to perform the steps in this article - EDIT ME.
---

# Error Message on the Adobe Workfront Mobile App: "Your account is not API enabled."

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

When trying to log in to the Adobe Workfront mobile app, you receive the following error: *Your account is not API enabled. Let your system admin know and they'll get you set up. Sorry about that.*

## Cause

Your Workfront administrator has not enabled your Workfront environment to be accessed from a mobile device.

## Solution

1. Log into the Workfront web application as a Workfront Administrator.
1. Go to the **Setup** area.
1. Expand the **System** menu, then click **Preferences**.

1. Under the **Security** section, select the **Let people use Workfront's mobile applications and the Workfront Outlook Add-In**&nbsp;option to enable it.&nbsp;

1. Click **Save**.  
   All users in the system can now access Workfront from their mobile apps, and from Outlook.

