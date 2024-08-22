---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configure Proof Settings for Your Organization
description: As an Adobe Workfront administrator or Workfront Proof administrator, you can customize the default proof settings for your organization. These settings include default sharing options, branding, and more.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
---
# Configure proof settings for your organization

As an Adobe Workfront administrator or Workfront Proof administrator, you can customize the default proof settings for your organization. These settings include default sharing options, branding, and more.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Premium or Select</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must have Administrator selected in your Proof Permission Profile. For more information, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configure a user's proofing access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Configure actions

For information about using actions in the proofing viewer, see [Use actions on proof comments](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md).

You can configure actions for your organization in the following ways:

* [Add or rename an action](#add-or-rename-an-action) 
* [Deactivate or reactivate an action](#deactivate-or-reactivate-an-action) 
* [Reorder actions](#reorder-actions)

### Add or rename an action {#add-or-rename-an-action}

{{step1-to-proofing}}

1. Click **Settings** > **Account settings** in the upper-right corner of the Workfront Proof interface, then click the **Settings** tab.

1. Do either of the following:

   * To create a new action, in the **Actions** section, click **New action**.

     There is no limit to the number of actions you can set up in your account.
   
   * To rename an existing action, click **Setup** next to the action.

1. Type a name for the action, then click **Save**.
1. Click **Save.**

### Deactivate or reactivate an action {#deactivate-or-reactivate-an-action}

{{step1-to-proofing}} 

1. Click **Settings** > **Account settings** in the upper-right corner of the Workfront Proof interface, then click the **Settings** tab.

1. Click **Setup** next to the action you want to deactivate or reactivate.
1. Select **Activate** or **Deactivate**, then click **Save**.

### Reorder actions {#reorder-actions}

{{step1-to-proofing}} 

1. Click **Settings** > **Account settings** in the upper-right corner of the Workfront Proof interface, then click the **Settings** tab.

1. Click the blue up and down arrows next to **Setup** to reorder the actions.

   ![Re-order_actions.png](assets/re-order-actions-350x103.png)

## Configure custom devices for proofs

You can add any custom devices to your system, allowing users to review interactive content and simulate how the content appears on a specific device.

For information about how users can select devices when reviewing interactive content, see [Change interactive proof resolution in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)

To add a custom device:

{{step1-to-proofing}} 

1. Click **Settings** > **Account settings** in the upper-right corner of the Workfront Proof interface, then click the **Settings** tab.

1. In the **Custom Devices for proofs** section, click **Add new device**.

1. In the **Add new device** box that appears, specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>The name users see when selecting the device in the Desktop Proofing Viewer, as described in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">Change interactive proof resolution in the proofing viewer</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensions</td> 
      <td>Specify the dimensions to use for this device. Users see the dimensions displayed below the device name.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ratio</td> 
      <td>Specify the ratio for the device.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type</td> 
      <td>Select whether the device is a Mobile, Tablet, or Desktop.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">User agent string</td> 
      <td>Enter the user agent for the device to provide information that makes our software run and display as designed for the device.<p>You can obtain the user agent by going to <a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a> from the device.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disabled</td> 
      <td>If this option is selected, the device is not available for users to select when reviewing interactive proofs.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Create**.

## Configure pop-up messages for proofs

You can configure pop-up messages on proofs to communicate general information to all reviewers in your organization.

You can configure messages to appear in the following situations:

* **On load message**: Displays when the proof first opens. Useful for explaining to users how to review a proof or to provide a disclaimer or other legal text.
* **On decision message**: Displays when a user selects a decision on a proof. Useful for giving your users checklists for things such as brand or regulatory compliance. For information about decisions, see [Make a decision on a proof in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

* **Confirm button text**: The label that displays on the button in the On load pop-up message explained above.

To create pop-up messages for proofs:

1. Click **Edit** to the right of the message you want to customize.
1. Specify a message and include the appropriate formatting, then click **Save**.
1. (Optional) If you customized the On load message and you want to also customize the confirmation button label, click **Edit** to the right of **Confirm button text**, specify a label, then click **Save**. 

## Configure proof defaults

For information about configuring proof defaults for your organization, see [Configure default proof settings](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).


## Configure sharing defaults

You can specify who your organization's proofs can be shared with, what versions are available for reviewers, and when proofs with an Automated Workflow are visible to users who are associated with a given stage.

For more detailed information about sharing settings within Workfront Proof, see [Configure sharing settings for your users](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md). 

## Brand the Workfront Proof site

If you are using Workfront Proof, you can set up branding for the following areas of the site:

* The splash page that displays when the proof loads
* Log in and Log out screens
* Email notifications

For detailed information about how to brand the Workfront Proof site, see  [Brand the Workfront Proof site](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).

## Configure advanced password settings

>[!IMPORTANT]
>
>This option is available only for Legacy Workfront plans. If you are on a Pro, Business or Enterprise Workfront plan, you can no longer configure advanced password settings.

Under **Advanced password settings**, you can enhance password security for your users.

1. Click **Setup** to the right of the setting you want to configure:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Minimum password length</td> 
      <td>The default Workfront Proof password length is six characters. You may want to increase the number, depending on your organization's policies.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Character mix</strong> </td> 
      <td>You can force the users to use a mix of lowercase, uppercase, numbers, and symbols in their passwords. You decide how many characters the password should contain.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Maximum characters repetition</strong> </td> 
      <td>You can specify how many characters can repeat in each user's password.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatic password aging</td> 
      <td>Forces users to regularly change their password. You decide how often they will do so.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Number of password repetitions not allowed</strong> </td> 
      <td>Configure the number of password repetitions not allowed in your account.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Profile lockout</strong> </td> 
      <td>Locks your users out of the account after a number of unsuccessful login attempts that you specify. You also specify how long they should wait before they can access their account again.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lock user if password not reset after 30 days</td> 
      <td>If your user doesn't change their initial password within 30 days from their profile activation, they are locked out of the account.<br><p>Account Administrators can unlock (reactivate) users who get automatically locked by the system. This will give them additional seven days to change their password.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lock user account if inactive for 120 days</td> 
      <td>If your user doesn't log into Workfront Proof or a Login-required proof for 120 days, they are locked out of the account.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Change password after first login</strong> </td> 
      <td>Requires users to change their temporary password after their first login.<p>Account Administrators can unlock (reactivate) users who are automatically locked out by the system.</p><p>or more password information, see <a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">Logging in and changing your password and email for Workfront Proof</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>
