---
filename: wp-manager-permissions-troubleshooting
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager permissions troubleshooting
description: Following are the permission profiles available in Adobe Workfront for proofing users - EDIT ME.
---

# Workfront Proof Manager permissions troubleshooting

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Following are the permission profiles available in Adobe Workfront for proofing users:

* Administrator
* Supervisor
* Manager

For detailed information about these options and how to configure them, see .

When granting a user Manager permissions, the following troubleshooting information is available:

* **PROBLEM:** Users with Manager permissions cannot view proofs created by other users. Instead, they see the Access Denied screen.&nbsp;

  ![](assets/access-denied-350x161.png)

  **SOLUTION:**&nbsp;Users with Manager permissions must be explicitly added to the proofs. Proofs should always be created via the Advanced proofing options window and users should always be added via this option.

* **PROBLEM:** Users with Manager permissions cannot add proof versions to the proofs created by other users (they could potentially submit a proof in the documents set, but the versions would NOT be connected to the original set created by another user).  
  **SOLUTION:** Users with Manager permissions can submit the versions to another user's proof only if the user with Manager permissions when both of the following :

   * Explicitly added to the proofs
   * Set as Authors (proof role) on the proofs

* **PROBLEM:** Users with Manager permissions cannot edit comments of other users on a proof they do not own or they did not create.  
  **SOLUTION:** If users with Manager permissions do not own the proofs, but they should be able to edit comments, add them as Authors (or Moderators).  
  These three types of permissions are available in Workfront for Planner, Worker, Requester, Reviewer type licenses. System Administrator or User Admin in Workfront can edit Users' profiles and adjust Workfront Proof permissions from there.&nbsp;

