---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Prepare to onboard your organization to the Adobe Admin Console
description: Because Adobe Workfront is an Adobe product, you can access it through the Adobe Admin Console. This enables you to manage Workfront along with other Adobe accounts and products for your users in a central place.
hidefromtoc: true
---

# Prepare to onboard your organization to the Adobe Admin Console

Because Adobe Workfront is an Adobe product, you can access it through the Adobe Admin Console. This enables you to manage Workfront along with other Adobe accounts and products for your users in a central place.

All Workfront customers will eventually be moved to the Adobe Admin Console. After your organization moves to the Adobe Admin Console, Workfront authentication is managed by the Adobe Admin Console. Preparing and making this move sooner lays the groundwork for efficiency in work management and positions your organization for faster innovation in the future 

<!--
<MadCap:conditionalText style="color: #ff0000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
(How?)
</MadCap:conditionalText>
-->

For an overview of the Adobe Admin Console, see [Admin Console Overview](https://helpx.adobe.com/enterprise/using/admin-console.html).

## Migration checklist

To ensure that your organization can migrate to the Adobe Admin Console, you must perform the following actions

1. Identify the desired Adobe Admin Console where you would like to add Workfront. If you have multiple Adobe Admin Consoles and you are unsure which one is most appropriate add Adobe Workfront to, contact Workfront Support.
1. Confirm your willingness to add Adobe Workfront to your current Adobe Admin Console. This is done from the Adobe Admin Console. 

   <!--
   <span style="color: #ff0000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Instructions?)</span>
   -->

1. Set up identity management on the Adobe Admin Console.

   For instructions, see the Identity Management section of the [Deployment Guide](https://helpx.adobe.com/enterprise/using/deployment-planning.html). 

1. (Conditional) If using Single Sign-on, connect the new Adobe Admin Console to your existing SSO provider

   For more information and instructions, see [Set up identity](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >If your organization does not use Single Sign-on, any users migrated to the Adobe Admin Console will receive an email to create their account and password.

1. Ensure that user email addresses are ready for migration:

   1. Remove duplicate emails from Workfront
   1. (Conditional) If you are utilizing custom API integrations, confirm those users have a valid email address that they can access.
   1. (Optional) We recommend deactivating any users who no longer need access to Workfront, so they are not added to the Adobe Admin Console.

   >[!IMPORTANT]
   >
   >These actions regarding user emails must be complete before your organization begins moving to the Adobe Admin Console.

1. (Optional) Update all custom integrations to use OAuth2.

   For instructions on setting up OAuth2 integrations, see [Create OAuth2 applications for Workfront integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   Creating OAuth2 integrations is only available in the new Workfront experience.

   >[!NOTE]
   >
   >This step is optional, but highly recommended.

After your Adobe Admin Console is configured with Workfront, you can use it to manage your users.

For more information, see [Manage users in the Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

For a list of other actions that are different based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
