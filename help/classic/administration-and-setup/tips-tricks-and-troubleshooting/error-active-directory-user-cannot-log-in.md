---
filename: error-active-directory-user-cannot-log-in
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Error: Active Directory User Cannot Log In
description: A single user or only a few users are unable to Login to Adobe Workfront. They are receiving the following error - EDIT ME.
---

# Error: Active Directory User Cannot Log In

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Problem

A single user or only a few users are unable to Login to Adobe Workfront. They are receiving the following error:

Invalid Username or Password

## Cause

One likely cause of this error is that the user's name in Active Directory is not a perfect match of their Federation ID on their Workfront user.

## Solution

Check the user's name in the Active Directory and compare it to the name in the Federation ID field in the individual user's profile in Workfront.

>[!NOTE]
>
>Please note that this must be a case-sensitive match.&nbsp;

