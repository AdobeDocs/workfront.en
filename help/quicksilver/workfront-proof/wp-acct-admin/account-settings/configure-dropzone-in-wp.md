---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configure the dropzone in [!DNL Workfront Proof]
description: As a [!DNL Workfront Proof] administrator, you can set, view, and edit your users' Dropzone settings. For information about Dropzone, see The Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
---
# Configure the dropzone in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

As a [!DNL Workfront Proof] administrator, you can set, view, and edit your users' Dropzone settings. For information about Dropzone, see [The Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Click **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]**, then open the **[!UICONTROL Dropzone]** tab.

1. Make any of the following changes in the **[!UICONTROL Dropzone details]** section:

   * **[!UICONTROL Web Dropzone]**: Enable or disable the Dropzone.
   * **[!UICONTROL Web Dropzone URL]**: The URL that you must enter into your browser to submit proofs via the Dropzone.
   * **[!UICONTROL Email Dropzone]**: Enable or disable the Email Dropzone.

      >[!NOTE]
      >
      >Emailing to dropzones is no longer supported.

   * **[!UICONTROL Dropzone Owner]**: Set or edit the Dropzone owner. This is the person who will be notified of new submissions to the Dropzone. To be set as the Dropzone owner, the user must be a Supervisor, Admin, Billing Admin, or the account Creator. For more information, see [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Default role for creators]**: All submitters are added to the proof with this role as a default.
   * **[!UICONTROL Email notification for all creators]**: Set the email alert preference for proof creators (submitters) here. See [Configure email notification settings in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) for information about the different alert settings available.

   * **[!UICONTROL New version function]**: Enable and disable the New Version function on the Dropzone. This gives or removes the ability for people to submit new versions of proofs via the Dropzone.
   * **[!UICONTROL Delete draft proofs after (days)]**: Specify the number of days after which a draft proof will be deleted. Proofs remain in a draft state if the Dropzone submission is not completed after uploading the file to the Dropzone.
   * **[!UICONTROL Hide reviewer role]**: Hide the reviewer role field when adding people to the Dropzone.
   * **[!UICONTROL Send proof message on activation]**: Configure [!DNL Workfront Proof] to send proof notification emails to the reviewers automatically when a proof is activated.
   * **[!UICONTROL Activate proof on submission]**: Configure [!DNL Workfront Proof] to activate proofs automatically on submission (removing the need to activate them manually).

   * If a proof is moved out of the Dropzone (for example, to another folder in your account), the Dropzone settings will no longer apply to the proof. This is particularly important in respect of email alert settings.

1. Make any changes in the **[!UICONTROL Dropzone fields]** section to specify which fields display in the [!UICONTROL Proof details] section of the Dropzone submission page when proofs are submitted via the Dropzone.
1. In the **[!UICONTROL Permitted domains]** section, specify domains that you want to be allowed to use the Dropzone.

   * You can click **[!UICONTROL Add domain]** to add a domain. When you have finished adding the domain details, click **[!UICONTROL Save]**.

   * You can **[!UICONTROL Edit]** and **[!UICONTROL Delete]** any existing domains you have previously added.

1. Under **[!UICONTROL People to notify]**, specify the people you want to be notified along with the Dropzone owner when new proofs are submitted to the Dropzone [The Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Click **[!UICONTROL Add people]**, enter the recipient's details, then click **[!UICONTROL Save]**.

   * **[!UICONTROL Delete]** people you have previously added.
