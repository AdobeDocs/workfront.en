---
filename: proof-state
product: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Understand Proof State in Workfront Proof
description: In Workfront Proof, proofs exist in different states. These states determine what actions you can take on the proof, such as commenting or making decisions.
---

# Understand Proof State in `Workfront Proof`

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product `Workfront Proof`. For information on proofing inside `Adobe Workfront`, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

In `Workfront Proof`, `proofs` exist in different states. These states determine what actions you can take on the `proof`, such as commenting or making decisions.

## Understanding Proof State

The four states are as follows:

* [Active](#active) 
* [Locked](#locked) 
* [Draft (Dropzone only)](#draft) 
* [Submitted (Dropzone only)](#submitted)

### Active

Proofs that are uploaded to `Workfront Proof` through the New Proof page or the Dropzone appear as Active ``after they are processed. When a `proof` is active users can review, make comments, and make decisions on the `proof`.

>[!NOTE]
>
>Proofs that are uploaded through the Dropzone appear as Active only if the Activate `proof` on submission ``option is enabled. If the option is not enabled, you must manually activate the `proof`.

For more information about Dropzone settings, see [Configure the dropzone in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Locked

You can lock a `proof` when you finish reviewing it. Locking a `proof` means no more comments or decisions can be made on the `proof`, but the `proof` can still be opened.&nbsp;

Any users with Edit rights on the `proof` can unlock it.&nbsp;

For more information about rights, see [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>Email notifications no longer send when a `proof` is locked. For example, if a `proof` is locked before its deadline, a notification email is not sent when the deadline is reached.

### Draft (Dropzone only)

When you submit a `proof` through the Dropzone, it goes into the Draft ``state before the admin activates it. When it is in the draft zone, you cannot take any actions on the `proof`.&nbsp;

### Submitted (Dropzone only)

After a draft is activated by the admin, your `proof` shows as Submitted ``in the Dropzone. After it is submitted, you can take actions on the `proof`.

## Viewing and Changing Proof State

For information about viewing a list of all `proofs` in a specific state, such as viewing all Active ``or Locked `proofs`, see [Manage Items on the Views Page in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) in the article [Manage Items on the Views Page in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

<ol> 
 <li value="1"> <p> Access your <span>Workfront Proof</span> Dashboard.<br></p> <p>For more information, see&nbsp;<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> </li> 
 <li value="2"> <p>On the <span class="bold">Dashboard,</span>&nbsp;click the&nbsp;<span class="bold">Expand&nbsp;</span>arrow next to the <span>proof</span> you want to view or change the state of.<br></p> <p> <img src="assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png" style="width: 350;height: 85;"> <br> </p> <p>The&nbsp;<span class="bold">Workflow process&nbsp;</span>section appears.<br></p> <p> <img src="assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png" style="width: 350;height: 226;"> <br> </p> </li> 
 <li value="3">View the&nbsp;<span class="bold">State&nbsp;</span>in the&nbsp;<span class="bold">Workflow process.</span></li> 
 <li value="4"> <p>(Optional) To change the state, mouse over the current&nbsp;<span class="bold">State&nbsp;</span>and click the drop-down menu, then select a new state.<br></p> <p> <img src="assets/screen-shot-2018-05-02-at-11.35.30-am.png"> </p> </li> 
</ol>

