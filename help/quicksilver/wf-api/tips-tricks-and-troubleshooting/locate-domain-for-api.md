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

When you make an API call to the Workfront API, you use your organization's domain in the call. The format for this domain URL differs based on whether your organization has been onboarded to the Adobe Unified Shell.

To know whether your organization is on the Adobe Unified Shell, examine the URL that displays when you are viewing a Workfront page.

| Workfront URL begins with: | URL for API calls: |
|---|---|
|`experience.adobe.com`|`<yourdomain>.my.workfront.adobe.com`|

## Access requirements 

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++


To locate your domain: 

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Select **System**, then select **Customer Info**.
   
   Your domain is listed on the right of the screen.

   ![Domain](assets/domain.png)

