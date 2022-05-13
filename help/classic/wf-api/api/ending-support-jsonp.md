---
filename: ending-support-jsonp
content-type: api
navigation-topic: api-navigation-topic
title: Ending support for JSONP
description: Because JSONP (Javascript with Padding) is an old standard with known security vulnerabilities, Adobe Workfront will no longer support JSONP as of November 2018. This decision supports our larger initiative to modernize the Workfront platform.
---

# Ending support for JSONP

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Because JSONP (Javascript with Padding) is an old standard with known security vulnerabilities, Adobe Workfront will no longer support JSONP as of November 2018. This decision supports our larger initiative to modernize the Workfront platform.

JSONP is a standard by which cross-origin or cross-site requests can be performed. Many Workfront customers and partners use JSONP to access Workfront from a system on their own domain as part of an integration. JSONP allows for requests from non-Workfront domains to be processed by the Workfront application.

If you are using JSONP as part of any of your Workfront integrations, you must update your integration to use the CORS (Cross-Origin Resource Sharing) standard. This update requires you to do the following:

1. Submit a request with the Workfront support team to have any domains that are being used to make cross-origin requests to our allowlist.

   To have your domains added to the allowlist for CORS, please contact Workfront Customer Support at 844-306-HELP(4357) or by submitting a support ticket online.

   >[!NOTE]
   >
   >Adding domains to the allowlist for CORS is supported only for customers who were using JSONP prior to August 1, 2018.

1. Make changes to your integration code to use CORS.
