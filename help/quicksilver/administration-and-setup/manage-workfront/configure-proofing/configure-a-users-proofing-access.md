---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configure a User's Proofing Access
description: As a Adobe Workfront administrator or Workfront Proof administrator, you can configure a user's access to create and view proofs in Workfront and Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
---
# Configure a user's proofing access

As a Adobe Workfront administrator or Workfront Proof administrator, you can configure a user's access to create and view proofs in Workfront and Workfront Proof.

For information about proofing functionality available for basic and integrated proofing, see [Access to proofing functionality in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront administrator or Workfront Proof administrator. For information on Workfront administrators, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Enable and disable proofing for a user (legacy plans only) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

If your organization is using a legacy Select or Premium Workfront Plan, as a Workfront administrator, you can enable and disable proofing functionality for the user.

When you enable proofing for a user, Workfront enables the option for the user's proofs to generate automatically.

Though you can enable a user as a proofing user, he or she must have Administrator permissions in order to navigate directly to the Workfront Proof interface from the Workfront Main Menu. For information about how you can enable this option for all proofing users in your Workfront system, see [Configure Workfront Proof access via Workfront Main Menu for all users](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. In the **Main Menu**, select **Users**.

1. Select a user, then click the **Edit** icon.
1. In the **Access** section, select or deselect **User can generate proofs**.

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
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
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

## Configure Workfront Proof access via Workfront Main Menu for all users {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

By default, only users with administrative rights within Workfront can access Workfront Proof as described  [Access Workfront Proof from Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

You can grant all users access to the Workfront Proof button within the Workfront Main Menu by contacting Workfront Support and submitting a request.

>[!IMPORTANT]
>
> If you plan to allow all Workfront users to access Workfront Proof directly from the Workfront Global Navigation Bar, ensure that the permission profile for each user does not provide more access than the user's access level within Workfront. This prevents users from accessing proofs within Workfront Proof that they cannot access within Workfront. For more information, see [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configure user access to the Desktop Proofing Viewer

If the users in your organization would prefer to use the Desktop Proofing Viewer instead of the Web Proofing Viewer to review interactive content, you can configure the Desktop Proofing Viewer to launch automatically when users open interactive content proofs. For information about this the Desktop Proofing Viewer and how it differs from the Web Proofing Viewer, see [Understand the Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) and [Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. From Workfront, click the Workfront Proof icon in the Global Navigation Bar to access Workfront Proof.

   ![](assets/proof-access-proofhq-350x39.png)

1. Click **Account settings** near the upper-right corner of Workfront Proof, then click the **Settings** tab.

1. Under **Proof Defaults**, at the end of the **Desktop Proofing Viewer for Interactive proofing** row, click **Setup**.

1. Modify the Desktop Proofing Viewer settings, as described in [Desktop Proofing Viewer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) in the article [Configure proof settings for your organization](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Click **Save**.

## Configure custom devices for interactive proofs

You can add any custom devices to your system, allowing users to review interactive content and simulate how the content appears on a specific device when they are using the Desktop Proofing Viewer. (This functionality is not available in the Web Proofing Viewer, where users can review interactive content, but only as it appears in various resolutions, not on various devices.)

For more information, see [Change interactive proof resolution in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. From Workfront, access the Workfront Proof interface, as described in [Access Workfront Proof from Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modify the Desktop Proofing Viewer settings, as described in [Configure custom devices for proofs](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) in the article [Configure proof settings for your organization](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
