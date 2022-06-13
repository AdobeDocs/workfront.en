---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Enhanced Authentication overview
description: The highlighted information on this page refers to functionality not yet generally available. It will be available at some point in the future.
feature: System Setup and Administration
role: Admin
---

# Enhanced Authentication overview

The highlighted information on this page refers to functionality not yet generally available. It will be available at some point in the future.

>[!IMPORTANT]
>
>The functionality described on this page applies only to organizations that are not yet onboarded to the Adobe Business Platform.
>
>If your organization has been onboarded to the Adobe Business Platform, authentication is handled automatically as part of that integration. You do not need to configure or enable this functionality.
>
>For a list of procedures that differ based on whether your organization is migrated to Adobe IMS, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront is changing the system management of users and passwords. These changes will roll out in a phased release called **Enhanced Authentication** experience. Enhanced Authentication offers users a more consistent and secure sign-in experience across all Workfront products and services.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

The following table provides details about current and future functionality:

>[!IMPORTANT]
>
>Most customers are currently using Legacy Authentication and some are using Enhanced Authentication 1.0.  
> 
>To verify which type of authentication you are currently using, go to *your_domain*.my.workfront.com/login. If you are redirected to /auth/login, then you are using Enhanced Authentication 1.0.  
> 
>If you are redirected to https://login-a-xx.workfront.com/, where 'xx' could be US (United States), EU (Europe), or GCP (Google Cloud Platform) depending on your location/platform, then you are using Enhanced Authentication 2.0.  
>
>All customers will be moving to Enhanced Authentication 2.0 by the end of 2021.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Feature</strong> </p> </th> 
   <th><strong>Legacy Authentication</strong> </th> 
   <th><strong>Enhanced Authentication 1.0</strong> </th> 
   <th> <p>Enhanced Authentication 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Login options</strong> </p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Enable a single username to be used for all Workfront products and services, including training, support, and others</p> </td> 
   <td>Not available</td> 
   <td> <p>Not available</p> </td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Allow using the same email address across Workfront instances</p> </td> 
   <td> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
   <td> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
   <td> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Email addresses are case-insensitive</p> </td> 
   <td> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
   <td> <p>✓</p> <p>Multiple users cannot have the same email address if the address differs only by case.&nbsp;</p> </td> 
   <td> <p class="preview">✓</p> <p class="preview">Multiple users cannot have the same email address if the address differs only by case. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        For more information, see . 
      </MadCap:conditionalText>
     --></p> <p class="preview">Workfront administrators will be notified toward the end of 2019 to begin fixing duplicate email addresses.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Password management options</strong> </p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Instigate a password reset email for a user as the Workfront administrator</p> </td> 
   <td> <p>Not available&nbsp;</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Set a temporary password for a user as the Workfront administrator</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Not planned</p> <p>This functionality is not a security best practice</p> </td> 
   <td> <p class="preview">Not planned</p> <p class="preview">This functionality is not a security best practice</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Password policy requirements</strong> </p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Require users to reset passwords after a certain timeframe</p> </td> 
   <td>✓</td> 
   <td> <p>Not planned</p> </td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Restrict users from using a previous password&nbsp;</p> </td> 
   <td>✓</td> 
   <td>Not planned&nbsp;</td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Safeguard against incorrect password entry attempts&nbsp;</p> </td> 
   <td> <p>✓&nbsp;</p> <p>Locks the account after 5 incorrect password entry attempts. The wait time required after lockout is configured by the Workfront administrator</p> </td> 
   <td> <p>✓</p> <p>Wait time is exponentially increased after each successive incorrect password based on industry best practices; the time required is not configurable by the Workfront administrator</p> </td> 
   <td> <p class="preview">✓</p> <p class="preview">Uses a lock-out algorithm that proactively blocks a variety of suspicious behavior.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Require a mix of lowercase, uppercase, numbers, and special characters</p> </td> 
   <td>✓</td> 
   <td> <p>✓&nbsp;</p> <p>Enhanced flexibility in choosing specific requirements</p> </td> 
   <td> <p class="preview">✓</p> <p class="preview"> <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        To learn more about setting password requirements, see . 
      </MadCap:conditionalText>
     --> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Set a minimum password length&nbsp;</p> </td> 
   <td> Not available&nbsp;</td> 
   <td> ✓&nbsp;</td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p class="preview">✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>Single Sign-On Protocol support</strong>&nbsp;&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supports SSO integrations that are compliant with Active Directory and LDAP protocols</p> </td> 
   <td> ✓&nbsp;</td> 
   <td> <p> Deprecated</p> <p>Active Directory, Azure, and LDAP&nbsp;systems should use SAML 2.0</p> </td> 
   <td> <p class="preview">Deprecated</p> <p class="preview">Active Directory, Azure, and LDAP&nbsp;systems can be configured with encrypted SAML 2.0 or OpenID Connect.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supports SSO protocols that are compliant with SAML 2.0&nbsp;</p> </td> 
   <td>✓</td> 
   <td> ✓&nbsp;</td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supports Open ID&nbsp;Connect protocols</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Configure the Workfront login page to always redirect to the identity provider login page </p> </td> 
   <td> Enabled by default and cannot be disabled</td> 
   <td> <p>✓</p> <p>Workfront administrator can configure the login page to redirect to the identity provider login page, or can configure a login button or buttons.</p> </td> 
   <td> <p class="preview">✓</p> <p class="preview"> Workfront administrators can configure the login page to redirect to the identity provider login page, or can configure a login button or buttons.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Allow each instance to enable multiple SSO&nbsp;providers</p> </td> 
   <td> <p>N/A</p> </td> 
   <td> <p>Not planned</p> </td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Environment support</strong> </p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>A single username and password for Preview environments</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>A single username and password for Sandbox environments</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p class="preview">✓</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p class="preview">✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p class="preview">✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

