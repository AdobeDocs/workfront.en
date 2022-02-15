---
filename: log-in-to-workfront
product-area: user-management
navigation-topic: manage-your-workfront-account
---



# Log in to *`Adobe Workfront`* {#log-in-to-adobe-workfront}

You need the following information to log in to *`Adobe Workfront`*:



*  `A login URL:` This is your company's unique URL, which should have this format: `yourCompanyDomain.my.workfront.com`.  
  If you are set up for single sign-on (SSO), your URL might have been changed by your *`Workfront administrator`*. For more information about logging in to *`Workfront`* with SSO, see [Log in to Workfront with SSO](#logging-in-to-workfront-with-sso) in this article.


  The domain name for your company is established by *`Workfront`*. To change your domain name, contact our Customer Support team. For information about how to contact our Customer Support team, see [Contact Customer Support](contact-customer-support.md).

* `A username:` Your *`Workfront administrator`* sets up your user name.

*  `A password:` If your system is not set up for SSO, you set up your *`Workfront`* password after receiving an email invitation from the *`Workfront administrator`*.


  For more information about logging in to *`Workfront`* with SSO, see [Log in to Workfront with SSO](#logging-in-to-workfront-with-sso) in this article.


  For more information about receiving email invitations and creating a *`Workfront`* password, see [Receive email invitations and create a password for Adobe Workfront](receive-email-invitations.md).





## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your *`Workfront administrator`*.


## Log in to *`Workfront`* without SSO {#log-in-to-workfront-without-sso}

If your *`Workfront administrator`* did not set up *`Workfront`* to integrate with your SSO solution, you will need a new username and password for *`Workfront`*. For information about configuring *`Workfront`* to integrate with an SSO solution, see [Overview of single sign-on in Adobe Workfront](sso-in-workfront.md).


To log into *`Workfront`* using your *`Workfront`* username and password:



1.  Open a browser window, then type in the unique URL of your company, which should have the following format: `yourCompanyDomain.my.workfront.com`.


   For more information about what browsers are supported for *`Workfront`*, see [Adobe Workfront browser requirements](workfront-browser-requirements.md).

1.  In the login screen, enter your username and password.


   Your username is typically the email address associated with your *`Workfront`* account. If you forgot your password, see [Reset your password](reset-your-password.md).

1.  (Conditional) If your organization's Workfront login URL&nbsp;doesn't contain a domain, you must specify your domain in the Domain field.
1. Click `Login`.




## Log in to *`Workfront`* with SSO {#log-in-to-workfront-with-sso}

If your *`Workfront administrator`* integrated *`Workfront`* with a single sign-on solution, you should contact them for the information needed for your logging in to *`Workfront`*. For more information about integrating *`Workfront`* with an SSO solution, see [Overview of single sign-on in Adobe Workfront](sso-in-workfront.md).


To log in to *`Workfront`* using your SSO&nbsp;username and password:



1.  Open a browser window. 


   For more information about what browsers are supported for *`Workfront`*, see [Adobe Workfront browser requirements](workfront-browser-requirements.md).

1.  Type the unique URL of your company.


   If your *`Workfront administrator`* did not change the default *`Workfront`* URL, it should have the following format:


   `yourCompanyDomain.my.workfront.com` 

1.  Your *`Workfront administrator`* can ensure that you have the correct URL.
1.  On the login screen, enter your username and password.


   Your username and password are typically your network user name and password, which you use for all your applications. If you forgot your password or your user name, use the tools provided in your environment for resetting them, or contact your *`Workfront administrator`*.


   The look and feel of your login screen changes depending on what SSO solution you use and the way it was configured by your *`Workfront administrator`*.&nbsp;

1.  Complete your login.




## Log in to the Workfront mobile app {#log-in-to-the-workfront-mobile-app}




1.  Launch the Workfront mobile app, then type your organization's domain.


   This is the SAML domain if your organization is using SSO.


   >[!TIP] {type="tip"}
   >
   >This is typically your company name. If you are unsure, contact your *`Workfront administrator`*.



1.  Specify the *`Workfront`* URL for your company or the link to your SAML authentication portal.


   The *`Workfront`* URL should display in the following format*:*<![CDATA[                               ]]>  
   `yourDomain.my.workfront.com`


   For example:


   `swains.my.workfront.com` 

1.  If you are logging in with you SAML credentials, follow the login steps from your SAML authentication portal.


   Your *`Workfront administrator`* must enable SAML 2.0 authentication with the *`Workfront`* web application in order to log in with your SAML credentials. For information about how to enable SAML 2.0, see the section [Configure Adobe Workfront with SAML 2.0](configure-workfront-saml-2.md#saml-with-workfront-web-app) in the article [Configure Adobe Workfront with SAML 2.0](configure-workfront-saml-2.md). If you cannot log in as described in this section, contact your *`Workfront administrator`*.

1. Tap `Continue in browser`.
1. Specify the `Username`of your *`Workfront`* account or SAML user.

1. Specify the `Password` for your *`Workfront`* account or SAML user.

1. (Optional) Tap the eye icon to display or hide your password.
1.  Tap `SIGN IN`.


   You are signed in.

1.  Tap `Okay, got it` or `GETTING STARTED` to navigate through the tutorials displayed.


   These tutorials display only the first time you access the app. They display again only when you uninstall and reinstall the *`Workfront`* mobile app, or if you log in as another user. After closing out the tutorials, the area that displays is the one that you selected to show 



