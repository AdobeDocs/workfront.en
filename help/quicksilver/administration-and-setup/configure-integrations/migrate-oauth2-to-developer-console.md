---
title: Migrate from Workfront OAuth2 to Adobe Developer Console
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Workfront's legacy custom OAuth2 application service is being retired. Learn what's changing, who is affected, and how to migrate your custom integrations to Adobe Developer Console.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
---
# Migrate from Workfront OAuth2 to Adobe Developer Console

Workfront's legacy custom OAuth2 application service (the integrations you set up under **Setup** > **System** > **OAuth2**) is being retired. Going forward, all custom integrations that authenticate against Workfront must use the Adobe Developer Console (developer.adobe.com) authentication flow instead.

This change affects any custom-built integration, script, or third-party tool that currently authenticates using a Workfront-issued OAuth2 client ID and secret. It does not affect how you log in to Workfront, and it does not affect standard, Adobe-managed integrations such as the packaged Microsoft Teams or Slack integrations, which Adobe is migrating separately.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront access level configurations</td> 
   <td><p>System Administrator</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Developer Console rights</td> 
   <td><p>Full IMS Org admin rights are required to access Adobe Developer Console for Workfront. This is broader than a Workfront product admin role, since it manages the whole Adobe org and all products under it.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Key dates

|Date|Milestone|What it means for you|
|---|---|---|
|November 1, 2026|New app creation disabled|You can no longer create new custom OAuth2 applications in Workfront. Existing applications continue to work.|
|February 1, 2027|Legacy service retired|Existing custom OAuth2 applications stop working entirely. Any integration that has not migrated to Adobe Developer Console loses access to the Workfront API at this point.|

>[!IMPORTANT]
>
>We highly recommend planning and completing your migration before November 1, 2026, so your integrations continue running without interruption, and so you are not migrating against the February 1, 2027 hard deadline.

## Affected organizations

Your organization is affected by this change if it has any integration, script, or tool that connects to Workfront using a custom OAuth2 client ID and secret issued through Workfront's legacy OAuth2 setup screen. Common examples include:

* Custom-built integrations your engineering team maintains against the Workfront API.
* Third-party or partner-built connectors configured with a Workfront-issued client ID. We recommend checking with your vendor if you're not sure how their integration authenticates.
* Internal automation, reporting, or data-sync scripts that call the Workfront API directly.

If you don't know whether your organization has any of these, your Workfront administrator can check the OAuth2 applications list under **Setup** > **System** > **OAuth2** to see what's currently registered. For information, see [View and Manage Custom OAuth2 Applications](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md).

## Understand Adobe Developer Console authentication types

Adobe Developer Console supports more than one way to authenticate. You can select the type that matches how your integration works:

* **Server-to-Server Authentication**: For an application running on your backend that calls Adobe APIs on behalf of your organization, with no end user involved. This is the closest match to the legacy Workfront OAuth2 pattern worked with client IDs and secrets, and is the type most custom Workfront integrations, scripts, and automations should use.
* **User Authentication**: For cases where an Adobe user needs to sign in and grant consent before your application can view or edit their data. If your integration needs to act on behalf of a specific signed-in Workfront user rather than your organization as a whole, use this type instead.

   If you choose User Authentication, there are three further options depending on your application's architecture:

   * **OAuth Web App**: For applications with a frontend UI and a backend server. The server securely stores the client secret and fetches tokens.
   * **OAuth Single-Page App**: For browser-only web applications with no backend server. The web app itself fetches tokens.
   * **OAuth Native App**: For mobile or desktop applications that run natively on a device and have no backend server. The native app fetches tokens.

Most organizations migrating a backend integration, script, or automation off the legacy OAuth2 service want Server-to-Server Authentication.

## Feature comparison: legacy OAuth2 vs. Adobe Developer Console

The legacy Workfront OAuth2 service (fount in **Setup** > **System** > **OAuth2 Applications**) offers three application types, with a limit of 10 OAuth2 applications per Workfront instance. Here's how these aspects compare to Adobe Developer Console:

