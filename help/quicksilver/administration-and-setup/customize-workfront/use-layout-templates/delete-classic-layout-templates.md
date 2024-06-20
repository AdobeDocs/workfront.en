---
title: Delete Classic Layout Templates
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Layout templates from the Classic Workfront experience are not longer available in the Workfront interface, but may still affect Workfront data. This can cause inconsistencies in fields affected by layout templates (such as Shared with) on reports or dashboards.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
---
# Grant administrative access for a layout template

Layout templates from the Classic Workfront experience are not longer available in the Workfront interface, but may still affect Workfront data. This can cause inconsistencies in fields affected by layout templates (such as Shared with) on reports or dashboards.

You can resolve these inconsistencies by deleting the Classic layout templates. Since they are not available in the Workfront interface, use must use the Workfront API to delete them.

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Delete the Classic layout templates using an API call

You can enter API calls into the URL bar of your browser and press enter. The API response is displayed in your browser.

>[!NOTE]
>
>Global and System layout templates cannot be deleted.

1. Log in to Workfront.
1. Locate the layout template you want to delete using the following API call:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Make note of the ID of the layout template you want to delete. 
1. Locate your session ID using the following API call:
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Never share your session ID with anyone. 

1. Insert the layout template ID and the session ID into the following API call:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Paste the API call from step 4 into the URL bar of your browser and press Enter.

   This deletes the layout template.
