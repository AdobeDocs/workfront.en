---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configure Your Email Allowlist
description: If your organization uses the WorkfrontEnterprise plan, you can create a Workfront email allowlist to control which email domains are allowed to accept emails from Workfront and which email domains can be in the email address that users specify in their user profile. This is useful if your organization's security policy restricts users from sending data stored in Workfront to external email addresses—you can include only your internal company domains in the allowlist to ensure that this policy is followed..
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
---
# Configure your email allowlist

If your organization uses the Workfront Enterprise plan, you can create a Workfront email allowlist to control:

* Which email domains are allowed to accept emails from Workfront.
* Which email domains can be in the email address that users specify in their user profile.

This is useful if your organization's security policy restricts users from sending data stored in Workfront to external email addresses—you can include only your internal company domains in the allowlist to ensure that this policy is followed.

>[!IMPORTANT]
>
>Your IT team should ensure that incoming email from `notifications@my.workfront.com` is not blocked in your organization's system.
>
>All email from Workfront is sent from that address to increase successful email delivery and to eliminate spoofing of emails. This includes both automated alerts and user-to-user communication.
>
>For example, the From line in a Workfront email you receive from a user named Joan Harris would look like this:
>`Joan Harris <notifications@my.workfront.com>`

For information about configuring your organization's firewall to open communication between your environment and the Adobe Workfront servers, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Other allowlists

If your organization has the Enterprise plan, you can configure an Adobe Workfront IP allowlist that limits access to Workfront to 45 IP addresses or IP address ranges that you specify. This provides an additional layer of security for the Workfront application. For more information, see [Restrict access to Adobe Workfront by IP address](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Also, if your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist. This opens communication between your environment and the Adobe Workfront servers. For information about that, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configure your email allowlist

{{step-1-to-setup}}

1. Click **System** > **Customer info**.
1. In the **Email Allowlist** section, select **Enable Domain Allowlist**, then click **Add Domain**.
1. In the box that displays, type a domain that you want to allow, such as `ourcompany.com`, then click **Add Domain**.
1. Repeat the previous step to add any other domains you want to allow.
1. When you are finished, click **Save**.
