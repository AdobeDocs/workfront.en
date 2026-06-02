---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domain format for Adobe Workfront API calls
description: Locate your domain for use in the Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
TQID: https://experienceleague.adobe.com/jzwKwes6zxs0KwpjFyP4VL7k2oRVx6KGUP07EQHE-gY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
    internal-label: APIs
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Domain format for Adobe Workfront API calls

When you make an API call to the Workfront API, you use your organization's domain in the call. 

The URL that you create for the API call depends on the URL that you use to connect to Workfront.

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

