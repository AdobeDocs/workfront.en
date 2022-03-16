---
filename: bulk-edit-users-other-groups
content-type: tips-tricks-troubleshooting
product: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Bulk edit user's Other Groups
description: When bulk editing I attempted to add a single Other Groups to numerous users. After Saving Changes, all the existing Other Groups were removed and only the new Other Group remained.
---

# Bulk edit user's Other Groups

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

## Problem:&nbsp;

When bulk editing I attempted to add a single Other Groups to numerous users.  
After Saving Changes, all the existing Other Groups were removed and only the new Other Group remained.&nbsp;

## Answer:

The resulting behavior depends&nbsp;on the current group membership of the selected users:

* If all of the selected users Other Groups memberships match exactly...  
  After you select the users and select edit, the Other Groups field will show the full listing  
  of all of the groups these users belong to.&nbsp;

* If the selected users have different Other Group memberships...  
  After you select the users and click Edit, the Other Groups field will be blank.

When you click `Save Changes`, whatever is showing in the Other Groups field is saved.

The previous contents of the field are overwritten.&nbsp; 
