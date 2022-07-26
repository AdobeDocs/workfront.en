---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integrate [!DNL Workfront Proof] with Basecamp Classic
description: If you use [!DNL Basecamp] for project management you can offer your project team richer review and approval tools using [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
---
# Integrate [!DNL Workfront Proof] with [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

If you use [!DNL Basecamp] for project management you can offer your project team richer review and approval tools using [!DNL Workfront Proof].

## Understanding the [!DNL Basecamp] Integration with [!DNL Workfront]

Integrating with [!DNL Basecamp] allows users to view, review, and approve proofs all within [!DNL Basecamp]. Users can submit proofs to your [!DNL Workfront Proof] account and connect them with your [!DNL Basecamp] project. Your reviewers can  and make [Make a decision on a proof in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp], using the mini proof embedded in your Basecamp message.

When integrated with [!DNL Workfront Proof], [!DNL Basecamp] allows users to do the following with proofs:

* Users can review and approve proofs within [!DNL Basecamp Classic].
* Users have review tools readily available.
* Project review teams receive a message in [!DNL Basecamp] with a mini proof for review and approval.
* Users can switch to a full-page proof for review and approval.
* Users can add comments and markups to both mini- and full-sized proofs.

   >[!NOTE]
   >
   >Once a comment has been replied to, it cannot be edited or deleted.

* Reviewers can respond to the and markups made by other reviewers.
* Users are alerted when a new version of proof is available.
* Users who are not [!DNL Workfront Proof] users can work on a proof in [!DNL Basecamp].

The integration of [!DNL Workfront Proof] with [!DNL Basecamp] must be set up on two levels:

* Configure [!DNL Basecamp] in [Account settings:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) This enables the Basecamp integration for your whole organization.
* For more information, see [Enabling the [!DNL Basecamp] Integration with [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Configure [!DNL Basecamp] in [Personal settings](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): This enables proof creators and owners to connect to their personal [!DNL Basecamp] account and to authorize [!DNL Workfront Proof] access. For more information, see [Configuring Personal Settings](#configuring-personal-settings).

You can integrate [!DNL Workfront] with either [!DNL Basecamp] or [!DNL Basecamp Classic]. Each version of [!DNL Basecamp] uses a different API and, therefore, requires different configuration procedures.

For information on configuring [!DNL Basecamp Classic], see [Enabling the [!DNL Basecamp] Integration with [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in this article.

For information on configuring [!DNL Basecamp], see [Integrate [!DNL Workfront Proof] with [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Enabling the [!DNL Basecamp] Integration with [!DNL Workfront Proof]

As a [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) or [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), you can set up Basecamp integration for the whole account in your [Account settings](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Go to [Account settings.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Open the **[!UICONTROL Integrations]** tab (1).
1. To enable the Basecamp integration, click **[!UICONTROL Enable]** (2).
1. Verify that [!DNL Basecamp Classic] is the version you are integrating with (3).
1. (Conditional) If no [!DNL Basecamp] URL displays (4), click **[!UICONTROL Edit]** and enter the URL for your [!DNL Basecamp] account (without the http://).
1. Click **[!UICONTROL Save]** (5).\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Optional) Check your [!DNL Basecamp] URL in your browser after logging into your [!DNL Basecamp Classic] account (6).

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   Once you integrate [!DNL Workfront Proof] with [!DNL Basecamp], your users can configure their personal settings. For information on setting up personal settings, see [Configuring Personal Settings](#configuring-personal-settings).

    If you cannot enable [!DNL Basecamp] integration, your [!DNL Workfront Proof] account ID might not be the same as the account ID you use in [!DNL Basecamp].

## Configuring Personal Settings

After you set up [Account settings](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) for your Organization, each of your authors that creates/submits proofs should set their  [personal settings.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>Completing these steps is easiest if you have your [!DNL Basecamp] session open in one browser window and your [!DNL Workfront Proof] session open in another window.

* [Retrieving Your [!DNL Basecamp] API Token](#retrieving-your-basecamp-api-token)
* [Adding Your [!DNL Basecamp] API token to Your Personal Settings](#adding-your-basecamp-api-token-to-your-personal-settings)

### Retrieving Your [!DNL Basecamp] API Token 

To complete integration at the individual level in [!DNL Workfront Proof], users need their individual authentication token for the [!DNL Basecamp] API.

To retrieve your [!DNL Basecamp] API token:

1. Sign in to your [!DNL Basecamp] account.
1. Click **[!UICONTROL My Info]** (1) in the upper-right corner of the screen.\
   The [!UICONTROL My Info] page displays.\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. In the [!UICONTROL Authentication tokens] section, click **[!UICONTROL Show your tokens]** (2) to display your personal authentication tokens.
1. Select the **[!UICONTROL Token for feed readers]** or the **[!UICONTROL Basecamp API]** (3), then copy the token to your clipboard.

1. Paste your [!DNL Basecamp] API token into the [!UICONTROL Token for feed readers] or the [!UICONTROL Basecamp API] box.\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Adding Your [!DNL Basecamp] API token to Your Personal Settings  

To paste the [!DNL Basecamp] API token into your [!DNL Workfront Proof] [Personal settings](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. Go to the [[!UICONTROL Integrations] - User Setup](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) in your [Personal settings](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1).\
   An administrator must first enable the [!DNL Basecamp Classic] integration in order for you enable your personal settings. For information on setting up the integration, see [Enabling the [!DNL Basecamp] Integration with [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in this article.

1. In the [!DNL Basecamp] API token box (2), paste the token that you just copied from your [!DNL Basecamp] [!UICONTROL My Info] page into the field (3).\
   For information on copying your [!DNL Basecamp] API token, see [Retrieving Your [!DNL Basecamp] API Token](#retrieving-your-basecamp-api-token) in this article.

1. Click **[!UICONTROL Save]** (4).

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Your [!DNL Workfront Proof] [Personal settings](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) are now integrated with your [!DNL Basecamp Classic] account.
