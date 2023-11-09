---
content-type: api
navigation-topic: api-navigation-topic
title: Ending support for JSONP
description: Ending support for JSONP
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
---
# Ending support for JSONP

Because JSONP (Javascript with Padding) is an old standard with known security vulnerabilities, Adobe Workfront will no longer support JSONP as of November 2018. This decision supports our larger initiative to modernize the Workfront platform.

JSONP is a standard by which cross-origin or cross-site requests can be performed. Many Workfront customers and partners use JSONP to access Workfront from a system on their own domain as part of an integration. JSONP allows for requests from non-Workfront domains to be processed by the Workfront application.

If you are using JSONP as part of any of your Workfront integrations, you must update your integration to use the CORS (Cross-Origin Resource Sharing) standard. This update requires you to do the following:

1. Submit a request with the Workfront support team to have any domains that are being used to make cross-origin requests to our allowlist. 
 
   To have your domains added to the allowlist for CORS, contact Workfront Customer Support at 844-306-HELP(4357) or by submitting a support ticket online.

   >[!NOTE]
   >
   >Adding domains to the allowlist for CORS is supported only for customers who were using JSONP prior to August 1, 2018.

    
1. Make changes to your integration code to use CORS.
