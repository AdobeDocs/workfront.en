


# Update SAML 2.0 metadata in your IDP when using enhanced authentication  {#update-saml-metadata-in-your-idp-when-using-enhanced-authentication}



>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Business Platform.
>
>
>If your organization has been onboarded to the Adobe Business Platform, Single Sign-On (SSO) is handled automatically as part of that integration. You do not need to configure or enable this functionality.
>
>
>For a list of procedures that differ based on whether your organization is migrated to Adobe IMS, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



As an *`Adobe Workfront administrator`*, you can integrate *`Workfront`* single sign-on (SSO) with any identity provider that supports the Security Assertion Markup Language (SAML) 2.0 protocol.


The following sections describe the integration process when your *`Workfront`* account has been upgraded to the enhanced authentication experience (not yet available to all organizations). For more information about the enhanced authentication experience, see [Enhanced Authentication overview](get-started-enhanced-authentication.md). 


For information about configuring SAML prior to your migration to the enhanced authentication experience, see [Update SAML 2.0 metadata in your identity provider](update-saml-2-metadata-ip.md).


##  



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



## Use Okta as your identity provider {#use-okta-as-your-identity-provider}

Okta is an example of an identity provider that supports SAML 2.0. This section describes how to use Okta as your identity provider. Similar steps would be required when configuring another identity provider that supports SAML 2.0.




>[!NOTE]
>
>Users are mapped based on their email address. In order to log in to *`Workfront`* using Okta, you must have a user with the same (case-insensitive) email address created in your *`Workfront`* customer.





Complete the following sections to configure Okta as your identity provider in *`Workfront`*.



* [Create a Workfront app in Okta](#creating-a-workfront-app-in-okta) 
* [Add your Okta instance as an identity provider in Workfront](#adding-your-okta-instance-as-an-identity-provider-in-workfront) 




### Create a *`Workfront`* app in Okta {#create-a-workfront-app-in-okta}




1. Log in to your Okta environment. 
1. Ensure that `Classic UI` is selected in the upper-left corner of the Okta interface.
1. In the menu, click `Applications` > `Applications`.

1. Click `Add Application`, then click `Create New App`.

1. In the `Create a New Application Integration dialog` box, select `SAML 2.0`, then click `Create`.

1. Specify a name for your *`Workfront`* app, then click `Next`.

1. In the SAML Settings page that displays, locate information required for the SAML Settings page: 
    
    
    1. Without exiting the browser tab where the Okta interface is displayed, open a separate browser tab or window.
    1. Specify the following URL in the browser:  

    
    
       *https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata*
    
    1. In the resulting XML file, identify the values for `entityID` and `Location`.
    
    
       ![sso-okta.png](assets/sso-okta-350x108.png)    
    

    
    1. Copy the value from the `entityID` field to your system clipboard. Do not close this browser tab.
    
    
1. Go back to the SAML Settings page that you opened in Step 6. 
1. Paste the value from the `entityID` field into the `Audience URI (SP Entity ID)` field.

1. In the XML file in your other browser tab, copy the value from the `Location` field.
1. Paste the value from the `Location` field into the `Single sign on` `URL` field.

1. Scroll to the `Attribute Statements (Optional)` section.
1. In the `Name` field, specify `email`.

1. In the `Value` field, specify `user.email`.

1. (Optional) Add any advanced values.
1. Click `Next`.
1. Select, `I'm an Okta customer adding an internal app`, then click `Finish`.





### Add your Okta instance as an identity provider in *`Workfront`* {#add-your-okta-instance-as-an-identity-provider-in-workfront}

This procedure provides essential information for configuring Okta as an identity provider in *`Workfront`*. For additional information about other mappings or configuration options, see [Configure Adobe Workfront with SAML 2.0](configure-workfront-saml-2.md).



1. Download the identity provider metadata for your Okta instance: 
    
    
    1. Log in to your Okta environment. 
    1. Ensure that `Classic UI` is selected in the upper-left corner of the Okta interface.
    1. In the menu, click `Applications` > `Applications`.
    
    1. Click the *`Workfront`* app that you created, as described in the section, [Create a Workfront app in Okta](#creating-a-workfront-app-in-okta)
    
    1. On the `Sign On` tab, click `Identity Provider metadata`.
    
    
       ![idp_okta_metadata.png](assets/idp-okta-metadata-350x243.png)    
    

    
    
       The metadata is opened as XML in a new browser tab.
    
    1. Copy the URL that is displayed in the browser URL field.
    
    
1. Log in to *`Workfront`* as a *`Workfront administrator`*.

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `System` > `Single Sign-On (SSO)`.

1.  (Conditional) If you see two tabs, click the `New SSO Providers`tab.


   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)




   >[!IMPORTANT] {type="important"}
   >
   >Do not delete your existing SSO configuration settings in the `Current SSO Provider` tab until your account is updated to the enhanced authentication experience and the new SSO configuration is fully functional.



1. Click `New SSO Provider`.
1. Specify a name, such as Okta IDP, then specify a description.
1. In the `Populate fields from Identity Provider Metadata` section, paste the URL that you copied in Step 1 into the `Metadata URL` field.   
   Alternatively, you can click `Choose File` to upload an .xml file, but we recommend that you paste the URL.

1. In the `Map User Attributes` section, in the `Directory Attribute` field, type `email`. ( `Email Address` is already populated in the ` *`Workfront`* User Attribute` field.)

1. (Optional) Enable `Make Default SSO Provider` to send unathenticated users to the identity provider login screen instead of to the *`Workfront`* login screen for authentication. We recommend that you enable this option only if all users in your system access *`Workfront`* through the identity provider.

1. Select the `Enable` checkbox. Before doing this, ensure that users in your system are aware of the new login experience to ensure they do not lose access to the *`Workfront`* system.

1. Click `Test Connection`.  
   You should see a message telling you the connection is successful. 

1. Click `Save`. 




## Using other identity providers {#using-other-identity-providers}

When using identity providers other than Okta (such as Ping or Centrify), you must re-upload the *`Workfront`* metadata to your identity provider.
