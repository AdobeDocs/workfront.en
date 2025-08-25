---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domain format for Adobe Workfront API calls
description: Locate your domain for use in the Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
---
# Domain format for Adobe Workfront API calls

When you make an API call to the Workfront API, you use your organization's domain in the call. 

The URL that you create for the API call depends on the URL that you use to connect to Workfront.

| Workfront URL begins with: | URL for API calls: |
|---|---|
|`<yourdomain>.my.workfront.com`|`<yourdomain>.my.workfront.com`|
|`experience.adobe.com`|`<yourdomain>.my.workfront.adobe.com`|

To locate your domain: 

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Select **System**, then select **Customer Info**.
   
   Your domain is listed on the right of the screen.

   ![Domain](assets/domain.png)

