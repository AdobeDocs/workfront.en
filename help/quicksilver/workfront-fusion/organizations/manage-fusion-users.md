---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Manage [!DNL Adobe Workfront] Fusion users in your organization
description: Manage [!DNL Adobe Workfront] Fusion users in your organization
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
---
# Manage [!DNL Adobe Workfront] Fusion users in your organization

&nbsp;

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

## View or edit user roles {#view}

Adobe Workfront Fusion administrators can view and update user roles.

1. While logged in as a Workfront Fusion administrator, select [!UICONTROL Users] in the left navigation.
1. Click **[!UICONTROL Details]** in the row of the user that you want to view.
1. (Optional) To update the role of the user, click the dropdown in the **[!DNL Role]** column in the row of the organization where you want to change the user's role, then select the new role.

## View or edit user details {#view2}

Adobe Workfront Fusion administrators can view and update user details.

1. While logged in as a Workfront Fusion administrator, select [!UICONTROL Users] in the left navigation.
1. Click **[!UICONTROL Details]** in the row of the user that you want to view.
1. (Optional) To update the user's details, click **Options** in the upper-right corner of the screen, then select **Change Details**.

## Delete a user {#delete}

Adobe Workfront Fusion administrators can delete users.

1. While logged in as a Workfront Fusion administrator, select [!UICONTROL Users] in the left navigation.
1. Click **[!UICONTROL Details]** in the row of the user that you want to view.
1. (Optional) To update the user's details, click **[!UICONTROL Options]** in the upper-right corner of the screen, then select **Delete**.

### Considerations when deleting a user in Workfront Fusion

* When a user is deleted, the user's connections, keys, and webhooks are removed. Any scenarios belonging to the user are transferred to the organization Owner. The connections in these scenarios must be updated, because the connections belonging to the user are no longer valid.
* If the deleted user owns any applications or public templates, the applications or public templates are transferred to the organization Owner. If there is not an organization Owner, the applications or public templates are transferred to another user.
