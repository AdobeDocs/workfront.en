---
filename: prevent-spoofing-add-wf-spf-records
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
---



# Prevent spoofing and add *`Adobe Workfront`* SPF records {#prevent-spoofing-and-add-adobe-workfront-spf-records}



## Problem {#problem}

If users are not receiving *`Adobe Workfront`* email notifications, you need to add *`Workfront`* SPF records to your firewall. You must work with your IT team to add SPF records.


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Solution {#solution}

If you already added the IP addresses to your allowlist for your production environment as described in&nbsp; [Configure your firewall](configure-your-firewall.md)&nbsp;and users are still not receiving emails:



1.  Add the following SPF record to your firewall:


   *spf.workfront.com* 


   This automatically adds all *`Workfront`* IP addresses to your allowlist on your firewall and allows all spam filters (that use SPF records) to validate *`Workfront`* servers as valid senders for&nbsp;your domain.


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



If you cannot add SPF records to your firewall due to company policy, please work with your *`Workfront`* Support Representative.
