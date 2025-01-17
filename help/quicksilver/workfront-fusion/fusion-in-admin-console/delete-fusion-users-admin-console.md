---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Delete users through the Adobe Admin Console
description: The Adobe Workfront Fusion documentation has moved to a new location. This article has been deprecated, but contains a link to the new article that covers this functionality.
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a

---
# Delete users through the [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>The Adobe Workfront Fusion documentation has moved to a new location. 
>
>The information in this article can now be found in the article:
>
>* [Delete users through the Adobe Admin Console](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/manage-users-and-teams/delete-users-admin-console.html)
>
>Please update any bookmarks.
>
>This article is no longer being updated, and will be removed in the near future.

>[!IMPORTANT]
>
>The functionality in this article is available only if your organization's instance of [!DNL Adobe Workfront Fusion] has been onboarded to the [!DNL Adobe Business Platform].
>
>For a list of procedures that differ based on whether your organization has been onboarded to the [!DNL Adobe Business Platform], see [Platform-based administration differences ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

You can remove a user from [!DNL Adobe Workfront Fusion] only, leaving access to any other [!DNL Adobe] product profiles, or you can remove the user from the [!DNL Adobe Admin Console] entirely.

## Delete a user in [!DNL Adobe Workfront Fusion]

To delete a user in [!DNL Adobe Workfront Fusion], you must deactivate the user through the [!DNL Adobe Admin Console].

A user is deactivated from the [!DNL Adobe Admin Console] when one of the following applies:

* The user is moved out from a product or product profile, and are not assigned to any other product or product profile.
* The user is removed from a group that is linked to a product profile, and is not included in any other group linked to a product profile.
* The user is removed from a product profile and is not assigned to another product profile.
* The user is deleted or deactivated in the organization that includes Workfront Fusion.

  For instructions, see the section "Remove users" in [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

In [!DNL Workfront Fusion], the deactivation affects the user in one of the following ways:

* If the user is in only one organization, the user is deactivated.
* If the user is in more than one organization, the user is removed from the organization that the user was modified in on the [!DNL Adobe Admin Console].
* For other considerations when deleting a user in [!DNL Workfront Fusion], see [Considerations when deleting a user in [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
