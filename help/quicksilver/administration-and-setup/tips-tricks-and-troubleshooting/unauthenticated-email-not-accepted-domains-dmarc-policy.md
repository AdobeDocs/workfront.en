---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Unauthenticated Email Is Not Accepted Due to Domain's DMARC Policy
description: If an email sent from the [!DNL Workfront] system is not accepted due to domain's DMARC policy, your email administrator can fix the problem by configuring your email system to allow all email from workfront.com.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
---
# Unauthenticated email is not accepted due to domain's DMARC policy

## Issue

[Test] I received the following bounce back email:

550-5.7.1 Unauthenticated email from "customer domain.com" is not accepted due to\
550-5.7.1 domain's DMARC policy. Please contact administrator of "customer domain.com"\
550-5.7.1 domain if this was a legitimate mail. Please visit\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) to learn about DMARC\
550 5.7.1 initiative.

## Solution

DMARC is configured in your company's email system and is not part of [!DNL Adobe Workfront]. If you receive this email, you need to contact your email administrator.

Your email administrator should configure your email system to allow/trust email from noreply@workfront.com or preferably all email from workfront.com.

For more information about DMARC, see [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
