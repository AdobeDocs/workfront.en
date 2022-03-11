---
filename: wf-preview-sandbox-environment
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: The Adobe Workfront Preview Sandbox Environment
description: There are two testing environments for Workfront that are replicas of your Workfront production environment:
---

# The Adobe Workfront Preview Sandbox Environment

There are two testing environments for Workfront that are replicas of your Workfront production environment:

* The Preview Sandbox

  The Preview Sandbox is a testing environment that serves as a replica of your live environment and is refreshed each weekend by Workfront. For example, data added to your live environment on Friday appears in your Preview Sandbox by the following Monday.  
  All support packages have access to the Preview Sandbox.

* The Custom Refresh Sandbox

  The Custom Refresh Sandbox is a separate testing environment which is refreshed manually by you. There is an additional cost to obtain the Custom Refresh Sandbox. For more information about the Custom Refresh Sandbox, see [The Adobe Workfront Custom Refresh Sandbox environment](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><span class="bold">Standard Support Package</span> </p> </th> 
   <th> <p><span class="bold">Plus, Preferred, and Enterprise Support Packages</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Preview Sandbox</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Custom Refresh Sandbox</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Preview Sandbox

The Preview Sandbox serves as an environment where users in your organization can safely test and work with data from the production environment without affecting the production environment.

The Preview Sandbox contains your actual production data; however, it refreshes every weekend so the data can be up to one week behind the production environment. Items created since the last refresh time are in the Preview Sandbox environment until the following refresh.

Data flows uni-directionally, from Production to Preview, and not in reverse. A refresh of the Preview environment is always scheduled by Workfront each weekend. For more information on the specific day and time of the refresh, go to [status.adobe.com](https://status.adobe.com/).

Preview Sandbox also allows Workfront to deploy new features in a safe environment, before they are ready to be deployed to Production. You can test the new features and give Workfront feedback on their functionality by accessing the Preview Sandbox. For this reason, the code of the Preview Sandbox is always ahead of the Production code, although your data is refreshed weekly.

The preview environment is ideal for running trainings, testing out new features, and determining setup functionality.

>[!NOTE]
>
>When you access the Preview Sandbox, notice the blue banner at the top of the screen. The banner cannot be removed while you are working in this environment.
>
>The name of the environment you are accessing (Preview) and the release version of the code display on the banner. Click `See what’s new` for information about that release.

## Accessing the Preview Sandbox

By default, as a Workfront administrator, you have access to the Preview Sandbox environment. If you cannot access the Preview Sandbox environment as described in this section, contact your Workfront administrator or our Customer Support team.

* [Accessing the Preview Sandbox from the Workfront Interface](#accessing-the-preview-sandbox-from-the-workfront-interface) 
* [Accessing the Preview Sandbox Using a URL](#accessing-the-preview-sandbox-with-a-url)

### Accessing the Preview Sandbox from the Workfront Interface

As a Workfront administrator, you can access the Preview Sandbox via the Workfront interface.

To access the Preview Sandbox:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Preferences</span>.</li> 
 <li value="3"> In the <span class="bold">Test Environments</span> section, click <span class="bold">Sandbox Preview</span>.</li> 
 <li value="4"> <p> Log in with your Preview credentials.</p> <p>These should be the same as your production credentials, unless you changed them in Production after the Preview refresh happened. The logins are synchronized only when a refresh occurs. They do not synchronize automatically. </p> </li> 
</ol>

### Accessing the Preview Sandbox Using a URL

* [Accessing the Preview Sandbox for Accounts on Cluster 1,2,3, and 5](#preview-through-url-on-cluster-1-2-3) 
* [Accessing the Preview Sandbox for Accounts on Cluster 4 (EMEA Accounts)](#preview-cluster-4)

#### `Accessing the Preview Sandbox for Accounts on Cluster 1,2,3, and 5`

Historically, you accessed the Preview Sandbox by going to [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&sa=D&sntz=1&usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg).

This URL is no longer supported and it has not been redirected to our new URL for the Preview Sandbox environment. The new correct URL for the Preview Sandbox is: [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&sa=D&sntz=1&usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ).

>[!NOTE]
>
>If you had bookmarks linking to the old URL for the Preview Sandbox, please make note of this change and update the URL in your bookmarks.

To log into the Preview Sandbox using a URL:

1. Navigate to this URL: ` [https://companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)  
   `

   If you are an EMEA customer and your account is on Cluster 4, see the section [Accessing the Preview Sandbox for Accounts on Cluster 4 (EMEA Accounts)](#preview-cluster-4) in this article.

1. Log in using your Preview credentials.

   Your Preview credentials should be the same as your production credentials, unless you changed them in Production after the Preview refresh happened. The logins are synchronized only when a refresh occurs. They do not synchronize automatically.

#### `Accessing the Preview Sandbox for Accounts on Cluster 4 (EMEA Accounts)`

To log into the Preview Sandbox using a URL:

1. Navigate to this URL: `https://companyname.preview.workfront.com/`.

   You may also access the Preview Sandbox by going to [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Log in using your Preview credentials.

   Your Preview credentials should be the same as your production credentials, unless you changed them in Production after the Preview refresh happened. The logins are synchronized only when a refresh occurs. They do not synchronize automatically.

## Receiving Emails from the Preview Sandbox

Workfront disables all email communication from the Preview Sandbox environment. If you want to receive email notifications from the Preview Sandbox environment, you must enable this functionality in your user settings. For more information about enabling email notifications in the Preview Sandbox environment, see [Enable delivery of emails from the Preview Sandbox environment](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Report delivery and push notifications on the mobile app are always disabled for the Preview Sandbox environment. Neither you nor the Workfront administrator can enable report delivery or push notifications for the mobile app when you access the Preview Sandbox environment.
>
>For more information about report deliveries for the production environment, see [Report delivery overview](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).
>
>For more information about push notifications on the mobile app for the production environment, see the section in .

## Single Sign-On (SSO)

If you are using SSO, work with our Customer Support team to ensure it is properly configured so that you can use your SSO credentials to log in to the Preview Sandbox. If your initial login fails, please contact your regular support contact or Workfront administrator for assistance.

For more information about Single Sign-On, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

## Configuring Single Sign-On in the Preview Sandbox

If you want to configure your Preview Sandbox to work with a Single Sign-On solution, you can do so by configuring it separately from your Production environment. The SSO configuration in the Preview Sandbox is independent from your SSO configuration in the Production environment.

When your Preview Sandbox refreshes (every weekend), the SSO information is not copied from your Production environment to overwrite the Preview Sandbox configuration.

The steps for configuring single sign-on in the Preview Sandbox are similar to those for configuring it in the Production environment.  
For more information about configuring Workfront with SSO, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Preview environment performance and availability

Workfront Preview environments are not intended for performance or load testing. Rather, use these environments to validate feature functionality with your organization's existing workflows.

Workfront Preview environments are intended to be always available.

Any outage to a Workfront Preview environment during regular business hours will be a first priority immediately after any Production issues are resolved if any exist.

Any outage to a Workfront Preview environment on weekends (Saturdays and Sundays) will be addressed so that the environment is running for business hours on Monday.
