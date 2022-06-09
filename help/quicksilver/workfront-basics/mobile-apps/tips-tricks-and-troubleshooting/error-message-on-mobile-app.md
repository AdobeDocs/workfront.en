---
filename: error-message-on-mobile-app
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: "Error Message on the Adobe Workfront Mobile App: 'Your account is not API enabled.'"
description: If you see the error "Your account is not API enabled" on the mobile app, talk to your system administrator.
---

# Error Message on the Adobe Workfront Mobile App: "Your account is not API enabled."

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
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

