---
filename: configure-workfront-saml-1.1
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
---



# Configure *`Adobe Workfront`* with SAML 1.1 {#configure-adobe-workfront-with-saml}



>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Business Platform.
>
>
>If your organization has been onboarded to the Adobe Business Platform, Single Sign-On (SSO) is handled automatically as part of that integration. You do not need to configure or enable this functionality.
>
>
>For a list of procedures that differ based on whether your organization is migrated to Adobe IMS, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).





>[!IMPORTANT] {type="important"}
>
>Security Assertion Markup Language (SAML) 1.1 is now supported only in a limited capacity as a single sign-on (SSO) option; it will be removed from the product in 2020. We recommend moving to SAML 2.0. For more information, see [Configure Adobe Workfront with SAML 2.0](configure-workfront-saml-2.md).


The following sections provide information about using SAML 1.1 with *`Adobe Workfront`*.


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



## SAML 1.1 single sign-on solution {#saml-single-sign-on-solution}

As a *`Workfront administrator`*, you can integrate *`Workfront`* with SAML 1.1.


Unlike other single sign-on solutions, auto-provisioning users and attribute-mapping are not available for Federated SSO configuration, including SAML 1.1.


## Configure the SAML 1.1 server to communicate with *`Workfront`* {#configure-the-saml-server-to-communicate-with-workfront}

In order to have home page landing preferences honored when implementing a Federated ID (SAML) SSO environment, you need to make sure the federated server is set up to point to *https://[Assigned Company Sub-domain]. *`Workfront`*-ondemand.com/ *`Workfront`*/.*


## Configure *`Workfront`* with SAML 1.1 {#configure-workfront-with-saml}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `System` > `Single Sign-On (SSO)`.

1.  In the `Type` drop-down list, select `SAML 1.1`.
1.  Specify the following information:

    
    
    * `Issuer`: Specify the domain provider obtained from your SAML service provider. It is possible to provide the port instead, for example: `example.company.com:80`  
    
    * `Login Portal URL`: Specify the login URL used to log in to all your SSO-enabled applications, including *`Workfront`*.  
    
    * `Sign-out URL`: Specify the URL displayed after users log out of *`Workfront`*.  
    
    * `Change password URL`: Specify the URL where users will be directed if they need to change their password.   
      Since users maintain one password across multiple platforms when integrated with SAML 1.1, it is important that they are directed to a central location to change their password rather than being allowed to change their password in *`Workfront`*.  
    
    * `Certificate`: Upload a valid certificate for authentication of a secure connection. OnDemand clients are required to do this. The certificate is obtained from your SAML 1.1 system administrator.  
    
    * `Admin Exemption`: When this box is checked, *`Workfront`* will attempt to first login through SAML for users with System Administrator Access Level. If authentication fails, *`Workfront`* will use local authentication for administrators. We recommend that you always have this option selected, to provide your *`Workfront administrator`* a way for logging into *`Workfront`* in the event that your SAML 1.1 provider is temporarily unavailable.  
    
    * `Enable`: Select this option to enable the integration with SAML 1.1. If it is not selected, SAML 1.1 will not be activated. 
    
    

1. Click `Save`. 


