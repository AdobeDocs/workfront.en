---
filename: configure-a-users-proofing-access
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configure a user's proofing access
description: The sections in this article shouldn't be lumped together.
---

# Configure a user's proofing access

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">The sections in this article shouldn't be lumped together. </p>
-->

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> -------------Also, need to add a bit of info to the bottom section about how you can view interactive content in screen sizes but not emulated.</p>
-->

As a Adobe Workfront administrator or Workfront Proof administrator, you can configure a user's access to create and view proofs in Workfront and Workfront Proof.

For information about proofing functionality available for basic and integrated proofing, see [Access to proofing functionality in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront administrator or Workfront Proof administrator. For information on Workfront administrators, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Enable and disable proofing for&nbsp;a user (legacy plans only) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

If your organization is using a legacy Select or Premium Workfront Plan, as a Workfront administrator, you can enable and disable proofing functionality for the user.

When you enable proofing for a user, Workfront enables the option for the user's proofs to generate automatically. For more information about this option and how to disable it, see [Configure a user's proofing access](#).&nbsp;

Though you can enable a user as a proofing user, he or she must have Administrator permissions in order to navigate directly to the Workfront Proof interface from the Workfront Main Menu. For information about how you can enable this option for all proofing users in your Workfront system, see [Configure Workfront Proof access via Workfront Main Menu for all users](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. In the **Main Menu**, select **Users**.

1. Select a user, then click the **Edit** icon.
1. In the **Access** section, select or deselect **User can generate proofs**.

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Users** ![](assets/users-icon-in-main-menu.png). 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile**&nbsp;drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).&nbsp;

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p>Note:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's&nbsp;Access Level&nbsp;setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher&nbsp;access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in&nbsp;<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes**&nbsp;to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront.&nbsp;For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's&nbsp;permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront.&nbsp;This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see&nbsp; [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)&nbsp;in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront&nbsp;only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for&nbsp;proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

## Configure Workfront Proof access via Workfront Main Menu for all users {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

By default, only users with administrative rights within Workfront can access Workfront Proof as described&nbsp; [Access Workfront Proof from Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

You can grant all users access to the Workfront Proof button within the Workfront Main Menu by contacting Workfront Support and submitting a request.

>[!IMPORTANT]
>
>&nbsp;If you plan to allow all Workfront users to access Workfront Proof directly from the Workfront Global Navigation Bar,&nbsp;ensure that the permission profile for each user does not provide more access than the user's access level within Workfront. This prevents users from accessing proofs within Workfront Proof that they cannot access within Workfront. For more information, see [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="configuring-whether-users-can-access-the-html5-proofing-viewer"></a>Configure user access to Web Proofing Viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Web Proofing Viewer launches by default when users in your organization proof video and static content.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the Workfront administrator, if your organization opted to use the Legacy proofing viewer as the default until it is removed, you can switch the default for your users to the Web Proofing Viewer.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You might not have access to the Legacy proofing viewer because it is supported by Flash, which has been deprecated in most environments.</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p>From Workfront, click the Workfront Proof icon in the Global Navigation Bar to access Workfront Proof.</p> <p> <img src="assets/proof-access-proofhq-350x39.png" alt="" style="width: 350;height: 39;"> </p> </li>
<li value="2">Click <strong>Account settings</strong> near the upper-right corner of Workfront Proof, then click the <strong>Settings</strong> tab.</li>
<li value="3">Under <strong>Proof Defaults</strong>, at the end of the <strong>New Proofing Viewer for video and static proofs</strong> row, click <strong>Setup</strong>.</li>
<li value="4">Modify the Web Proofing Viewer settings, as explained under <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#web-proofing-viewer" class="MCXref xref">Web Proofing Viewer</a> in the article <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md" class="MCXref xref">Configure proof settings for your organization</a>.</li>
<li value="5">Click <strong>Save</strong>.&nbsp;</li>
</ol>
-->

## Configure user access to the Desktop Proofing Viewer

If the users in your organization would prefer to use the Desktop Proofing Viewer instead of the Web Proofing Viewer to review interactive content, you can configure the Desktop Proofing Viewer to launch automatically when users open interactive content proofs.&nbsp;For information about this the Desktop Proofing Viewer and how it differs from the Web Proofing Viewer, see [Understand the Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) and [Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. From Workfront, click the Workfront Proof icon in the Global Navigation Bar to access Workfront Proof.

   ![](assets/proof-access-proofhq-350x39.png)

1. Click **Account settings** near the upper-right corner of Workfront Proof, then click the **Settings** tab.

1. Under **Proof Defaults**, at the end of the **Desktop Proofing Viewer for Interactive proofing**&nbsp;row, click **Setup**.

1. Modify the Desktop Proofing Viewer settings, as described in [Desktop Proofing Viewer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) in the article [Configure proof settings for your organization](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Click **Save**.

## Configure custom devices for interactive proofs

You can&nbsp;add any custom devices to your system, allowing users to review interactive content and simulate how the content appears on a specific device when they are using the Desktop Proofing Viewer. (This functionality is not available in the Web Proofing Viewer, where users can review&nbsp;interactive content, but only as it appears in various resolutions, not on various devices.)

For more information, see [Change interactive proof resolution in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. From Workfront, access the Workfront Proof interface, as described in [Access Workfront Proof from Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modify the Desktop Proofing Viewer settings, as described in [Configure custom devices for proofs](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) in the article [Configure proof settings for your organization](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).****

