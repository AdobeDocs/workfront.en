---
filename: folder-permissions
content-type: reference
product: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Understand Folder Permissions in Workfront Proof
description: If a person has permission to see an item in a folder, they can also see the folder itself. However, they can see only the items in the folder that have been explicitly shared with them.
---

# Understand Folder Permissions in Workfront Proof

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

If a person has permission to see an item in a folder, they can also see the folder itself. However, they can see only the items in the folder that have been explicitly shared with them.

## Public Folders

If a folder is public, users in the account (excluding Observers and Light users) can see the folder name in the left sidebar.

Your permission profile also affects the rights you have over public folders:

| **Profile/ Action** |**See all items in folder** |**See items explicitly shared with them** |**Add items** |**Delete items** |**Add sub-folders** |**Delete sub-folders** |**Edit folder details** |
|---|---|---|---|---|---|---|---|
| **Creator** |Yes |Yes |Yes |Yes |Yes |Yes |Yes |
| **Billing Administrator** |Yes |Yes |Yes |Yes |Yes |Yes |Yes |
| &nbsp;**Administrator** |Yes |Yes |Yes |Yes |Yes |Yes |Yes |
| **Supervisor** |Yes |Yes |Yes |Yes |Yes |Yes |Yes |
| &nbsp;**Manager &#42;** |&nbsp;No |Yes |Yes |No |Yes |No |Yes |
| **Observer** |No |Yes |No |No |No |No |No |

&#42; If the public folder is owned by a manager, he or she can delete the root folder and any sub-folders.

For more information, see [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Private folders

If a folder is private, other users in the same account will not&nbsp;be able to see the name of the folder in the left sidebar unless the folder or items in the folder have been explicitly shared with them or they have a profile of Supervisor, Administrator, or Billing Administrator:

| **Profile/ Action** |**See all items in folder** |**See items explicitly shared with them** |**Add items** |**Delete items** |**Add sub-folders** |**Delete sub-folders** |**Edit folder details** |
|---|---|---|---|---|---|---|---|
| **Creator** |Yes |Yes |Yes |Yes |Yes |Yes |Yes |
| **Billing Administrator** |Yes |Yes |Yes |Yes |Yes |Yes |Yes |
| &nbsp;**Administrator** |Yes |Yes |Yes |Yes |Yes |Yes |Yes |
| **Supervisor** |Yes |Yes |Yes |Yes |Yes |Yes |Yes |
| &nbsp;**Manager &#42;** |&nbsp;No&nbsp; |Yes |No |No |No |No |No |
| **Observer &#42;&#42;** |No |Yes |No |No |No |No |No |

If, for example, you would like your Project Manager and their teams to see specific folders only, the Project Manager can set up a private folder and then share the folder with specific users.

&#42;&nbsp;When sharing a private folder, you can decide if you would like Managers to be able to create, edit, and delete folder items.

You can set this for each person individually on the New folder page and change it in the Shared with section of the Folder details page. For more information, see [Create Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)&nbsp;and [Manage Folders and their Contents in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

&#42;&#42;&nbsp;If a Private folder is shared with an or Observer, they will have Read Only access to all items in the folder. For more information, see&nbsp; [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) and&nbsp; [Share Folders in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* If a parent folder is private, all sub-folders will also be private. You cannot have a public sub-folder under a private parent folder. You can, however, have a private sub-folder under a public parent folder. 
>* The Creator and Owner of the folder will always have access to it and will not be removable. 
>* Only the Creator and Owner of the private folder can delete the folder. 
>

