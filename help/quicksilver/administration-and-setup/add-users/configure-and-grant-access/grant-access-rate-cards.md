---
title: Grant Access to Financial Data
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: As an Adobe Workfront administrator, you can define a user's access to financial data in Workfront through their access level.
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
---

# Grant access to rate cards

{{highlighted-preview-article-level}}

As an Adobe Workfront administrator, you can define a user's access to rate cards through the user's access level, as explained in [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

For information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations for granting access to rate cards

Consider the following when granting users access to rate cards in Workfront:

* Users must have Edit access to Rate Cards, Projects, and Financial Data to attach a rate card to a project.
* Users with No Access to Rate Cards and Edit access to Financial Data can't attach a rate card to a project, but they can edit other billing rates on the project that came from other sources.

## Configure user access to rate cards using a custom access level

1. Begin creating or editing the access level, as explained in [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Click the gear icon ![](assets/gear-icon-settings.png) on the **View** or **Edit** button to the right of Rate Cards, then select the abilities you want to grant under **Fine-tune your settings**.

   ![Fine-tune rate card access](assets/rate-card-access-fine-tune.png)

1. (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) such as [Grant access to tasks](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. When you are finished, click **Save**.

   After the access level is created, you can assign it to a user. For more information, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Access to shared rate cards

You can share a rate card with other users by granting them permissions to it, as explained in [Share a rate card](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md).

When you share any object with another user, the recipient's rights on it are determined by a combination of two things:

* The permissions that you grant to your recipient for the object
* The recipient's access level settings for the object's type
