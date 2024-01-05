---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configure User Information using [!DNL Workfront Proof]
description: Configure User Information using [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
---
# Configure User Information using [!DNL Workfront Proof]

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

1. Begin creating or editing a user as described in [Create Users using [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Specify the following information:

   * In the **[!UICONTROL Personal Details]** section:

      * **Email Address:** The user's email address.
      * **First Name:** The user's first name.
      * **Last Name:** The user's last name.
      * **Position:** The user's position in the company.
      * **Permission profile:** The user's permissions on the proof account.
      * **Language:** The user's primary language.
      * **Time zone:** Select the user's time zone.
      * **Date format:** Select the user's preferred date format.
      * **Opt in - Product and marketing emails:** Select whether to opt the user in for product and marketing emails.
      * **API only:** Allows the user to log in only via the API.

   * In the **[!UICONTROL User Details]** section, type the user's contact information, such as street address and phone number.
   * In the **[!UICONTROL Default proof settings]** section, configure the settings that affect the way the user creates or works on proofs.

      * **Default proof role:** Select a default proof role for the user. Role options are **[!UICONTROL Read only]**, **[!UICONTROL Reviewer]**, **[!UICONTROL Approver]**, **[!UICONTROL Reviewer & Approver]**, **[!UICONTROL Author]**, or **[!UICONTROL Moderator]**.

         For more information on proof roles, see [Manage Proof Roles in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Lock the proof when all decisions are made:** Automatically locks the proof from further changes after all decisions on the proof are made.
      * **Login required. The proof can only be shared with other users:** Makes the proof available only to users with [!DNL Workfront Proof] login credentials.
      * **Only one decision required:** Requires only one decision on a proof.
      * **Download of original file:** Enables the user to download the original file for a proof. This option is enabled by default.

         For more information on downloading original files, see [Download Files Stored in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

         <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Subscription. People can sign up for the proof via the public URL or embed code:** Allows reviewers external to the organization to sign up for the proof via the public URL or embed code.

         When this option is selected, **Subscriber must click a link in an email to access a proof** is also available. Select this option to require the external reviewer to click a link within the email to access the proof.
         This option is enabled by default if the **Public sharing** option is selected.

      * **Default role for new guest reviewers:** Select a default proof role for guest reviewers. Options are the same as those in **Default proof role**, with the exception of Moderator and Author.

   * In the **[!UICONTROL Default email alert settings]** section:

      * **Default email alert:** Select how frequently the user receives email updates. Select **All Activity, Replies to my comments, Decisions, Final decision, Hourly summary, Daily summary,** or **Disabled**.

         For more information on default email alert options, see [Configure email notification settings in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Default email alert for new guest reviewers:** Select how frequently guest reviewers receive email updates. Options are the same as those for **Default email alert.**

      * **Send an email confirmation when proofs are ready:** Select to automatically send the user a confirmation email when proofs are ready.
      * **Format of emails sent to this user:** Select **[!UICONTROL HTML]** or **[!UICONTROL Plain text]** as the default format for emails sent to the user.

   * In the **[!UICONTROL Custom message settings]** section: Create settings for proof templates.

      For more information on templates, see:

      * **Proof subject template:** Create a template for a proof subject.
      * **Proof message template:** Create a template for a proof message and its format.
