---
filename: configure-your-email-allowlist
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configure your email allowlist
description: If your organization uses the WorkfrontEnterprise plan, you can create a Workfront email allowlist to control:
---

# Configure your email allowlist

If your organization uses the *Workfront**Enterprise* plan, you can create a *Workfront* email allowlist to control:

* Which email domains are allowed to accept emails from *Workfront*.
* Which email domains can be in the email address that users specify in their user profile.

This is useful if your organization’s security policy restricts users from sending data stored in *Workfront* to external email addresses—you can include only your internal company domains in the allowlist to ensure that this policy is followed.

>[!IMPORTANT]
>
>*Your IT team* should ensure that incoming email from >
>```>
>notifications@my.workfront.com
>```>
>is not blocked in your organization’s system.
>
>All email from *Workfront* is sent from that address to increase successful email delivery and to eliminate spoofing of emails. This includes both automated alerts and user-to-user communication.
>
>For example, the From line in a *Workfront* email you receive from a user named Joan Harris would look like this:
>
>```>
>Joan Harris <notifications@my.workfront.com>
>```>

For information about configuring your organization's firewall to open communication between your environment and the *Adobe Workfront* servers, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Other allowlists

If your organization has the *Enterprise* plan, you can configure an *Adobe Workfront* IP allowlist that limits access to *Workfront* to 45 IP addresses or IP address ranges that you specify. This provides an additional layer of security for the *Workfront* application. For more information, see [Restrict access to Adobe Workfront by IP address](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Also, if your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist. This opens communication between your environment and the *Adobe Workfront* servers. For information about that, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configure your email allowlist

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Customer info</span>.</li> 
 <li value="3"> <p>In the <span class="bold">Email Allowlist</span> section, select <span class="bold">Enable Domain Allowlist</span>, then click <span class="bold">Add Domain</span>.</p> </li> 
 <li value="4">In the box that displays, type a domain that you want to allow, such as <code>ourcompany.com</code>, then click <span class="bold">Add Domain</span>.</li> 
 <li value="5">Repeat the previous step to add any other domains you want to allow.</li> 
 <li value="6">When you are finished, click <span class="bold">Save</span>.</li> 
</ol>

