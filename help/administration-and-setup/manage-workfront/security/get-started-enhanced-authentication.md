---
filename: get-started-enhanced-authentication
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
---



# Enhanced Authentication overview {#enhanced-authentication-overview}

The highlighted information on this page refers to functionality not yet generally available. It will be available at some point in the future.


>[!IMPORTANT] {type="important"}
>
>The functionality described on this page applies only to organizations that are not yet onboarded to the Adobe Business Platform.
>
>
>If your organization has been onboarded to the Adobe Business Platform, authentication is handled automatically as part of that integration. You do not need to configure or enable this functionality.
>
>
>For a list of procedures that differ based on whether your organization is migrated to Adobe IMS, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



*`Adobe Workfront`* is changing the system management of users and passwords. These changes will roll out in a phased release called **Enhanced Authentication** experience. Enhanced Authentication offers users a more consistent and secure sign-in experience across all *`Workfront`* products and services.


The following table provides details about current and future functionality:


>[!IMPORTANT] {type="important"}
>
>`Most customers are currently using Legacy Authentication and some are using Enhanced Authentication 1.0.  
  
>To verify which type of authentication you are currently using, go to *your_domain*.my.workfront.com/login. If you are redirected to /auth/login, then you are using Enhanced Authentication 1.0.  
  
>If you are redirected to https://login-a-xx.workfront.com/, where 'xx' could be US (United States), EU (Europe), or GCP (Google Cloud Platform) depending on your location/platform, then you are using Enhanced Authentication 2.0.  
  
>All customers will be moving to Enhanced Authentication 2.0 by the end of 2021.` 



<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" data-mc-conditions=""> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Feature</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Legacy Authentication</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Enhanced Authentication 1.0</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p>Enhanced Authentication 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td colspan="3" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span class="bold">Login options</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Enable a single username to be used for all <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> products and services, including training, support, and others</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Not available</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Not available</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Allow using the same email address across <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> instances</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Email addresses are case-insensitive</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>✓</p> <p>Multiple users cannot have the same email address if the address differs only by case.&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p class="preview">✓</p> <p class="preview">Multiple users cannot have the same email address if the address differs only by case. </p> <p class="preview"><span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span> will be notified toward the end of 2019 to begin fixing duplicate email addresses.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td colspan="3" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span class="bold">Password management options</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Instigate a password reset email for a user as the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span></p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Not available&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>✓</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Set a temporary password for a user as the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span></p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>✓</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Not planned</p> <p>This functionality is not a security best practice</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p class="preview">Not planned</p> <p class="preview">This functionality is not a security best practice</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td colspan="3" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">Password policy requirements</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Require users to reset passwords after a certain timeframe</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Not planned</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Restrict users from using a previous password&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Not planned&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Safeguard against incorrect password entry attempts&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>✓&nbsp;</p> <p>Locks the account after 5 incorrect password entry attempts. The wait time required after lockout is configured by the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span></p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>✓</p> <p>Wait time is exponentially increased after each successive incorrect password based on industry best practices; the time required is not configurable by the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span></p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p class="preview">✓</p> <p class="preview">Uses a lock-out algorithm that proactively blocks a variety of suspicious behavior.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Require a mix of lowercase, uppercase, numbers, and special characters</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>✓&nbsp;</p> <p>Enhanced flexibility in choosing specific requirements</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Set a minimum password length&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Not available&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> ✓&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td colspan="3" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">Single Sign-On Protocol support</span>&nbsp;&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Supports SSO integrations that are compliant with Active Directory and LDAP protocols</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> ✓&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p> Deprecated</p> <p>Active Directory, Azure, and LDAP&nbsp;systems should use SAML 2.0</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p class="preview">Deprecated</p> <p class="preview">Active Directory, Azure, and LDAP&nbsp;systems can be configured with encrypted SAML 2.0 or OpenID Connect.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Supports SSO protocols that are compliant with SAML 2.0&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> ✓&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Supports Open ID&nbsp;Connect protocols</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Not available</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Not available</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p> Configure the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> login page to always redirect to the identity provider login page </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Enabled by default and cannot be disabled</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>✓</p> <p><span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can configure the login page to redirect to the identity provider login page, or can configure a login button or buttons.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p class="preview">✓</p> <p class="preview"> <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span> can configure the login page to redirect to the identity provider login page, or can configure a login button or buttons.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Allow each instance to enable multiple SSO&nbsp;providers</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>N/A</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Not planned</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td colspan="3" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">Environment support</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>A single username and password for Preview environments</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Not available</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Not available</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p class="preview">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>A single username and password for Sandbox environments</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Not available</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Not available</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p class="preview">✓</p> </td> 
  </tr> 
 </tbody> 
</table>

