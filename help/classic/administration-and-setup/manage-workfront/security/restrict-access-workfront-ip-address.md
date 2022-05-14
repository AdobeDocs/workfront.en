---
filename: restrict-access-workfront-IP-address
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Restrict access to Adobe Workfront by IP address
description: You can configure an Adobe Workfront IP allowlist that limits access to Workfront to 45 IP addresses or IP address ranges that you specify. This provides an additional layer of security for the Workfront application.
---

# Restrict access to Adobe Workfront by IP address

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can configure an Adobe Workfront IP allowlist that limits access to Workfront to 45 IP addresses or IP address ranges that you specify. This provides an additional layer of security for the Workfront application.

These IP addresses or IP address ranges should be provided by your network administrator.

## Access requirements

You must have the following to perform the steps in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Enterprise</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Other allowlists

If your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist. This opens communication between your environment and the Adobe Workfront servers. For information about that, see [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Also, if your organization uses the Enterprise plan, you can configure the Workfront email allowlist to control which email domains are allowed to accept emails from Workfront and which email domains can be in the email address that users specify in their Workfront user profile. For more information, see [Configure your email allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Adding IP addresses to the allowlist

After you add IP addresses to the Workfront allowlist, only those IP addresses can be used to access Workfront. Users who try to access Workfront from another IP address receive an error message indicating that their IP address is blocked.

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
1. Click **System** > **Customer Info.**

1. In the **IP allowlist** section, select **Enable IP allowlist.**

   This option is disabled by default.

1. Specify the IP address that you are currently using to access the Workfront system.

   Or

   Specify a range of IP addresses that includes the one you are currently using to access the Workfront system.

   The IP address you are using to access Workfront must be added to the allowlist before the allowlist is enabled.

1. Click **Add IP Range,** then specify the IP address or range of IP addresses that you want to be able to access Workfront.
1. (Optional) Repeat the previous step to add additional IP addresses or IP address ranges.

   You can add up to 30 addresses or ranges.

1. Click **Save.**

