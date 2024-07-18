---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] with updated security measures
description: Google recently introduced restrictions on how users can use their API. This article describes how to connect [!DNL Adobe Workfront Fusion] to Google, accounting for these update security measures.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
---
# Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] with updated security measures

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restrictions

[!DNL Google] introduced restrictions on how users can use their API as of June 1st, 2020. These security measures protect [!DNL Google] users from leakage or misuse of their personal data on [!DNL Google]. The restrictions are related to the [!DNL Gmail] and [!DNL Google Drive] apps. For more information about these restrictions, see "Additional Requirements for Specific API Scopes" in the [[!DNL Google] API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

To access restricted scopes, the connected service ([!DNL Adobe Workfront Fusion] or any other service that wants to access the user's data via the API) must be verified and must have a Letter of Assessment to prove that the service is secure and transparent about how they use the data. [!DNL Workfront Fusion] complies with all of [!DNL Google]'s requirements for access to restricted scopes. However, most of the third-party connected services in [!DNL Workfront Fusion] don't have the Letter of Assessment, and therefore don't comply with [!DNL Google] terms. Because of that, [!DNL Workfront Fusion] is not permitted to send data to these services.

## Exceptions to [!DNL Google Services] restrictions

There are a few exceptions that make it possible to send data to an unapproved third-party service that doesn't have the Letter of Assessment without violating any of the new restrictions. They differ based on [!DNL Google Workspace] with the [!DNL Workfront Fusion] OAuth client, [!DNL Google Workspace] with another OAuth client, or [!DNL @gmail.com] and [!DNL @google.mail.com].

* [[!DNL Google Workspace] with [!DNL Workfront Fusion] OAuth client](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] with another OAuth client](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] and [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] with [!DNL Workfront Fusion] OAuth client

[!DNL Workfront Fusion] uses the [!UICONTROL Domain-wide Installation] exception. Domain-wide Installation is suited for [!DNL Google Workspace] users, and allows users to integrate unapproved services without any limitations. If you are a Google Workspace user, you don't have to perform any additional steps and can directly connect to unapproved services.

### [!DNL Google Workspace] with another OAuth client 

[!DNL Google Workspace] users that prefer to use their own OAuth client instead of using the [!DNL Workfront Fusion] OAuth client can connect to [!DNL Google Services] through the [!UICONTROL Internal] Use approach. This option is intended for advanced users. For instructions, see [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] and [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

User that access [!DNL Google Services] through [!DNL @gmail.com] or [!DNL @googlemail.com] can connect to [!DNL Google Services] through the Personal Use approach. This option is intended for advanced users. For instructions, see [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQ

* [What apps in [!DNL Adobe Workfront Fusion] are affected?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Do I have a [!DNL Google Workspace] account?](#do-i-have-a-g-suite-account)
* [What should I do if I'm [!DNL @gmail.com] or [!DNL @googlemail.com] user?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [What should I do if I'm a [!DNL Google Workspace] user?](#what-should-i-do-if-im-a-g-suite-user)

### What apps in [!DNL Adobe Workfront Fusion] are affected? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail], and Email (connected to [!DNL Gmail] account).

### Do I have a [!DNL Google Workspace] account? {#do-i-have-a-g-suite-account}

If your email address ends with [!DNL @gmail.com] or [!DNL @googlemail.com] your account is not a [!DNL Google Workspace] account. If your [!DNL Google] account ends with custom domain such as @my-company.com then it is a [!DNL Google Workspace] account.

### What should I do if I'm [!DNL @gmail.com] or [!DNL @googlemail.com] user? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

These new restrictions only apply if you are integrating [!DNL Google Drive] or [!DNL Gmail]. If you want to connect to [!DNL Google Drive] or [!DNL Gmail], you can

* Switch to [!DNL Google Workspace]

   or

* Create a custom OAuth client. This option is intended for advanced users.

   For instructions, see [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

If you want to integrate any other service than [!DNL Google Drive] or [!DNL Gmail], these restrictions do not apply.

For instructions about connecting other [!DNL Google Services] to [!DNL Workfront Fusion], see [Connect the module's app or web service to [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) in the article [Create a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### What should I do if I'm a [!DNL Google Workspace] user? {#what-should-i-do-if-im-a-g-suite-user}

There is no required action.
