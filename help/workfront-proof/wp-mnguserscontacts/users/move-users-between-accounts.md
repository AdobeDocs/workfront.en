---
filename: move-users-between-accounts
product: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: Move Users Between Accounts using Workfront Proof
description: If you are a Workfront Proof administrator and you have one or more satellite accounts connected to your main account, you can move the users between all these accounts.
---

# Move Users Between Accounts using `Workfront Proof`

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product `Workfront Proof`. For information on proofing inside `Adobe Workfront`, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

If you are a `Workfront Proof administrator` and you have one or more&nbsp;satellite accounts connected to your main account, you can move the users between all these accounts.

## Moving Users Between Connected Accounts

<ol> 
 <li value="1">Click <span class="bold">Settings</span> > <span class="bold">Account settings</span>.</li> 
 <li value="2">Open the <span class="bold">Users</span> tab.</li> 
 <li value="3">Click the <span class="bold">Move user</span>&nbsp;icon (1). <img src="assets/move-user2-350x95.png" alt="Move_user2.png" style="width: 350;height: 95;"></li> 
 <li value="4">In&nbsp;the Move user box that appears, confirm the&nbsp;user you want to move (1).</li> 
 <li value="5">Select a destination account from&nbsp;the connected accounts list (2).</li> 
 <li value="6">Assign the&nbsp;profile permission (3) that&nbsp;this user should have on the new account.</li> 
 <li value="7">Select a user (4) who should take ownership of&nbsp;the items that won't be moved. <br>This includes the items that you will decide to leave on the old account and the items that can't be moved (see <a href="https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can't-be-moved">Items That Can't Be Moved</a> below).</li> 
 <li value="8">Check the checkboxes if you want to move the <span>proofs</span> (5)&nbsp;and files (6)&nbsp;along with the user.</li> 
 <li value="9">Create a name for the folder (7) in which all the moved items will be placed on the new account.</li> 
 <li value="10">Click <span class="bold">Move user</span> (8) to start the&nbsp;process.<br><img src="assets/moving-users-pop-up-350x380.png" alt="Moving_users_pop-up.png" style="width: 350;height: 380;"></li> 
</ol>

If you choose to move the user without their `proofs` and files then this action will be performed straight away. If you choose to move the user along with their `proofs` and files, the user's profile will be reassigned straight away, but the `proofs` and files will be gradually appearing on the destination account as this operation requires time to transfer the data.

Depending on the number of files and `proofs` moving process&nbsp;may take anything from a few minutes up to a few hours.

>[!NOTE]
>
>If you suspect that the process takes longer than expected or the moved `proofs` and / or files don't appear&nbsp;on the new account, please contact&nbsp;our Support team.

## Items That Can't be Moved

###  Folders Created or Owned by the Moved User

Due to the nature of various permissions applied&nbsp;to folders and its contents (e.g., they may be shared with other users and accounts) we are unable to move folder structures with the user.

If a folder is owned by the moved user, ownership will be transferred to the selected user (4) in the "Move user" pop-up.&nbsp;

>[!NOTE]
>
>&nbsp;If a folder has been created by the moved user ,they will remain its creator - only the ownership will be transferred. The&nbsp;folder will be remain&nbsp;visible to the moved user in the sidebar of their new account. The moved user will still have "Read Only" access to the items placed inside these&nbsp;folders.

If you don't want the moved user to keep such&nbsp;permissions or the moved user does not want to see their old folders on&nbsp;the old&nbsp;account, the solution here would be to delete the folders as follows:

1. Create a new folder on the old&nbsp;account.
1. Move all the items from the moved user's folders to the newly created one.
1. Delete all the folders left by the moved user.

### Sets of Versions With Different Owners

If a `proof` has a few versions and each of them is owned by a different user the versions owned by the moved user will not be moved along. Ownership of such versions will be transferred on to another&nbsp;user as per your choice (4) in the Move user box. (For more information, see .)

>[!NOTE]
>
>A moved user needs to own all the `proof` versions in the set in order for the `proof` to be moved along.

### Groups

Groups will need to be re-created by the moved user on their new account. For more information, see [Create Proofing Groups using Workfront Proof](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).&nbsp;

### Custom Views

Personal&nbsp;Custom views&nbsp;will need to be re-created by the moved user on their new account. For more information, see [Create and Manage Custom Views in Workfront Proof Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### Custom Fields

Custom Fields cannot be moved and data from custom fields will be lost, so make sure you generate the reports on the required items prior to the move.

### Automated Workflow Templates

Automated Workflow Templates need to be recreated on the new account, but the stages will be retained on the moved `proofs` created with the templates.

### Actions on Comments

Actions on Comments will remain on the `proofs`, but it will not be possible to filter by them any more. Solution would be to create matching Actions on the new account and re-flag the comments with the new actions if needed.
