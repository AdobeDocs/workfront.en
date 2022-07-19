---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrate Workfront Proof with Basecamp
description: If you use Basecamp for project management you can offer your project team richer review and approval tools using Workfront Proof.
author: Courtney
feature: "Workfront Proof, Digital Content and Documents"
---

# Integrate Workfront Proof with Basecamp

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

If you use Basecamp for project management you can offer your project team richer review and approval tools using Workfront Proof.

## Understanding the Basecamp Integration with Workfront

Integrating with Basecamp allows users to view, review, and approve proofs all within Basecamp. Users can submit proofs to your Workfront Proof account and connect them with your Basecamp project. Your reviewers can&nbsp;comment and make decisions via Basecamp, using the mini proof embedded in your Basecamp message.

When integrated with Workfront Proof, Basecamp has the following proofing functionality:

* Users can review and approve proofs within Basecamp Classic.
* Users have review tools readily available.
* Project review teams receive a message in Basecamp with a mini proof for review and approval.
* Users can switch to a full-page proof for review and approval.
* Users can add comments and markups to both mini- and full-sized proofs.

  >[!NOTE]
  >
  >Once a comment has been replied to, it cannot be edited or deleted.

* Reviewers can respond to the and markups made by other reviewers.
* Users are alerted when a new version of proof is available.
* Users who are not Workfront Proof users can work on a proof in Basecamp.

The integration of Workfront Proof with Basecamp must be set up on two levels:

* Configure Basecamp in [Account settings:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)&nbsp;This enables the Basecamp integration for your whole organization. For more information, see [Enabling the Basecamp Integration with Workfront Proof](#enabling-the-basecamp-integration-with-workfront-proof).

* Configure Basecamp in [Personal settings](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): This enables proof creators and owners to connect to their personal Basecamp account and to authorize Workfront Proof access. For more information, see [Configuring Personal Settings](#configuring-personal-settings).

You can integrate Workfront with either Basecamp or Basecamp Classic. Each version of Basecamp uses a different API and, therefore, requires different configuration procedures.

For information on configuring Basecamp Classic, see [Integrating Workfront Proof with Basecamp Classic.](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Enabling the Basecamp Integration with Workfront Proof {#enabling-the-basecamp-integration-with-workfront-proof}

As a [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) or [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), you can set up the Basecamp integration for the whole account in your [Account settings](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. In Basecamp, collect the following information:

   * The URL for your Basecamp account
   * The URL found in the "My info" section

1. Log out of Basecamp.
1. Click **Account settings** near the upper-right corner.
1. Click the **Integrations** tab.
1. In the **Basecamp** section, to the right of **Basecamp integration**, click **Enable**.

1. Next to **Basecamp version**, verify the **Classic version** is the version you are integrating with.

1. (Conditional) If no Basecamp URL displays, click **Edit**, type the URL for your Basecamp account, without including "http://," and then click **Save**.

1. In the upper-right corner of the window, click **Settings** > **Personal settings**.

1. Click the **Integrations** tab.
1. Under **Basecamp**, to the right of **Basecamp integration**, click **Enable**.

1. In the options appear, to the right of **Basecamp API Token**, click **Edit**.

1. In the box that appears, type the URL found in the "My info" section in Basecamp, then click **Save**.  
   Once you integrate Workfront Proof with Basecamp, your users can configure their personal settings. For information on setting up personal settings, see [Configuring Personal Settings](#configuring-personal-settings)

1. &nbsp;If you cannot enable Basecamp integration, your Workfront Proof account ID might not be the same as the account ID you use in Basecamp.
1. Once you integrate Workfront Proof with Basecamp, your users can configure their personal settings. For information on setting up personal settings, see [Configuring Personal Settings](#configuring-personal-settings).

## Configuring Personal Settings {#configuring-personal-settings}

After you set up [Account settings](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) for your Organization, each one of your authors that creates/submits proofs should set their&nbsp; [personal settings.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Go to **Personal****settings**.

1. Open the **Integrations** tab&nbsp;(1).
1. To enable the Basecamp integration, click **Enable** (2).
1. Click **Connect to your Basecamp account** (3).  
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)  

1. Log in to your Basecamp account (1).  
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Click **Yes, I'll allow access** to authorize Workfront Proof access to your account (2).  
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Optional) When your personal integration is active (3), you can switch easily between your Basecamp accounts.

   1. Clicking **Switch Basecamp account** (4).  
      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)  
      The Switch Basecamp Account takes you to the Personal Settings page, where you can choose which of your Basecamp accounts you want to integrate with your Workfront Proof account.
   
   1. Click **Re-Integrate with Basecamp** (5) before choosing the Basecamp account  
      This refreshes the Personal Settings page and shows your most up-to-date list of Basecamp accounts.
   
   1. Click **Integrate with this account** to connect it with Workfront Proof.  
      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)  
      You can now add proofs to Basecamp projects.

