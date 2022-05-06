---
filename: prevent-spoofing-add-wf-spf-records
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Prevent spoofing and add Adobe Workfront SPF records
description: If users are not receiving Adobe Workfront email notifications, you need to add Workfront SPF records to your firewall. You must work with your IT team to add SPF records.
---

# Prevent spoofing and add Adobe Workfront SPF records

## Problem

If users are not receiving Adobe Workfront&nbsp;email notifications, you need to add Workfront SPF records to your firewall. You must work with your IT team to add SPF records.

## Access requirements

You must have the following access to perform the steps in this article: 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

If you already added the IP addresses to your allowlist for your production environment as described in&nbsp; [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)&nbsp;and users are still not receiving emails:

1. Add the following SPF record to your firewall:

   *spf.workfront.com*

   This automatically adds all Workfront IP addresses to your allowlist on your firewall&nbsp;and allows all spam filters (that use SPF records) to validate Workfront servers as valid senders for&nbsp;your domain.

   >[!NOTE]
   >
   >&nbsp;An SPF record is a TXT record that is part of a DNS zone file. We do not support modifying your DNS zone file.

1. You must specify what type of SPF record needs to be configured. These are the valid types of SPF records:&nbsp;

   * all (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx&nbsp;(https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * exists (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   For example, “v=spf1 a mx include: [spf.workfront.com](http://spf.workfront.com/)&nbsp;-all”

If you cannot add SPF records to your firewall due to company policy, please work with your Workfront Support Representative.
