---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Generate Proofs in [!DNL Workfront Proof]
description: Workfront Proof enables you to create proofs from documents or websites, and share those proofs with others.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
---
# Generate Proofs in [!DNL Workfront Proof]

 <!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] enables you to create proofs from documents or websites, and share those proofs with others. The following steps describe the various configuration options that are available:

## Generate a proof from a document

1. Do one of the following to open the **[!UICONTROL New Proof]** page:

   * Click the **[!UICONTROL New proof]** button in the upper-left corner of any page.
   * Submit via Dropzone (Enterprise feature).

1. To proof one or more documents, add documents to be proofed in either of the following ways (repeat this process to add multiple documents):

   * Drag a document from your file system into the drag-and-drop area in the **[!UICONTROL Add Files]** area.
   * In the **[!UICONTROL Add Files]** area, click the **browse** link to find and select the document you want to upload from the file system on your workstation.

      ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. To proof a website, enter the website's URL in the **[!UICONTROL Add Files]** area, then press **[!UICONTROL Enter]**. Repeat this step to add multiple websites to proof.

   For more details about proofing websites, see [Generate a proof for a URL](#generate-a-proof-for-a-url).

   ![Proof website](assets/proof-website-350x65.png)

1. (Optional) Modify the file names of any uploaded files:

   1. In the document list, hover over the document name you want to modify, then click the **[!UICONTROL Edit]** icon.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. In the **[!UICONTROL Proof name]** field, specify a new name, then click **[!UICONTROL Done]**.

   1. (Optional) To delete any files from being uploaded, hover over the document you want to delete in the document list, then click the **[!UICONTROL Delete]** icon.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Optional) Enable the **[!UICONTROL Combine all compatible files into single proof]** option.

      **When this option is enabled:** All static files and websites are available in a single proof, and you can upload up to 50 files at a given time.

      >[!NOTE]
      >
      >Interactive files, including videos and interactive websites, cannot be combined into a single proof.

      **When this option is disabled:** All documents and websites are generated as individual proofs, and you can upload up to 20 files at a given time.

      To combine all uploaded files and websites into a single proof:

      1. Enable the **[!UICONTROL Combine all compatible files into single proof]** option.
      1. In the **[!UICONTROL Proof name]** field, enter a new name for the combined proof.
      1. In the **[!UICONTROL Add Files]** area, reorder the included files by dragging a file to the desired order. The order of the files is the page order of the combined proof. For more information about creating combined proofs, see [Create a multi-page proof](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Optional) If you want to use an automated workflow that includes multiple stages, select from the following options in the **[!UICONTROL Workflow]** section:

   * **Basic:** Select this option to designate users who you want to have access to the proof immediately after it is created. You can share the proof with multiple users.

      For more information about sharing a proof, see [Share a proof within [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automated:** Select this option to manage content review and approval when you have complex review processes, or if you send content for review to the same groups of people regularly. With an automated workflow, the proof moves from stage to stage until final approval. The relevant users are notified any time that they are required to make an approval.

      For more information about creating an Automated Workflow, see [Set up a proof with an Automated Workflow in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Select whether to send email notifications and a custom message to the users you selected in the previous step:

   * **Notify recipients about this proof:** Select this option to send an email notification to users. When **[!UICONTROL Basic sharing]** is selected in the **[!UICONTROL Workflow]** section, an email notification sends when the proof is created. When **[!UICONTROL Automated workflow]** is selected in the **[!UICONTROL Workflow]** section, an email notification sends when the proof enters the stage of the automated workflow that the user is associated with.

   * **Add custom message:** Select this option to include a custom message in the notification. You can specify a subject and message body. The message body can include rich text formatting, such as bold, bullets, and hyperlinks.

1. Select any of the following proof settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Require login. This proof cannot be shared with other users</td> 
      <td> <p>When this option is selected:</p> 
       <ul> 
        <li>Users cannot sign in to the proof to view it unless they have been added to it.</li> 
        <li>Subscriptions cannot be enabled.</li> 
       </ul> 
       <p>This option is disabled by default.</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Require decisions to be electronically signed</td> 
      <td><p>When this option is selected, users are required to specify their username and password at the time that they make a decision on a proof.</p>
      <p>This option is disabled by default.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lock proof when all required decisions are made</td> 
      <td> <p>When this setting is enabled, the proof state is locked after all decisions have been made. The state is automatically changed from unlocked to locked when the final approver makes their decision.</p> 
      <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow downloading the original file</td> 
      <td> <p><strong></strong> When this option is selected, reviewers are able to download the original file from which the proof was created.</p> <p>When this option is deselected, the Download icon is no longer visible.</p>
      <p>This option is enabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow sharing proof via public URL or embed code</td> 
      <td><p>When this option is selected, the proof can be shared via a public URL or embed code.</p>
       <p>This option is enabled by default.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow subscribing to proof via a public URL or embed code</td> 
      <td> <p>When this option is selected, people who have not been added to the proof can subscribe to the proof. The person subscribing to the proof is granted the role and email that you define in the following settings:</p> 
       <ul> 
        <li><strong>Subscriber role</strong>: The default proof role that is assigned to all reviewers that subscribe to the proof.</li> 
        <li><strong>Email alert settings for subscribers</strong>: The default email alert that is assigned to all reviewers that subscribe to the proof.</li> 
        <li> <p><strong>Proof access via email link required for</strong>: Configure whether the subscriber receives an email with a link to the proof. You can select <strong>No email</strong> (email link is not required to access the proof), <strong>Proof notification email only</strong> (the subscriber receives a link to the proof via email without any verification), or <strong>Validation and proof notification emails</strong> (Subscriber receives a link to the proof via email and must click the link to access a proof. The purpose of this option is to ensure that the person has entered a correct email address to which they have access).</p> <p>Note: If the proofs have an Automated Workflow attached, all subscriptions will generate confirmation emails to the proof Owner so they can decide which stage the person should be added to.</p> </li> 
       </ul> 
        <p>This option is disabled by default.</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create Proof]**. Workfront generates a proof of the selected documents or websites. 
   
   The lag time on a document upload varies depending on the file size and type. Larger files will take longer to generate. You can navigate away from the page as Workfront continues to generate your file. The maximum file upload size is 4GB.
   
## Generate a static proof with a URL {#generate-a-proof-for-a-url}

You can generate a static proof using a website URL.

>[!NOTE]
>
>You can generate an interactive proof for a URL only if your [!DNL Workfront] environment is integrated with a [!DNL Workfront Proof] Premium account. If you can't use proofing as discussed in this section, contact your Workfront administrator.

1. Do one of the following to open the **[!UICONTROL New Proof]** page:

   * Click the **[!UICONTROL New proof]** button in the upper-left corner of any page.
   * Submit via Dropzone (Enterprise feature).

1. In the **New proof** page, enter the URL of the website you want to create a proof from in the **[!UICONTROL Add Files]** area, then press **[!UICONTROL Enter]** or **[!UICONTROL Return]** on your keyboard.

1. (Optional) Repeat this process to add multiple websites to the proof.

   ![proof_website.png](assets/proof-website-350x65.png)

1. In the **[!UICONTROL Add Files]** area, click the **Edit** icon to the right of the URL to open the website proof details.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Enter a **[!UICONTROL Proof name]**. By default, the proof name is the same as the site URL.

1. Select any of the following **[!UICONTROL Handle site contents]** options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Capture screenshot</td> 
      <td>Creates a proof of a static image of the URL's front page.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interactive</td> 
      <td> <p>Creates a proof that allows reviewers to navigate the site, view HTML5 images, Flash elements, and so forth.</p> <p>To create an interactive proof, the website must be hosted with a secure protocol (https). Additionally, websites that can't be embedded in an iframe can't be generated as an interactive proof (iframe embedding restrictions are controlled by the website you are attempting to embed).</p> <p>After the initial proof is created, this setting cannot be changed when creating subsequent versions.</p> <p>For more information about interactive proofing, see <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Generate a proof for interactive content</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Screenshot resolution</td> 
      <td> <p>(This option is not available for interactive proofs.) You can adjust the resolution that your content is displayed in, or you can select multiple resolutions.</p> <p>This enables users reviewing the proof to view how content will appear on different devices, such as various sizes of phones, tablets, and monitors.</p> <p>If you select multiple resolutions, a separate proof is created for each resolution you select.</p> <p>When users comment on the proof, the current screen resolution is automatically displayed in the comment to ensure other users are aware what resolution the comment is associated with.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Look for subpages</td> 
      <td>(This option is not available for interactive proofs.) Select this option to navigate through pages of the website. You can expand the website up to 2 levels deep from the main page. Hover over a page to view the URL of the page and select only those pages that you want to proof. Each page you select is created as an individual proof by default. Alternatively, you can enable the <strong>Combine all compatible files into single proof</strong> option.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Configure any advanced proofing options, such as sharing the proof, adding an Automated Workflow, or setting up access and subscription settings. For more details about these options, see the following articles:

   * [Share a proof within [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Set up a proof with an Automated Workflow in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Configure access and subscription settings for a proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Click **[!UICONTROL Done]**.

1. Click **[!UICONTROL Create Proof]**.

## Generate a proof for interactive content {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

For more information about Interactive content, see [Interactive content proofs overview](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Add interactive content as a URL](#add-interactive-content-as-a-url)
* [Add interactive content as a ZIP file](#add-interactive-content-as-a-zip-file)

### Add interactive content as a URL {#add-interactive-content-as-a-url}

For information about how to add an interactive URL proof, see [Generate a proof for a URL](#generate-a-proof-for-a-url).

### Add interactive content as a ZIP file {#add-interactive-content-as-a-zip-file}

1. Prepare your content by creating a .zip bundled file.

   For information about .zip bundled file specifications, see [Interactive content proofs overview](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Do one of the following to open the **[!UICONTROL New Proof]** page:

   * Click the **[!UICONTROL New proof]** button in the upper-left corner of any page.
   * Submit via Dropzone (Enterprise feature).

1. In the **[!UICONTROL New proof]** page, drag and drop your interactive .zip bundle into the **[!UICONTROL Add files]** area.

1. (Optional) Configure any advanced proofing options, such as sharing the proof, adding an automated workflow, or setting up access and subscription settings. For more details about these options, see the following articles:

   * [Share a proof within [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configure access and subscription settings for a proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Click **[!UICONTROL Create Proof]**. Workfront generates a proof of the zip file.
   
   The lag time on a document upload varies depending on the zip file size. You can navigate away from the page as Workfront continues to generate your file. The maximum file upload size is 4GB.
