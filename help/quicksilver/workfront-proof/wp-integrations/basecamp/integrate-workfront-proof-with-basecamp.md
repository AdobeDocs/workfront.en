---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrate [!DNL Workfront] Proof with [!DNL Basecamp]
description: If you use [!DNL Basecamp] for project management you can offer your project team richer review and approval tools using [!DNL Workfront] Proof.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
---
# Integrate [!DNL Workfront] Proof with [!DNL Basecamp]

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront] Proof. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

If you use [!DNL Basecamp] for project management you can offer your project team richer review and approval tools using [!DNL Workfront] Proof.

## Understanding the Basecamp Integration with [!DNL Workfront]

Integrating with Basecamp allows users to view, review, and approve proofs all within Basecamp. Users can submit proofs to your [!DNL Workfront] Proof account and connect them with your Basecamp project. Your reviewers can&nbsp;comment and make decisions via Basecamp, using the mini proof embedded in your Basecamp message.

When integrated with [!DNL Workfront Proof], [!DNL Basecamp] has the following proofing functionality:

* Users can review and approve proofs within Basecamp Classic.
* Users have review tools readily available.
* Project review teams receive a message in [!DNL Basecamp] with a mini proof for review and approval.
* Users can switch to a full-page proof for review and approval.
* Users can add comments and markups to both mini- and full-sized proofs.

   >[!NOTE]
   >
   >Once a comment has been replied to, it cannot be edited or deleted.

* Reviewers can respond to the and markups made by other reviewers.
* Users are alerted when a new version of proof is available.
* Users who are not [!DNL Workfront] Proof users can work on a proof in Basecamp.

The integration of [!DNL Workfront] Proof with [!DNL Basecamp] must be set up on two levels:

* Configure [!DNL Basecamp] in [Account settings:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)&nbsp;This enables the Basecamp integration for your whole organization. For more information, see [Enabling the Basecamp Integration with [!DNL Workfront] Proof](#enabling-the-basecamp-integration-with-workfront-proof).

* Configure [!DNL Basecamp] in [Personal settings](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): This enables proof creators and owners to connect to their personal Basecamp account and to authorize [!DNL Workfront] Proof access. For more information, see [Configuring Personal Settings](#configuring-personal-settings).

You can integrate [!DNL Workfront] with either Basecamp or Basecamp Classic. Each version of Basecamp uses a different API and, therefore, requires different configuration procedures.

For information on configuring Basecamp Classic, see [Integrating [!DNL Workfront] Proof with Basecamp Classic.](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Enabling the [!DNL Basecamp] Integration with [!DNL Workfront] Proof {#enabling-the-basecamp-integration-with-workfront-proof}

As a [Proof Permissions Profiles in [!DNL Workfront] Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) or [Proof Permissions Profiles in [!DNL Workfront] Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), you can set up the [!DNL Basecamp] integration for the whole account in your [Account settings](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. In [!UICONTROL Basecamp], collect the following information:

   * The URL for your Basecamp account
   * The URL found in the "My info" section

1. Log out of Basecamp.
1. Click **[!UICONTROL Account settings]** near the upper-right corner.
1. Click the **[!UICONTROL Integrations]** tab.
1. In the **[!UICONTROL Basecamp]** section, to the right of **[!UICONTROL Basecamp integration]**, click **[!UICONTROL Enable]**.

1. Next to **[!UICONTROL Basecamp version]**, verify the **[!UICONTROL Classic version]** is the version you are integrating with.

1. (Conditional) If no Basecamp URL displays, click **[!UICONTROL Edit]**, type the URL for your Basecamp account, without including "http://," and then click **[!UICONTROL Save]**.

1. In the upper-right corner of the window, click **[!UICONTROL Settings]** > **[!UICONTROL Personal settings]**.

1. Click the **[!UICONTROL Integrations]** tab.
1. Under **[!UICONTROL Basecamp]**, to the right of **[!UICONTROL Basecamp integration]**, click **[!UICONTROL Enable]**.

1. In the options appear, to the right of **[!UICONTROL Basecamp API Token]**, click **[!UICONTROL Edit]**.

1. In the box that appears, type the URL found in the "My info" section in Basecamp, then click **[!UICONTROL Save]**.\
   Once you integrate [!DNL Workfront] Proof with [!DNL Basecamp], your users can configure their personal settings. For information on setting up personal settings, see [Configuring Personal Settings](#configuring-personal-settings)

1. &nbsp;If you cannot enable Basecamp integration, your [!DNL Workfront] Proof account ID might not be the same as the account ID you use in Basecamp.
1. Once you integrate [!DNL Workfront] Proof with Basecamp, your users can configure their personal settings. For information on setting up personal settings, see [Configuring Personal Settings](#configuring-personal-settings).

## Configuring Personal Settings {#configuring-personal-settings}

After you set up [Account settings](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) for your Organization, each one of your authors that creates/submits proofs should set their&nbsp; [personal settings.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Go to **[!UICONTROL Personal**&#x200B;**settings]**.

1. Open the **[!UICONTROL Integrations]** tab&nbsp;(1).
1. To enable the Basecamp integration, click **[!UICONTROL Enable]** (2).
1. Click **[!UICONTROL Connect to your Basecamp account]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Log in to your Basecamp account (1).\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Click **[!UICONTROL Yes, I'll allow access]** to authorize [!DNL Workfront] Proof access to your account (2).\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Optional) When your personal integration is active (3), you can switch easily between your Basecamp accounts.

   1. Clicking **[!UICONTROL Switch Basecamp account]** (4).\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      The [!UICONTROL Switch Basecamp] Account takes you to the [!UICONTROL Personal Settings] page, where you can choose which of your Basecamp accounts you want to integrate with your [!DNL Workfront] Proof account.

   1. Click **[!UICONTROL Re-Integrate with Basecamp]** (5) before choosing the Basecamp account\

      This refreshes the Personal Settings page and shows your most up-to-date list of Basecamp accounts.

   1. Click **[!UICONTROL Integrate with this account]** to connect it with [!DNL Workfront] Proof.\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      You can now add proofs to [!DNL Basecamp] projects.
