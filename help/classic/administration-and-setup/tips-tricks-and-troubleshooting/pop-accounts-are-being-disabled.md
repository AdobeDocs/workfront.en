---
filename: pop-accounts-are-being-disabled
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: POP accounts are being disabled
description: Replies made via a POP email account are not received by Adobe Workfront or a user can no longer create issues using a POP email account address. The Workfront administrator looks at the request queue or setup area and finds that the POP email account is disabled.
---

# POP accounts are being disabled

>[!IMPORTANT]
>
>Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the new Workfront experience as soon as possible.

## Problem

Replies made via a POP email account are not received by Adobe Workfront or a user can no longer create issues using a POP email account address. The Workfront administrator looks at the request queue or setup area and finds that the POP email account is disabled.&nbsp;

## Cause

The following are potential causes of this problem:

* After making 25 failed attempts to connect to the POP account, Workfront disables the POP account.&nbsp;
* After a period of&nbsp;12 hours without being&nbsp;able to connect to the POP&nbsp;account, Workfront disables the POP account.
* Workfront connects to the POP account and finds ten emails that are not&nbsp;related to comments in Workfront. In this case, Workfront stops&nbsp;processing emails to the account and sends a notification to the Workfront administrator that says:  
  "We encountered a problem while processing emails from your POP account: <POP email address>. We either found emails that are not related to Workfront comments, or something might be wrong with your POP credentials. Please ensure that the email credentials configured under Setup > Email > Setup are valid and that the email address is used only for Workfront communication."  
  Workfront starts checking the account again, after five minutes.

  >[!TIP]
  >
  >Workfront recommends users use their POP account for Workfront communication only. Any other emails could potentially disable the connection between Workfront and the&nbsp;POP account.

  &nbsp;

## Solution

The following are potential solutions to this problem:

* Verify the username and password to the POP account are correct. Oftentimes a password for a POP account is changed as part of a company's security policy, but not changed in Workfront. Ensure that the passwords for both the POP account and Workfront are the same.
* Verify the ports being used to connect to the POP account.
* Use the Workfront feature of sending a test email to check if the functionality is working correctly.&nbsp;

To learn more about configuring Workfront to work with a POP account, see .