|Legacy Workfront type|Flow / auth method|Developer Console equivalent|Fit|
|---|---|---|---|
|Machine to Machine Application (CLIs, daemons, backend scripts)|JWT with public/private key pair|Server-to-Server Authentication|Same purpose of not having the end user involved, but the mechanism changes. The legacy flow uses a public/private key pair and JWT, while Server-to-Server uses a client ID and client secret with an OAuth client-credentials grant. This is not a drop-in credential swap. The integration's auth code needs to change, not just the credential values. For information, see [Using JWT flow for custom OAuth 2 applications](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md).|
|Web Application (server-side apps: Go, Java, .NET, Node, PHP)|OAuth 2.0 Authorization Code flow|OAuth Web App (under User Authentication)|Closest 1:1 match. This has the same flow, and the same basic shape where a backend server stores the client secret. For information, see [Authorization code flow for custom OAuth 2 applications](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md).|
|Single Page Web Application (JS, Angular, React, Vue)|Authorization Code flow with PKCE, no client secret|OAuth Single-Page App (under User Authentication)|Closest 1:1 matchThis has the same PKCE-based, secret-less flow. For information, see [Using PKCE flow for OAuth 2 applications](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md).|
|(no legacy equivalent)|—|OAuth Native App (under User Authentication)|This is a new capability. Legacy Workfront OAuth2 has no dedicated type for native mobile or desktop applications.|

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## Migration procedure

### If you are a Workfront System Administrator

>[!NOTE]
>
>If you're a Workfront product administrator but not an Org administrator, you need to work with your Org administrator to complete this migration, or ask to be made one.

1. Log in to [developer.adobe.com](developer.adobe.com) and create a new Project. Projects are how the console organizes different integrations or client apps.
1. From the Project, add an API, and select **Adobe Workfront**. This API is under the Experience Cloud category. All Workfront APIs, including Planning, Workflow, and Review and Approvals, share this single API.
1. Select the **Server-to-Server** authentication option, then choose the correct instance if your IMS Org has more than one Workfront instance.

   For guidance on choosing an authentication type, see [Understand Adobe Developer Console authentication types](#understand-adobe-developer-console-authentication-types) in this article.
1. On the Project page, open the details of your new OAuth Server-to-Server credential to find your Client ID, Client Secret, and the information needed to generate access tokens.
1. Update your integration, script, or tool to authenticate with these new credentials in place of the old Workfront OAuth2 client ID and secret.
1. Confirm access in Workfront. Creating the API client automatically adds it as the Workfront user "`techacct`". By default, it's added as a Contributor with limited access, but you can adjust its access level like you would for any other user. 
1. (Optional) To grant the `techacct` user administrator rights, add the Technical Account's email as an administrator of the relevant Product Profile in Admin Console.
1. Test the integration end-to-end.
1. Retire the old OAuth2 application entry in Workfront after you've confirmed the new connection is working.

For full step-by-step details and screenshots, see [Gaining access](https://developer.adobe.com/workfront-apis/guides/gaining_access/) in Adobe's Developer Console documentation.

### If you are not a System Administrator

You need to loop in your organization's IMS Org administrator to complete the migration, since setting up the new credential in Adobe Developer Console requires that level of access. If you manage or maintain an integration but so know know who your organization's IMS Org administrator is, contact one of the following:

   * Your Workfront account team
   * Your internal IT team
   * Your engineering contact

## If you don't migrate

Integrations still using the legacy OAuth2 client ID/secret pattern after February 1, 2027 stop being able to authenticate against the Workfront API, and any dependent workflow, sync, or automation fails. There is no extension planned past this date, so migrate your integrations well ahead of it.

## Frequently asked questions

**Does this affect the packaged integrations Adobe provides, such as Slack or Microsoft Teams?**

No. Adobe-managed global applications are being migrated by Adobe directly and don't require action on your part.

**Will my existing integration stop working before February 1, 2027?**

No. Existing custom OAuth2 applications continue to function normally through February 1, 2027. Only the ability to create new custom OAuth2 applications is affected, starting November 1, 2026.

**Is there a cost to migrating?**

No, there is no additional cost associated with authenticating through Adobe Developer Console.

**Where can I get help?**

Reach out to your Workfront account team or open a support case if you have questions about your specific integration or timeline. For the official, up-to-date setup walkthrough with screenshots, see [Gaining access](https://developer.adobe.com/workfront-apis/guides/gaining_access/) in Adobe's Developer Console documentation.
