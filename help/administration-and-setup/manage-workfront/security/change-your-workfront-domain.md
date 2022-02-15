---
filename: change-your-workfront-domain
user-type: administrator
product-area: system-administration
navigation-topic: security
---



# Change your *`Adobe Workfront`* domain {#change-your-adobe-workfront-domain}

As an *`Adobe Workfront administrator`* and an authorized *`Workfront`* Support contact, you can request help from the *`Workfront`* Support team to change your organization's *`Workfront`* domain.


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



## Request a domain change {#request-a-domain-change}




1. Click the `Support` tab on the Workfront One page, then start creating a support case.
1. In the `Description` box, include the new new domain you want, as well as the timeframe when you want the new domain to go live.
1.  Finish filling out the boxes for the support case, then click `Submit`.


You can also call Workfront Support to get help changing your domain.


## Update the new domain if you are an SSO customer {#update-the-new-domain-if-you-are-an-sso-customer}

If your company utilizes SSO, the following steps are required after you have your *`Workfront`* domain changed.



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left sidebar, click `System` > `Customer Info` and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click `System` > `Single Sign-On (SSO)`.

1. Click `Download SAML 2.0 Metadata`.
1. After the file is downloaded, open it and make sure of the following:
    
    
    1. `entityID` is pointing to the new domain.
    1. All locations within `<md:AssertionConsumerService>` point to the new domain.
    
    
1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all *`Workfront`* integrations used by your organization.


