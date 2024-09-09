---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: The [!DNL Adobe Workfront] Custom Refresh Sandbox Environment
description: The Custom Refresh Sandbox is an environment where you can test and work using data from your production environment. It's also ideal for running trainings and determining setup functionality.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
---
# The [!DNL Adobe Workfront] Custom Refresh Sandbox environment

The Custom Refresh Sandbox is an environment where you can test and work using data from your production environment. It's also ideal for running trainings and determining setup functionality.

>[!NOTE]
>
>This is different from the Preview Sandbox, which is also a testing environment that replicates your [!DNL Workfront] production environment.
>
>* New features are introduced to the Preview Sandbox before they become available in Production.
>* New features are not introduced to the Custom Refresh Sandbox before they become available in Production.
>
>  Also, there is an additional cost to obtain the Custom Refresh Sandbox that is not required for the Preview Sandbox.
>
>  For more information about the Preview Sandbox, see [The [!DNL Adobe Workfront] Preview Sandbox Environment](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>[!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] license</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>You must be a [!DNL Workfront] administrator. For information on [!DNL Workfront] administrators, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Support package</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred], or [!UICONTROL Enterprise]</p> <p>The standard support package does not have access to the Custom Refresh Sandbox, but it does have access to the Preview Sandbox.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Refreshing the Custom Refresh Sandbox

The Custom Refresh Sandbox contains your actual production data, and it does not refresh until you schedule it to do so. You can schedule a refresh any time is convenient for you, as frequently as once a week.

