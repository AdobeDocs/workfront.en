---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Error: Active Directory User Cannot Log In'
description: If someone receives the message "Invalid Username or Password" when trying to log in to Adobe Workfront, it's possible that the user's name in Active Directory doesn't match their Federation. Compare the user's name in the Active Directory to the name in the Federation ID field in the individual user's profile.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: afea757b-4d9f-40c1-ad23-9ba01258ac7c
---
# Error: Active Directory User Cannot Log In

## Problem

A single user or only a few users are unable to Login to Adobe Workfront. They are receiving the following error:

Invalid Username or Password

## Cause

One likely cause of this error is that the user's name in Active Directory is not a perfect match of their Federation ID on their Workfront user.

## Solution

Check the user's name in the Active Directory and compare it to the name in the Federation ID field in the individual user's profile in Workfront.

>[!NOTE]
>
>Please note that this must be a case-sensitive match.
