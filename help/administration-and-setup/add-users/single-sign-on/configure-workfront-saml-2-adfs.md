---
filename: configure-workfront-saml-2-adfs
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
---



# Configure *`Adobe Workfront`* with SAML 2.0 using ADFS {#configure-adobe-workfront-with-saml-using-adfs}



>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Business Platform.
>
>
>If your organization has been onboarded to the Adobe Business Platform, Single Sign-On (SSO) is handled automatically as part of that integration. You do not need to configure or enable this functionality.
>
>
>For a list of procedures that differ based on whether your organization is migrated to Adobe IMS, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



As an *`Adobe Workfront administrator`*, you can integrate *`Workfront`* with a Security Assertion Markup Language (SAML) 2.0 solution for single sign-on while using Active Directory Federation Services (ADFS).


This guide focuses on setting up ADFS without auto provisioning or attribute mappings. We recommend that you complete the setup and test it prior to setting up any auto provisioning.


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



## Enable authentication to *`Workfront`* with SAML 2.0 {#enable-authentication-to-workfront-with-saml}

To enable authentication to the *`Workfront`* web application and the *`Workfront`* mobile application with SAML 2.0, complete the following sections: 




* [Retrieve the Workfront SSO metadata file](#retrieving-workfront-metatdata) 
* [Configure Relying Party Trusts](#configuring-relying-party-trusts) 
* [Configure Claim Rules](#configuring-claim-rules) 
* [Upload the metadata file and test the connection](#uploading-metadata-file) 




### Retrieve the *`Workfront`* SSO metadata file {#retrieve-the-workfront-sso-metadata-file}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `System` > `Single Sign-On (SSO)`.

1.  In the `Type` drop-down menu, click `SAML 2.0` to display additional information and options.  

1. Copy the URL that displays after `Metadata URL`. 
1. Continue to the following section, [Configure Relying Party Trusts](#configuring-relying-party-trusts).




### Configure Relying Party Trusts {#configure-relying-party-trusts}




1. Open the `ADFS Manager` using the Windows server 2008 R2 (version may vary).
1. Go to `Start.`
1. Click `Administration Tools.`
1. Click `ADFS 2.0 Management.`
1. Select `ADFS` and expand `Trust Relationships`.

1.  Right-click `Relying Party Trusts`, then select `Add Relying Party Trust`to launch the Add Relying Party Trust Wizard.


   ![](assets/screen-shot-2014-10-22-at-2.48.12-pm-1-350x153.png)



1.  From the `Welcome Page`, select `Start`. 
1. In the `Select Date Source` section, paste the metadata URL from *`Workfront`*.

1.  Click `Next`.
1.  Click `OK`to acknowledge the warning message. 


   This opens the `Specify Display Name` section.

1.  Add a `Display Name` and `Notes`to distinguish the Trust, then click `Next`.  



   ![](assets/screen-shot-2014-10-22-at-2.50.58-pm-350x282.png)



1.  Select `Permit all user to access this relying party` (Or `None` if you want to configure this later).  



   ![](assets/screen-shot-2014-10-22-at-2.53.19-pm-350x232.png)



1.  Click `Next`. 


   This takes you to the `Ready to Add Trust` section.

1. Continue to the following section [Configure Claim Rules](#configuring-claim-rules).




### Configure Claim Rules {#configure-claim-rules}




1.  `<li> <p>Click <span class="bold">Next</span> in the Ready to Add Trust section<span class="bold">, </span>then ensure that the <span class="bold">Open the Edit Claim Rules dialog box </span>option is selected. </p> <p>This will allow you to edit Claim Rules in a future step.<br><img src="assets/screen-shot-2014-10-22-at-2.53.28-pm-350x236.png" alt="" style="width: 350;height: 236;"></p> </li>` `<li>Click <span class="bold">Close</span>.</li>` `<li>Click <span class="bold">Add Rule.</span></li>` `<li>Select <span class="bold">Send LDAP Attribute as Claims</span>.<br><img src="assets/screen-shot-2014-10-22-at-2.56.29-pm-350x185.png" alt="" style="width: 350;height: 185;"></li>` `<li>Click <span class="bold">Next</span> to display the <span class="bold">Configure Claim Rule</span> step.<br><img src="assets/screen-shot-2014-10-22-at-2.57.00-pm-350x224.png" alt="" style="width: 350;height: 224;"></li>` `<li> <p>Specify the following minimum requirements to configure the claim rule: (This will go in the <span class="bold">Federation ID</span> on the user setup and is used to distinguish who is logging in.)</p>  <table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">   <tbody>    <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">     <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Claim rule name:</span> </td>     <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Specify a name for the claim rule. For example, "<span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>."</td>    </tr>    <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">     <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Attribute store</td>     <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select <span class="bold">Active Directory</span> from the drop-down menu.</td>    </tr>    <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">     <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">LDAP Attribute</td>     <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This can be any type of attribute. We recommend using <span class="bold">SAM-Account-Name</span> for this attribute.</td>    </tr>    <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">     <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Outgoing Claim Type</td>     <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">You must select <span class="bold">Name ID</span> as the outgoing claim type</td>    </tr>   </tbody>  </table> </li>` `<li> <p> (Optional) In order to establish auto provisioning, add the following additional claims in both the LDAP Attribute and Outgoing Claim Type:</p>  <ul>   <li style="font-weight: normal;"> <span class="bold">Given Name</span></li>   <li style="font-weight: normal;"><span class="bold">Surname</span> </li>   <li style="font-weight: normal;"><span class="bold">E-Mail Address</span> </li>  </ul> </li>` `<li>Click <span class="bold">Finish</span>, then click <span class="bold">OK</span> on the next screen.</li>` `<li> <p>Right-click the new <span class="bold">Relying Party Trust</span>, then select <span class="bold">Properties</span>.</p> <p> <img src="assets/screen-shot-2014-10-22-at-3.03.47-pm-350x129.png" alt="" style="width: 350;height: 129;"> </p> </li>` `<li>Select the<span class="bold"> Advanced Tab</span>. And under <span class="bold">Secure Hash Algorithm</span> select SHA-1 or SHA-256.</li>` 





>[!NOTE]
>
>What you select under Secure Hash Algorithm here must match the Secure Hash Algorithm field in *`Workfront`* under Setup > System > Single Sign-ON (SSO).


![](assets/screen-shot-2014-10-22-at-3.04.55-pm-350x232.png)




11. Continue to the following section [Upload the metadata file and test the connection](#uploading-metadata-file).


### Upload the metadata file and test the connection {#upload-the-metadata-file-and-test-the-connection}




1.  Open a browser and navigate to https://*<yourserver>*/FederationMetadata/2007-06/FederationMetadata.xml.   



   This should download a Metadata file FederationMetadata.xml file.

1. Click `Choose File` under `Populate fields from Identity Provider Metadata`, and select the `FederationMetadata.xml` file.

1. (Optional) If the certificate information did not populate with the metadata file, you can upload a file separately. Select `Choose File`in the `Certificate`section.

1.  Click `Test Connection`. If set up correctly, you should see a page similar to the one shown below:  



   ![](assets/screen-shot-2014-10-22-at-3.09.17-pm-adobe-branding-350x120.png)




   >[!NOTE]
   >
   >If you want to set up attribute mapping, ensure that you copy the attributes from the Test Connection into the Directory Attribute. For more information, see Mapping User Attributes.  




1.  Select `Admin Exemption` to allow *`Workfront administrators`* to log in using *`Workfront`* credentials with the bypass url. 


   Bookmarks pointing to *<yourdomain>*.my.workfront.com/login bypass the redirect.

1. Select the `Enable` box to enable the configuration.
1. Click `Save`.




## About updating users for SSO {#about-updating-users-for-sso}

Following this guide, the `SSO Username` will be their `Active Directory Username`. 


As a *`Workfront administrator`*, you can bulk update users for SSO. For more information about updating users for SSO, see [Update users for single sign-on](update-users-SSO.md).


As a *`Workfront administrator`*, you can also manually assign a Federation ID editing the user's profile and completing the Federation ID field. For more information about editing a user, see [Edit a user's profile](edit-a-users-profile.md).


>[!NOTE]
>
>When editing users' profiles to include a Federation ID, selecting `Only Allow SAML 2.0 Authentication` removes the ability to log in to *`Workfront`* using the bypass url (*<yourdomain>*.my.workfront.com/login). 


