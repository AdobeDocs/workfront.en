---
filename: wp-manager-permissions-troubleshooting
content-type: tips-tricks-troubleshooting
product: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager permissions troubleshooting
description: Following are the permission profiles available in Adobe Workfront for proofing users:
---

# `Workfront Proof` Manager permissions troubleshooting

Following are the permission profiles available in `Adobe Workfront` for `proofing` users:

* Administrator
* Supervisor
* Manager

For detailed information about these options and how to configure them, see [Configure a user's proofing access](../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

When granting a user Manager permissions, the following troubleshooting information is available:

<ul> 
 <li><span class="bold">PROBLEM:</span> Users with Manager permissions cannot view <span>proofs</span> created by other users. Instead, they see the Access Denied screen.&nbsp;<a href="../../Resources/Images/Getting Started/Tips, Tricks, and Troubleshooting/Access_Denied.png" class="MCXref xref" xrefformat="{para}"><img src="assets/access-denied.png" alt="" width="1296" height="595"><br></a><span class="bold">SOLUTION:</span>&nbsp;Users with Manager permissions must be explicitly added to the <span>proofs</span>. Proofs should always be created via the Advanced <span>proofing</span> options window and users should always be added via this option.</li> 
</ul>

* `PROBLEM:` Users with Manager permissions cannot add `proof` versions to the `proofs` created by other users (they could potentially submit a `proof` in the documents set, but the versions would NOT be connected to the original set created by another user).  
  `SOLUTION:` Users with Manager permissions can submit the versions to another user's `proof` only if the user with Manager permissions when both of the following :

  * Explicitly added to the `proofs`
  * Set as Authors ( `proof` role) on the `proofs`

* `PROBLEM:` Users with Manager permissions cannot edit comments of other users on a `proof` they do not own or they did not create.  
  `SOLUTION:` If users with Manager permissions do not own the `proofs`, but they should be able to edit comments, add them as Authors (or Moderators).  
  These three types of permissions are available in `Workfront` for Planner, Worker, Requester, Reviewer type licenses. System Administrator or User Admin in `Workfront` can edit Users' profiles and adjust `Workfront Proof` permissions from there.&nbsp;

