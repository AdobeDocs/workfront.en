---
filename: prevent-spoofing-add-wf-spf-records
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Prevent spoofing and add Adobe Workfront SPF records
description: If users are not receiving Adobe Workfront email notifications, you need to add Workfront SPF records to your firewall. You must work with your IT team to add SPF records.
---

# Prevent spoofing and add `Adobe Workfront` SPF records

## Problem

If users are not receiving `Adobe Workfront` email notifications, you need to add `Workfront` SPF records to your firewall. You must work with your IT team to add SPF records.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

If you already added the IP addresses to your allowlist for your production environment as described in&nbsp; [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)&nbsp;and users are still not receiving emails:

<ol> 
 <li value="1"> <p>Add the following SPF record to your firewall:</p> <p><em style="font-weight: bold; font-style: normal;">spf.workfront.com</em> </p> <p>This automatically adds all <span>Workfront</span> IP addresses to your allowlist on your firewall&nbsp;and allows all spam filters (that use SPF records) to validate <span>Workfront</span> servers as valid senders for&nbsp;your domain.</p> <note type="note">
   &nbsp;An SPF record is a TXT record that is part of a DNS zone file. We do not support modifying your DNS zone file.
  </note> </li> 
 <li value="2">You must specify what type of SPF record needs to be configured. These are the valid types of SPF records:&nbsp;<br>
  <ul dir="auto">
   <li>all (https://dmarcian.com/spf-syntax-table/#all)</li>
   <li>ip4 (https://dmarcian.com/spf-syntax-table/#ip4)</li>
   <li>ip6 (https://dmarcian.com/spf-syntax-table/#ip6)</li>
   <li>a (https://dmarcian.com/spf-syntax-table/#a)</li>
   <li>mx&nbsp;(https://dmarcian.com/spf-syntax-table/#mx)</li>
   <li>ptr (https://dmarcian.com/spf-syntax-table/#ptr)</li>
   <li>exists (https://dmarcian.com/spf-syntax-table/#exists)</li>
   <li>include (https://dmarcian.com/spf-syntax-table/#include)</li>
  </ul> For example, “v=spf1 a mx include:<a href="http://spf.workfront.com/">spf.workfront.com</a>&nbsp;-all”</li> 
</ol>

If you cannot add SPF records to your firewall due to company policy, please work with your `Workfront` Support Representative.
