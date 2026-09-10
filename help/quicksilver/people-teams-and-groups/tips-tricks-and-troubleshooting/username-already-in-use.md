---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Username Already in Use
description: Read these tips when you get an error that the username is already taken.
author: Becky
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
TQID: https://experienceleague.adobe.com/uGrOaZZzbE6CkodhE1TlCtW4rRJkfqljWGJbNSzxODc
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
# Username already in use

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
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td><p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Question

When creating a new user, a [!UICONTROL Whoops] error is displayed stating that the username is already taken. There are no other occurrences of this email in the system. Why is this being displayed?

## Solution

This can occur either because the username or email address is not unique in the current [!DNL Adobe Workfront] instance. Users can have the same username or email address in separate instances. For example, User A could have the following email addresses associated with a [!DNL Workfront] account: usera@company1.com and usera@company2.com.

>[!NOTE]
>
>The primary [!DNL Workfront] administrator can't have the same username or email address if they are in separate Workfront instances on the same cluster.   
>
>If the instances are on different clusters, the primary admin can have the same username or email address. You can view the cluster your instance is on under [!UICONTROL Setup] > [!UICONTROL System] > [!UICONTROL Customer Info].

### Check if your username is unique in your instance

Ensure that the username and email address is unique in the current [!DNL Workfront] instance:

{{step-1-to-users}}

1. In the list of people, look in the **[!UICONTROL Email]** column to ensure there are no duplicate emails.
1. Add a column for username to the view.

   1. In the **[!UICONTROL View]** drop-down menu, click **[!UICONTROL Customize View]**.
   1. Click **[!UICONTROL Add Column]**.
   1. In the search field, type *[!UICONTROL username]*.
   1. Select **[!UICONTROL User]** > **[!UICONTROL Username]**.
   1. Save the view.  
      This results in a view to display the usernames where you can look for the duplicate.

1. In the list of people, look in the **[!UICONTROL Username]** column to ensure there are no duplicate usernames.
