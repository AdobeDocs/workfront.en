---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Bulk edit user's Other Groups
description: When bulk editing I attempted to add a single Other Groups to numerous users. After Saving Changes, all the existing Other Groups were removed and only the new Other Group remained.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
TQID: https://experienceleague.adobe.com/oH--gAyZgNsSf-HBHUs7TSZxW3jAktySyvZx-wNlpG0
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Bulk edit user's Other Groups

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

## Problem:

When bulk editing I attempted to add a single Other Groups to numerous users.
After Saving Changes, all the existing Other Groups were removed and only the new Other Group remained.

## Answer:

The resulting behavior depends on the current group membership of the selected users:

* If all of the selected users Other Groups memberships match exactly...
   After you select the users and select [!UICONTROL edit], the [!UICONTROL Other Groups] field will show the full listing
   of all of the groups these users belong to.

* If the selected users have different Other Group memberships...
   After you select the users and click [!UICONTROL Edit], the [!UICONTROL Other Groups] field will be blank.

When you click **[!UICONTROL Save Changes]**, whatever is showing in the Other Groups field is saved.

The previous contents of the field are overwritten.
