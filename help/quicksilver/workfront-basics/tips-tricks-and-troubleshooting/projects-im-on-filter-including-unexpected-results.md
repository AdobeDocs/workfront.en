---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projects I'm On filter including unexpected results
description: Read this article to troubleshoot the Projects I'm On filter including unexpected results.
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
TQID: https://experienceleague.adobe.com/xE5RW947MUFg5d2X6ikKhHSftQDUMxDJlC05un0oDH0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Projects I'm On filter includes unexpected results 

## Access requirements 

+++ Expand to view access requirements for the functionality in this article.

<table>
  <tr>
   <td>Adobe Workfront package
   </td>
   <td> <p>Prime or Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront licenses
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Access level configurations
   </td>
   <td>You must be a [!DNL Workfront] administrator.
   </td>
  </tr>
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 
 
+++


## Problem

The [!UICONTROL **Projects I'm On**] filter includes results that I would not expect, as I am not assigned or asssociated with those projects.

## Solution

The [!UICONTROL **Projects I'm On**] filter includes projects that contain the user in any of its [!UICONTROL **Project Details**] fields, including easily missed or automatically filled fields such as [!UICONTROL **Entered By**] or [!UICONTROL **Sponsor ID**]. To remove unwanted results, there are two possible solutions:

1. Check the [!UICONTROL **Project Details**] for each unexpected project included by the filter, and remove your name from all fields.

   OR

1. Try using a similar filter, such as [!UICONTROL **Projects I Own**], which only includes projects that are specifically assigned to you.

 For more information on using filters in [!DNL Workfront], see [Filters Overview](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
