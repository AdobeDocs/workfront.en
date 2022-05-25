---
filename: configure-sharing-settings-users
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configure sharing settings for your users
description: As an Adobe Workfront administrator or Workfront Proof administrator, you can configure the user accounts with which proofs can be shared, whether users can see all versions of a proof, and the timing when users gain access to shared items.
---

# Configure sharing settings for your users

As an Adobe Workfront administrator or Workfront Proof administrator, you can configure the user accounts with which proofs can be shared, whether users can see all versions of a proof, and the timing when users gain&nbsp;access to shared items.&nbsp;

## Access requirements

You must have the following:

<table> 
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

## Configure sharing with other accounts&nbsp;

1. From Workfront, click the Main Menu ![](assets/main-menu-icon.png), then click Proofing ![](assets/proofing-in-main-menu.png) to access Workfront Proof.    

1. Click **Settings** > **Account settings**, then click the **Settings** tab.

1. In the **Sharing** section, to the right of **Allow sharing with**, click **Setup**.

1. In the drop-down list that appears, select an option to specify whether you want to make proofs available to anyone, restrict the sharing of your proofs to your own account only, or restrict it to your own account and any partner accounts you're collaborating with.
1. Click **Save.**

## Configure visibility to all versions of a shared proof

1. From Workfront, click the Main Menu ![](assets/main-menu-icon.png), then click Proofing ![](assets/proofing-in-main-menu.png) to access Workfront Proof.    

1. Click **Settings** > **Account settings**, then click the **Settings** tab.

1. In the **Sharing** section, to the right of **Recipients can view all versions**, select **Enable** or **Disable** to indicate whether you want to allow&nbsp;recipients to view all versions of a proof within the proofing viewer when the Proof URL is enabled.

## Configure proof visibility based on workflow stage activity

You can specify when proofs with an automated workflow are visible to users who are associated with a given stage.

>[!NOTE]
>
>* This option is available&nbsp;only when using the standalone Workfront Proof application; it is not available when using a Workfront Proof instance that is integrated with Workfront or when proofing within Workfront.
>* Users receive an email notification about the proof only after it enters the stage the user is associated with, regardless of this setting.
>

To configure when proofs with an automated workflow are visible to users:

1. From Workfront, click the Main Menu ![](assets/main-menu-icon.png), then click Proofing ![](assets/proofing-in-main-menu.png) to access Workfront Proof.    

1. Click **Settings** > **Account settings**, then click the **Settings** tab.

1. In the&nbsp;**Sharing**&nbsp;section, enable or disable&nbsp;**Proof visibility based on stage activation**.

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Disabled</strong> (default)</td> 
      <td>Proofs are visible to users at the time&nbsp;the proof is created.<br><p>Any user associated with a stage in the workflow for the proof can see the proof in search results immediately after the proof is created.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enabled</strong> </td> 
      <td> <p>Proofs are visible to users only&nbsp;after the stage they are associated with becomes <strong>active.</strong></p> <p><b>NOTE</b>:   
        <ul> 
         <li><em style="font-style: normal;">After you enable this option, existing proofs are still visible to users who could view it when it was created.</em> </li> 
         <li><em style="font-style: normal;">After a user gains access to a version of a proof (because the stage the user is associated with becomes active), the user can see only the version where the stage is activated. If a previous version never reached the stage the user is associated with, the user cannot see that version of the proof.&nbsp;</em> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

