---
filename: accounts-merge-process
product: workfront-proof
product-area: documents;system-administration
navigation-topic: account-administration
title: Accounts merge process
description: This document outlines the tasks involved in processing merge and split requests for the following data migrations:
hidefromtoc: true
---

# Accounts merge process

This document outlines the tasks involved in processing merge and split requests for the following data migrations:

* From one standalone proofing instance to another standalone proofing instance
* From a standalone proofing instance to an integrated proofing instance

These tasks can minimize the impact of merge and split requests both to our customers and to various teams at Workfront.

## Processing merge and split requests for proof data migrations

>[!IMPORTANT]
>
>To streamline the merge process and reduce its impact to customers and Workfront teams, all migration requests should be completed outside the client’s working hours.

1. The Customer Support engineer registers each data merge request as a ticket in Salesforce and informs an Account Executive (AE) of the request.
1. The Customer Support engineer creates a merge request in Hub under the Proof accounts migrations project.

   This allows us to queue customers who want to migrate and mitigate the impact.

1. The AE liaises with the client to do the following:

   * Confirm that the client's license plan eligibility to make sure that it accommodates licenses for the users and data being moved from the origin account.

   * Make sure that plan renewal or upgrade is in place before the merge is completed.

1. The __________ works with the client using the information in this article under [Information to analyze with the client](#information-to-analyze-with-the-client)
1. Once all information from step 4 is confirmed, the __________ sets the Merge date and arranges Development Team support.
1. The ___________ uses the template under [Merge process template](#merge-process-template) in this article to analyze the original and destination accounts.
1. The ___________ analyzes both the origin and destination accounts using the template under [Merge process template](#merge-process-template) later in this article.
1. The Adobe Workfront Support team moves all folders and loose items to the top folder on the original account.
1. The Workfront developer team scans folder structure on the original account.
1. The Workfront Support team deactivates email notifications for both accounts on the account level from the Proofing backend.
1. If needed, the Workfront Support team increases the number of user licensee on the destination account.
1. The Workfront Support team moves users along with their proofs, retaining the users' permissions or changing them if requested by the client.

   If asked to set a user for data that can not be moved, the Workfront Support team selects a Power User as a new owner.

1. The Workfront Support team moves the Power User to be the last user.
1. The Workfront Support team moves all the leftover items from the original account.

   If needed, assign this to the Power User.

1. Once all the items are moved, the Workfront developer team runs the Folder recreation script on the destination account and assigns _________ to the Power User.
1. The Workfront Support team checks account consistency on the destination account and does a final cleanup, if necessary.
1. The Workfront Support team removes user folders when empty.
1. The Workfront Support team enables email notifications on the destination account.
1. __________ confirms the merge with the customer and updates the relevant task in the Hub project.

## Information to analyze with the client {#information-to-analyze-with-the-client}

In step 4 above, the __________ goes over the information below with the client:

During the migration, we move users along with the proofs they own. Proof ownership is retained as long as all versions in the proof set are owned by a single user. No comments, decisions, or proof recipients are lost. All proof recipients retain their proof access as per proof sharing.

### Regarding any data lost during the migration

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Custom Fields</td> 
   <td> <p>We are currently not able to pull Custom Fields data from the client's original account to the destination account. However, we can generate an Excel/CSV report containing all the proof fields values, if needed.</p> <p>The Workfront development team will complete this prior the merge.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Automated Workflow templates</td> 
   <td> <p>The client must re-create these on the destination account, but all moved proofs will keep their Automated Workflows.</p> <p>The client will complete this after the merge.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions on comments</td> 
   <td> <p>Actions applied on the original account will still be visible on comments after the merge, but it will not be possible to filter by those actions because the actions IDs will not match the actions from the destination account. One solution could be to create matching actions on the destination account and apply new actions to the comments after the move.</p> <p>The client will complete this after the merge.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folders</td> 
   <td> <p>We re-create folder structure upon the content move, but privacy setting, sharing, and folder ownership is lost. Currently, the structure upon move can be assigned to a single owner only.</p> <p>The client completes this after the merge.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Contacts</td> 
   <td>We do not migrate the Contacts list, but the client can easily export it from the account import it to the destination account at any time. Also, we automatically add all recipients to the list as the proofs are shared with them.</td> 
  </tr> 
 </tbody> 
</table>

### Regarding users

* All moved users will keep their current credentials and the move will not cause any interruption. We will perform the move outside the users working hours to minimize any potential impact.
* The client must provide a list of users that should be deleted.
* The client must provide a list of users that should be moved and the profile permissions that should be assigned to each one. This will determine what access and visibility levels users will have on the destination account.
* The client must select a power user on the original account to oversee the folder structure and any outstanding proofs identified during the move.

## Merge process template {#merge-process-template}

In step 6 above, the __________ can use the following template to analyze the original and destination accounts:

### XXX account merge into XXX account

**Date**:

#### **Checklist**

* Has a power user been appointed to be the folder structure owner on destination account?

  YES/NO

* Does the client need an Excel/CSV report report for Custom Fields?

  YES/NO

* Which branding remains?
* Has the client created matching Actions on Comments on the destination account and applied new Actions on Comments to the comments after the move?

  YES/NO

* Has the client specified which users should be deleted? and which should be moved?

  YES/NO

* Has the client specified which users should be moved and indicated the permissions that should be assigned to each one?

  YES/NO

#### **Original account - XXX**

* Proof backend ID: https://app.proofhq.com/backend.php/organisation/XXX ```[Tatev, can we change the spelling to the American "organization"?]```
* Current plan: _______________________
* Number of active users: _______
* Number of deactivated users: _______
* Domain name: ______________________
* AW templates: If yes, how many: _______
* Actions on comments:

  YES/NO

* Custom Fields:

  YES/NO

* Folders:

  YES/NO

* Custom Views:

  YES/NO

* Power user ID: _________________

#### Destination account - XXX

* Proof backend ID: https://app.proofhq.com/backend.php/organisation/XXX ```[same question as above]```
* Current plan: _______________________
* Number of active users: _______
* Number of deactivated users: _______
* Domain name: ______________________
* AW templates: If yes, how many: _______
* Actions on comments:

  YES/NO

* Custom Fields:

  YES/NO

* Folders:

  YES/NO

* Custom Views:

  YES/NO

