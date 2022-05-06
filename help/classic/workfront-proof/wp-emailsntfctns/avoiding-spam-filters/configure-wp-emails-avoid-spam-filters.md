---
filename: configure-wp-emails-avoid-spam-filters
product: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configure Workfront Proof emails to avoid spam filters
description: Your email client's spam filter serves an important purpose: protecting you from annoying and possibly malicious spam emails. But, if you don't have the correct settings in the spam filter, it can keep you from seeing the following important Workfront Proof emails: proof email notifications, newsletters, and special communications.
---

# Configure Workfront Proof emails to avoid spam filters

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Your email client's spam filter serves an important purpose: protecting you from annoying and possibly malicious spam emails. But, if you don't have the correct settings in the spam filter, it can keep you from seeing the following important Workfront Proof emails: proof email notifications, newsletters, and special communications.

To make sure that your Workfront Proof emails are always routed to your inbox instead of your spam folder, you should add the following to the allowlist:

* Workfront Proof mail server: **mx.proofhq.com**
* Workfront Proof "from" email addresses (for example, notification@proofhq.com)

For more information about URLs to add to your allowlist, see [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)&nbsp;in the article [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Workfront Proof "from" email addresses

Depending on your type of email client, you might need to add Workfront Proof "from" email addresses to one of the following to prevent the spam filter from routing your emails to your spam folder in the future:

* Your contacts list
* Your Safe Senders list
* A filter that you create to deliver emails from those addresses to your inbox

You might also need to remove any existing Workfront Proof emails from your spam folder and check whether any of the "from" addresses are on the blocked address list. This help page lists the Workfront Proof "from" addresses and shows how to add them to the spam filter in the following email clients:

* Gmail
* Microsoft Outlook 2003 - 2007
* Windows Live Hotmail
* Yahoo Mail
* Aol

>[!NOTE]
>
>If you have any questions about a procedure described here, please check your email client's help.

For more information, see [Configure spam settings for common email clients](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## The Workfront Proof "from" email addresses to copy

To make sure that your Workfront Proof emails reach your inbox, you will need to add two Workfront Proof email addresses separately to your email client's spam filter:

* The general support address, support@proofhq.com, from which Workfront Proof sends out many email communications
* A notification address from which Workfront Proof sends proof notification emails to the proof creator and the reviewers with links to the proof. This might be a general address, notification@support.proofhq.com, or a specific address if you have a customized subdomain or a white label domain.

To add Workfront Proof "from" addresses to your email client's filter:

1. Copy the general Workfront Proof support "from" email address (support@proofhq.com) and paste it into the field indicated for your email client.
1. Copy the appropriate one of the following Workfront Proof "from" email addresses and paste it SEPARATELY into the field indicated for your email client:

   * notification@support.proofhq.com if you do NOT have a customized subdomain or a white label domain
   * notification@yoursubdomain.proofhq.com if you have a customized subdomain; substitute your subdomain name in this address
   * notification@yoursubdomain.yourdomain.com if you have a white label domain; substitute your subdomain name and domain name in this address

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "from" addresses.</p>
-->

