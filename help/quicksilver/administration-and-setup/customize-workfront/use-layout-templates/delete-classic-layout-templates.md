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
TQID: https://experienceleague.adobe.com/AcxOFTyZbrQakRoeBlslCoLJgrgY4HS41vaYLOx5i-I
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Delete Classic layout templates

Layout templates from the Classic Workfront experience are not longer available in the Workfront interface, but may still affect Workfront data. This can cause inconsistencies in fields affected by layout templates (such as Shared with) on reports or dashboards.

You can resolve these inconsistencies by deleting the Classic layout templates. Since they are not available in the Workfront interface, use must use the Workfront API to delete them.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.</p>
        <p>To perform them for a group, you must be a manager of that group.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

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
