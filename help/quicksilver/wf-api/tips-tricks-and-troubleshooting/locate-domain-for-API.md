---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domain format for Adobe Workfront API calls
description: Locate your domain for use in the Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
---

# Domain format for Adobe Workfront API calls

When you make an API call to the Workfront API, you use your organization's domain in the call. The format for this domain URL differs based on whether your organization has been onboarded to the Adobe Unified Shell.

To know whether your organization is on the Adobe Unified Shell, examine the URL that displays when you are viewing a Workfront page.

| Workfront URL begins with: | URL for API calls: |
|---|---|
|`<yourdomain>.my.workfront.com`|`<yourdomain>.my.workfront.com`|
|`experience.adobe.com`|`<yourdomain>.my.workfront.adobe.com`|

To locate your domain: 

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Select **System**, then select **Customer Info**.
   
   Your domain is listed on the right of the screen.

   ![Domain](assets/domain.png)