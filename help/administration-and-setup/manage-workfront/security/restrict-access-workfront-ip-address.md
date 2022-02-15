---
filename: restrict-access-workfront-IP-address
user-type: administrator
product-area: system-administration
navigation-topic: security
---



# Restrict access to *`Adobe Workfront`* by IP address {#restrict-access-to-adobe-workfront-by-ip-address}

You can configure *`Adobe Workfront`* to allow access only from designated IP addresses. Configuring *`Workfront`* in this way provides an additional layer of security for the *`Workfront`* application.


When someone attempts to access *`Workfront`* from an IP address that is not on the allowlist, *`Workfront`* cannot be reached.




>[!NOTE]
>
>Depending on the *`Workfront`* plan that you have purchased, you might not have access to this functionality in *`Workfront`*. Contact your Account Representative to learn what *`Workfront`* plan your organization has purchased





## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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



## How the firewall allowlist differs from the *`Workfront`* allowlist {#how-the-firewall-allowlist-differs-from-the-workfront-allowlist}

Configuring a *`Workfront`* allowlist is not the same as adding *`Workfront`* IP addresses to your corporate firewall allowlist.


For more information about adding *`Workfront`* IP addresses to your corporate firewall allowlist, see [Configure your firewall](configure-your-firewall.md).


## Adding IP addresses to the allowlist {#adding-ip-addresses-to-the-allowlist}

After you add IP addresses to the *`Workfront`* allowlist, only those IP addresses can be used to access *`Workfront`*.


Users who attempt to access *`Workfront`* from an IP address that is not on the allowlist are not able to log in. They receive an error message indicating that they are attempting to access *`Workfront`* from an IP address that has been blocked by the *`Workfront administrator`*.


To add IP addresses to the *`Workfront`* allowlist:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `System` > `Customer Info.`

1.  In the `IP allowlist` section, select `Enable IP allowlist.`


   This option is disabled by default.

1. Specify the IP address that you are currently using to access the *`Workfront`* system.  
   Or  
   Specify a range of IP addresses that includes the IP address that you are currently using to access the *`Workfront`* system.  
   The IP address that you are currently using to access *`Workfront`* must be added to the allowlist or the allowlist cannot be enabled.  
   These IP addresses should be provided by your network administrator. 

1. Click `Add IP Range,` then specify the IP address or range of IP addresses that you want to be able to access *`Workfront`*.  
   Repeat this step to add additional IP addresses or IP ranges. You can add up to 15 IP address or IP ranges.

1. Click `Save.`


