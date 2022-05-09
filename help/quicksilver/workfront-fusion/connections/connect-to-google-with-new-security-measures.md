---
filename: connect-to-google-with-new-security-measures
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Connect Adobe Workfront Fusion to Google Services with updated security measures
description: You must have the following access to use the functionality in this article - EDIT ME.
---

# Connect Adobe Workfront Fusion to Google Services with updated security measures

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Google Services restrictions

Google introduced restrictions on how users can use their API as of June 1st, 2020. These security measures protect Google users from leakage or misuse of their personal data on Google. The restrictions are related to the Gmail and Google Drive apps. For more information about these restrictions, see "Additional Requirements for Specific API Scopes" in the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

To access restricted scopes, the connected service (Adobe Workfront Fusion or any other service that wants to access the user's data via the API) must be verified and must have a Letter of Assessment to prove that the service is secure and transparent about how they use the data. Workfront Fusion complies with all of Google’s requirements for access to restricted scopes. However, most of the third-party connected services in Workfront Fusion don't have the Letter of Assessment, and therefore don't comply with Google terms. Because of that, Workfront Fusion is not permitted to send data to these services.

## Exceptions to Google Services restrictions

There are a few exceptions that make it possible to send data to an unapproved third-party service that doesn’t have the Letter of Assessment without violating any of the new restrictions. They differ based on G Suite with the Workfront Fusion OAuth client, G Suite with another OAuth client, or @gmail.com and @google.mail.com.

* [G suite with Workfront Fusion OAuth client](#g-suite-with-workfront-fusion-oauth-client) 
* [G suite with another OAuth client](#g-suite-with-another-oauth-client) 
* [@gmail.com and @googlemail.com](#gmail-com-and-googlemail-com)

### G suite with Workfront Fusion OAuth client {#g-suite-with-workfront-fusion-oauth-client}

Workfront Fusion uses the Domain-wide Installation exception. Domain-wide Installation is suited for G Suite users, and allows users to integrate unapproved services without any limitations. If you are a G Suite user, you don't have to perform any additional steps and can directly connect to unapproved services.

### G suite with another OAuth client {#g-suite-with-another-oauth-client}

G Suite users that prefer to use their own OAuth client instead of using the Workfront Fusion OAuth client can connect to Google Services through the Internal Use approach. This option is intended for advanced users. For instructions, see [Connect Adobe Workfront Fusion to Google Services using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### @gmail.com and @googlemail.com  {#gmail-com-and-googlemail-com}

User that access Google Services through @gmail.com or @googlemail.com can connect to Google Services through the Personal Use approach. This option is intended for advanced users. For instructions, see [Connect Adobe Workfront Fusion to Google Services using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQ

* [What apps in Adobe Workfront Fusion are affected?](#what-apps-in-adobe-workfront-fusion-are-affected) 
* [Do I have a G Suite account?](#do-i-have-a-g-suite-account) 
* [What should I do if I'm @gmail.com or @googlemail.com user?](#what-should-i-do-if-i-m-gmail-com-or-googlemail-com-user) 
* [What should I do if I'm a G Suite user?](#what-should-i-do-if-i-m-a-g-suite-user)

### What apps in Adobe Workfront Fusion are affected? {#what-apps-in-adobe-workfront-fusion-are-affected}

Google Drive, Gmail, and Email (connected to Gmail account).

### Do I have a G Suite account? {#do-i-have-a-g-suite-account}

If your email address ends with @gmail.com or @googlemail.com your account is not a G Suite account. If your Google account ends with custom domain such as @my-company.com then it is a G Suite account.

### What should I do if I'm @gmail.com or @googlemail.com user? {#what-should-i-do-if-i-m-gmail-com-or-googlemail-com-user}

These new restrictions only apply if you are integrating Google Drive or Gmail. If you want to connect to Google Drive or Gmail, you can

* Switch to G Suite

  or 

* Create a custom OAuth client. This option is intended for advanced users.

  For instructions, see [Connect Adobe Workfront Fusion to Google Services using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

If you want to integrate any other service than Google Drive or Gmail, these restrictions do not apply.

For instructions about connecting other Google Services to Workfront Fusion, see [Connect the module's app or web service to Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md#connect) in the article [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

### What should I do if I'm a G Suite user? {#what-should-i-do-if-i-m-a-g-suite-user}

There is no required action.
