---
filename: unauthenticated-email-not-accepted-domains-dmarc-policy
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Unauthenticated email is not accepted due to domain's DMARC policy
description: [Test]I received the following bounce back email - EDIT ME.
---

# Unauthenticated email is not accepted due to domain's DMARC policy

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

##  Issue

[Test]I received the following bounce back email:

550-5.7.1 Unauthenticated email from "customer domain.com" is not accepted due to  
550-5.7.1 domain's DMARC policy. Please contact administrator of "customer domain.com"  
550-5.7.1 domain if this was a legitimate mail. Please visit  
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) to learn about DMARC  
550 5.7.1 initiative.&nbsp;

## Solution

DMARC is configured in your company's email system and is not part of Adobe Workfront. If you receive&nbsp;this email, you need to contact your email administrator.

Your email administrator should configure your email system to allow/trust email from noreply@workfront.com or preferably all email from workfront.com.

For more information about DMARC, see&nbsp; [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