>[!NOTE]
>
>* You cannot schedule a refresh for the current day. For example, if today is June 1, the earliest day when you can schedule a refresh is June 2.
>* The scheduled refresh occurs sometime during the night, based on the user's cluster (US clusters refresh during night in the US). The specific time is unpredictable due to other customers in the queue and how much data is refreshed. If the queue has many large customers, your refresh may not run until later that day, or the next day.
>* Your Custom Refresh Sandbox always has the same product features as your production environment. However, when you refresh your Custom Refresh Sandbox, it preserves branding only for the login screen background color. The login screen and navigation bar logos are reset to [!DNL Workfront] defaults, and any branding images you modified prior to the refresh do not display.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Access the Custom Refresh Sandbox from your Production environment {#access-the-custom-refresh-sandbox-from-your-production-environment}

As a [!DNL Workfront] administrator, you can access your Custom Refresh Sandbox from your production environment.

>[!NOTE]
>
>If your account is on Cluster 4 (EMEA Cluster), you cannot access your Custom Refresh Sandbox from the Production Environment. For more information about how you can access your Custom Refresh Sandbox when you have an account on Cluster 4, see [Access the Custom Refresh Sandbox for Accounts on Cluster 4 (EMEA Accounts)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Access the Custom Refresh Sandbox for Accounts on Cluster 4 (EMEA Accounts)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

To access your Custom Refresh Sandbox:

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Click **[!UICONTROL System]** >**[!UICONTROL Preferences]**.

1. In the **[!UICONTROL Test Environment]** section, click **[!UICONTROL Sandbox 1]** or **[!UICONTROL Sandbox 2]**.

   Your support package specifies whether you have access to one or two Custom Refresh Sandboxes.

1. Log in using your Custom Refresh Sandbox credentials.

   Your Custom Refresh Sandbox credentials are the same as your production credentials, unless you have changed your production credentials since you last refreshed your Custom Refresh Sandbox. The logins are synchronized only when a refresh occurs. They do not synchronize automatically.

   The Custom Refresh Sandbox shows the version as well as the last refresh date in the banner at the top of the screen. All information from production is available and ready to work with after a refresh completes.

## Access the Custom Refresh Sandbox using a URL {#access-the-custom-refresh-sandbox-using-a-url}

Any user can access the Custom Refresh Sandbox by using a URL.

* [Access the Custom Refresh Sandbox for accounts on Clusters 1,2,3, and 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Access the Custom Refresh Sandbox for Accounts on Cluster 4 (EMEA Accounts)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Access the Custom Refresh Sandbox for accounts on Clusters 1,2,3, and 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Depending on your Support package, you should have access to one or two Custom Refresh Sandboxes.

To access your Custom Refresh Sandbox using a URL:

1. Navigate to this URL if you only have one Custom Refresh Sandbox:

   https://companyname.sb01.workfront.com (old URL:https://cr1.attasksandbox.com/.)

   Or If you have two Custom Refresh Sandboxes, in addition to the URLs above, you can also go to the following URL to access your second Custom Refresh Sandbox:

   https://companyname.sb02.workfront.com (old URL:https://cr2.attasksandbox.com/)

1. On the login screen, log in using your Custom Refresh Sandbox credentials.
1. Your Custom Refresh Sandbox credentials are the same as your production credentials, unless you have changed your production credentials since your Custom Refresh Sandbox was last refreshed. The logins are synchronized only when a refresh occurs. They do not synchronize automatically.

### Access the Custom Refresh Sandbox for Accounts on Cluster 4 (EMEA Accounts) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

If your [!DNL Workfront] account is on Cluster 4 (EMEA cluster), you can access your Custom Refresh Sandbox only using a URL. To find out what cluster your account is on, contact our Customer Support team.

Depending on your Support package, you should have access to one or two Custom Refresh Sandboxes.

To access your Custom Refresh Sandbox using a URL:

1. Navigate to this URL if you only have one Custom Refresh Sandbox:

   https://companyname.sb01.workfront.com (old URL:https://cr3.attasksandbox.com)

   Or

   Go to either one of these URLs if you have two Custom Refresh Sandboxes:

   https://companyname.sb01.workfront.com (old URL:https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (old URL:https://cr4.attasksandbox.com)

1. On the login screen, log in using your Custom Refresh Sandbox credentials.

   Your Custom Refresh Sandbox credentials are the same as your production credentials, unless you have changed your production credentials since your Custom Refresh Sandbox was last refreshed. The logins are synchronized only when a refresh occurs. They do not synchronize automatically.

## Schedule a refresh of your Custom Refresh Sandbox

>[!IMPORTANT]
>
>The duration of the refresh depends on the size of the data being refreshed. During the refresh process, it is critical that your custom refresh sandbox environment is not being used in any way (including API calls and integrations) as this will prevent the sandbox refresh from successfully finishing. [!DNL Workfront] will disable the custom refresh sandbox environment before it begins but you must end any active sessions to ensure that your sandbox refresh is successful.

After you schedule a refresh of your Custom Refresh Sandbox, you can cancel it by clicking [!UICONTROL Cancel] at the top of the page. You can also reschedule it for a later time.

>[!NOTE]
>
>You cannot schedule automatic sandbox refreshes.

To schedule a refresh of your Customer Refresh Sandbox:

1. Log in to your Custom Refresh Sandbox.
1. Click **[!UICONTROL Schedule]** in the banner at the top of the screen and select a date from the calendar.
1. Select a date for when you want the refresh to happen, then click **[!UICONTROL Schedule Refresh]**.

## Switch to Production from the Custom Refresh Sandbox

1. Log in to your Custom Refresh Sandbox.

   For more information about accessing your Custom Refresh Sandbox, see [Access the Custom Refresh Sandbox from your Production environment](#access-the-custom-refresh-sandbox-from-your-production-environment) or [Access the Custom Refresh Sandbox using a URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Click **[!UICONTROL Go To Production]** in the banner at the top of the screen.

   Remember that work done in the sandbox will not be visible in the [!UICONTROL production] environment, as the transfer of data is unidirectional, from production to your Custom Refresh Sandbox, and not in reverse.

## Receive emails from the Custom Refresh Sandbox

[!DNL Workfront] disables all email communication from the Custom Refresh Sandbox environment. If you want to receive email notifications from the Custom Refresh Sandbox environment, you must enable this functionality in your user settings. For more information about enabling email notifications in the Custom Refresh Sandbox environment, see [Enable delivery of emails from the Preview Sandbox environment](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Report delivery and push notifications on the mobile app are always disabled for the Custom Refresh Sandbox environment. Neither you nor the [!DNL Workfront] administrator can enable report delivery or push notifications for the mobile app when you access the Custom Refresh Sandbox environment.\
>For more information about report deliveries for the production environment, see [Report delivery overview](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).For more information about push notifications on the mobile app for the production environment, see the section in .

## Configure Single Sign-On in the Custom Refresh Sandbox

If you want to configure your Custom Refresh Sandbox to work with a Single Sign-On solution, you can do so by configuring it separately from your Production environment. The SSO configuration in the Custom Refresh Sandbox is independent from your SSO configuration in the Production environment.\
When you refresh your Custom Refresh Sandbox, the SSO information is not copied from your Production environment to overwrite the Custom Refresh Sandbox configuration.

The steps for configuring single sign-on in the Custom Refresh Sandbox are similar to those for configuring it in the Production environment.\
For more information about configuring [!DNL Workfront] with SSO, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>This is not available if your organization's [!DNL Workfront] instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

## Intended use and availability

* [!DNL Workfront] Custom Refresh Sandbox environments are not intended for performance or load testing. Rather, use these environments to validate feature functionality with your organization's existing workflows.

* [!DNL Workfront] Custom Refresh Sandbox environments are intended to be always available. Any outage to a Workfront Custom Refresh Sandbox environment during regular business hours will be a first priority immediately after any Production issues are resolved if any exist. Any outage to a Workfront Custom Refresh Sandbox environment on weekends (Saturdays and Sundays) will be addressed so that the environment is running for business hours on Monday.

* Proofing is not available in the Custom Refresh Sandbox environments.
