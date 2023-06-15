---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Prevent spoofing and add [!DNL Adobe Workfront] SPF records
description: If users are not receiving [!DNL Adobe Workfront] email notifications, you need to add [!DNL Workfront] SPF records to your firewall. You must work with your IT team to add SPF records.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
---
# Prevent spoofing and add [!DNL Adobe Workfront] SPF records

## Problem

If users are not receiving [!DNL Adobe Workfront] email notifications, you need to add [!DNL Workfront] SPF records to your firewall. You must work with your IT team to add SPF records.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a [!DNL Workfront] administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

If you already added the IP addresses to your allowlist for your production environment as described in [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) and users are still not receiving emails:

1. Add the following SPF record to your firewall:

   *spf.workfront.com*

   This automatically adds all [!DNL Workfront] IP addresses to your allowlist on your firewall and allows all spam filters (that use SPF records) to validate [!DNL Workfront] servers as valid senders for your domain.

   >[!NOTE]
   >
   > An SPF record is a TXT record that is part of a DNS zone file. We do not support modifying your DNS zone file.

1. You must specify what type of SPF record needs to be configured. These are the valid types of SPF records:

   * all (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * exists (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   For example, "v=spf1 a mx include: spf.workfront.com -all"

If you cannot add SPF records to your firewall due to company policy, please work with your [!DNL Workfront] Support Representative.
