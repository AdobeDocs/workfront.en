---
filename: renew-wf-saml-2-certificate
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,security,certificate,Admin,Exemption,configure,metadata
navigation-topic: security
---



# Renew the *`Adobe Workfront`* SAML 2.0 metadata certificate {#renew-the-adobe-workfront-saml-metadata-certificate}



>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Adobe Business Platform. If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.
>
>
>For instructions on performing this action in the Adobe Admin Console, see "The digital signature in the SAML response did not validate with the identity provider's certificate" in [Troubleshooting errors](https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html), or reach out to your Adobe Admin Console Administrator.
>
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



The *`Adobe Workfront`* servers utilize the SAML 2.0 protocol for authentication and authorization. Once updated, the new certiﬁcate remains valid for one year. When it is time for you to renew the certiﬁcate on your identity provider, you receive a warning in Workfront alerting you that this change must occur. As a *`Workfront administrator`*, you can manage this change at the system level.


In 2021, our SAML 2.0 metadata certiﬁcate expired on October 27. The next date when we plan to update the certiﬁcate is November 22, 2022.


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



## Configure SAML 2.0 within *`Workfront`* {#configure-saml-within-workfront}

To review the warning message and acknowledge the update of the SAML 2.0 metadata in your identity provider:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `System` > `Single Sign-On`.

1. In the `Type` drop-down menu, select `SAML 2.0`.

1.  Click `Download SAML 2.0 Metadata`.


   This downloads the renewed *`Workfront`* certiﬁcate for SAML 2.0, which contains the correct metadata for your server.

   ` `**Warning: **`` Before you upload the *`Workfront`* metadata to your Single Sign-On (SSO) provider in Step 5, copy your current Assertion Consumer Service (ACS) URL to a safe place. This URL, also known as the Reply URL, is found on your SSO provider's *`Workfront`* configuration page. 


   If the ACS URL changes after you upload the *`Workfront`* metadata, this means that the metadata might contain an incorrect ACS URL. You must change it back to the one you copied in order to avoid breaking your Single Sign-On connection. Your updated certificate will still be correct after you do this.

1. Go to your identity provider server and update the new certiﬁcate you downloaded from *`Workfront`* on that server, as explained in [Update SAML 2.0 metadata in your identity provider](update-saml-2-metadata-ip.md).

1.  In *`Workfront`*, on the **Single Sign-on (SSO) page**, make sure that `Admin Exemption` is selected.


   When this ﬁeld is selected, *`Workfront administrators`* can log in to *`Workfront`* with their SSO credentials or their *`Workfront`* credentials.

1.  Click `Save`.


   The warning message no longer displays because you acknowledged the renewal of the SAML 2.0 certiﬁcate on the server of your identity provider.

1.  Click `Test Connection` to test your conﬁguration.


   You should see a message confirming that the connection was successful.



For more information, or for assistance with the manual conﬁguration of metadata, please contact our Support Team, as explained in [Contact Customer Support](contact-customer-support.md).
