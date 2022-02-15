---
filename: prevent-spoofing-add-wf-spf-records
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# Prevent spoofing and add `Workfront` SPF records {#prevent-spoofing-and-add-workfront-spf-records}



## Problem {#problem}

If users are not receiving `Workfront` email notifications, you need to add `Workfront` SPF records to your firewall. You must work with your IT team to add SPF records.


## Solution {#solution}

If you already added the IP addresses to your allowlist for your production environment as described in&nbsp; [Configure your firewall](configure-your-firewall.md)&nbsp;and users are still not receiving emails:



1.  Add the following SPF record to your firewall:


   *spf.workfront.com* 


   This automatically adds all `Workfront` IP addresses to your allowlist on your firewall and allows all spam filters (that use SPF records) to validate `Workfront` servers as valid senders for&nbsp;your domain.


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



If you cannot add SPF records to your firewall due to company policy, please work with your `Workfront` Support Representative.
