---
filename: generate-proofs
product: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Generate Proofs in Workfront Proof
description: Workfront Proof enables you to create proofs from documents or websites, and share those proofs with others. The following steps describe the various configuration options that are available:
---

# Generate Proofs in Workfront Proof

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Workfront Proof enables you to create proofs from documents or websites, and share those proofs with others. The following steps describe the various configuration options that are available:

## Generate a proof for a document

<ol> 
 <li value="1">Do any of the following to begin creating a new proof and display the New Proof page: 
  <ul> 
   <li>Click the green <span class="bold">New proof</span> button in the upper-left corner of any&nbsp;page.</li> 
   <li>In the <span class="bold">Dashboard</span> area, in the <span class="bold">Overview</span> tab, click the <span class="bold">New proof</span> link.</li> 
   <li>Submit via Dropzone (Enterprise feature).</li> 
   <p>The <span class="bold">New Proof</span> page displays.<br></p> 
  </ul></li> 
 <li value="2">To proof one or more documents, add documents to be proofed in either of the following ways (repeat this process to add multiple documents to be proofed): 
  <ul> 
   <li>Drag a document from you file system into the drag-and-drop area in the <span class="bold">Add Files</span> area.</li> 
   <li><p>Click in the drag-and-drop area in the&nbsp;<span class="bold">Add Files</span>&nbsp;area, then browse to find and select the document you want to upload from the file system on your workstation.</p><p><img src="assets/proof-document-upload-350x64.png" alt="proof_document_upload.png" style="width: 350;height: 64;"><br></p></li> 
  </ul></li> 
 <li value="3">To proof one or more websites, specify the URL of the website you want to proof in the&nbsp;<span class="bold">Add Files</span>&nbsp;area, then press <span class="bold">Enter</span>.<br></li> 
 <li value="4"> <p>(Optional) Repeat this process to add multiple websites to proof.</p> <p>For more details about proofing websites, see&nbsp;<a href="#generating-a-proof-for-a-url" class="MCXref xref">Generate a proof for a URL</a>.</p> <p> <img src="assets/proof-website-350x65.png" style="width: 350;height: 65;"> </p> </li> 
 <li value="5">(Optional) Modify the file names of any uploaded files: 
  <ol style="list-style-type: lower-alpha;"> 
   <li value="1"><p>Mouse over the document name you want to modify in the document list in the <span class="bold">Add Files</span> area, then click&nbsp;the <span class="bold">Edit</span> icon.&nbsp;</p><p><img src="assets/proof-edit-350x53.png" alt="proof_edit.png" style="width: 350;height: 53;"><br></p></li> 
   <li value="2">In the <span class="bold">Proof name</span> field, specify a new name, then click <span class="bold">Done</span>.</li> 
   <li value="3"><p>(Optional) To delete any files from being uploaded, mouse over the document you want to delete in the document list in the&nbsp;<span class="bold">Add Files</span>&nbsp;area, then&nbsp;click&nbsp;the <span class="bold">Delete</span>&nbsp;icon.&nbsp;</p><p><img src="assets/proof-delete-350x53.png" alt="proof_delete.png" style="width: 350;height: 53;"><br></p></li> 
   <li value="4"><p>(Optional) Enable the option, <span class="bold">Combine all compatible files into single proof</span>.</p><p><span class="bold">When this option is enabled:</span> All static files and websites are available in a single proof, and you can upload up to 50 files at a given time.</p><note type="note">
     Interactive files, including videos and interactive websites, cannot be combined into a single proof.
    </note><p><span class="bold">When this option is disabled:</span> All documents and websites are generated as individual proofs, and you can upload up to 20 files at a given time.</p><p>To combine all uploaded files and websites into a single proof:</p> 
    <ol style="list-style-type: lower-roman;"> 
     <li value="1">Enable the option, <span class="bold">Combine all compatible files into single proof</span>.</li> 
     <li value="2">In the <span class="bold">Proof name</span> field, specify a new name for the combined proof.</li> 
     <li value="3">In the <span class="bold">Add Files</span> area, reorder the included&nbsp;files by dragging a file to the desired order. The order of the files is&nbsp;the page order of the combined&nbsp;proof. For more information about creating combined proofs, see <a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md" class="MCXref xref">Create a multi-page proof</a>.</li> 
    </ol></li> 
  </ol></li> 
 <li value="6">(Optional) If you want to use an automated workflow that includes multiple stages, in the <span class="bold">Workflow</span> section, select from the following options: 
  <ul> 
   <li><p><span class="bold">Basic:</span> Select this option to designate users who you want to have access to the proof immediately after it is created. You can share the proof with multiple users.</p><p>For more information about sharing a proof, see "Adding Users to a Proof" in&nbsp;<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md" class="MCXref xref">Share a proof within Adobe Workfront</a>.</p></li> 
   <li><p><span class="bold">Automated:</span>&nbsp;Select this option to manage content review and approval when you have complex review processes, or if you send content for review to the same groups of people regularly. With automated workflow, the proof&nbsp;moves from stage to stage&nbsp;until final approval. The relevant users are notified any time they are required to make an approval.</p><p>For more information about creating an Automated Workflow, see <a href="../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2" class="MCXref xref">Set up a proof with an Automated Workflow in Workfront Proof</a>.</p></li> 
  </ul></li> 
 <li value="7">Select whether to send email notifications and a custom message to&nbsp;the users you selected in the previous step: 
  <ul> 
   <li><span class="bold">Notify recipients about this proof:</span> Select this option to send an email notification to users. When <span class="bold">Basic sharing</span> is selected in the <span class="bold">Workflow</span> section, an email notification sends when the proof is created. When <span class="bold">Automated workflow</span> is selected in the <span class="bold">Workflow</span> section, an email notification sends when the proof enters the stage of the automated workflow that the user is associated with.</li> 
   <li><span class="bold">Add custom message:</span> Select this option to include a custom message in the notification. You can specify a subject and message body. The message body can include rich text formatting, such as bold, bullets, and hyperlinks.</li> 
  </ul></li> 
 <li value="8"> <p>Select any of the following proof settings:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Require login - proof can only be shared with other users</td> 
     <td> <p><span class="bold">Require login - proof can only be shared with other users:</span>&nbsp;When this option is selected, only Workfront Proof&nbsp;users are able to view the proof.</p> <p>This option is disabled by default; any person with the URL is able to view the proof.</p> <p>When this option is selected:</p> 
      <ul> 
       <li>Users cannot sign in to the proof unless they have been added to the proof.</li> 
       <li>Subscriptions cannot be enabled.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Only one decision required for this proof</td> 
     <td> <p>When this option is selected, the review is completed after one of the decision makers makes their decision.</p> <p>This option is disabled by default.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Require decisions to be electronically signed</td> 
     <td>Users are required to specify their user name and password at the time that they make a decision on&nbsp;a proof.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Lock proof when all required decisions are made</td> 
     <td> <p><span class="bold">:</span>&nbsp;When this setting is enabled, the proof state is locked after all decisions have been made. The state is automatically changed from unlocked to locked when the final approver makes their decision.</p> <p>This option is disabled by default.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Download original file</td> 
     <td> <p><span class="bold">:</span>&nbsp;When this option is selected, reviewers are able to download the original file from which the proof was created.</p> <p>When this option is deselected, the Download icon is no longer visible.<br>This option is enabled by default.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Share proof via public URL or embed code</td> 
     <td>When this option is selected, the proof can be shared via a public URL or embed code.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Subscribe to proof via public URL or embed code</td> 
     <td> <p>When this option is selected, people who have not been added explicitly to the proof can subscribe to the proof. The person subscribing to the proof is granted the role and email that you define in the following settings:</p> 
      <ul> 
       <li><span class="bold">Subscriber role</span>: The default proof role that is&nbsp;assigned to all reviewers that subscribe to the proof.</li> 
       <li><span class="bold">Email alert settings for subscribers</span>: The default email alert that is assigned to all reviewers that subscribe to the proof.</li> 
       <li> <p><span class="bold">Proof access via email link required for</span>: Configure whether the subscriber receives an email with a link to the proof. You can select <span class="bold">No email</span> (email link is not required to access the proof), <span class="bold">Proof notification email only</span> (the subscriber receives a link to the proof via email without any verification), or <span class="bold">Validation and proof notification emails</span> (Subscriber receives a link to the proof via email and must click the link to access a proof; the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</p> <note type="note">
         If the proofs have Automated Workflow attached all subscriptions will generate confirmation emails to the proof Owner, so they could decide which stage the person should be added to.
        </note> </li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="9"> <p>Click <span class="bold">Create Proof</span>.</p> <p>Workfront&nbsp;begins generating a proof of the selected documents or websites.&nbsp;Depending on the file size and type, the lag time on a document upload varies. Be patient as bigger files take longer to generate. You can navigate away from the page and Workfront&nbsp;continues to generate your file.&nbsp;The maximum file upload size is 4GB.</p> <p>After&nbsp;the proof is generated, click <span class="bold">Go to proof</span>&nbsp;to launch the proofing tool.&nbsp;</p> <p> <img src="assets/screenshot-2018-05-16-08-59-34-350x134.png" alt="Screenshot_2018-05-16_08-59-34.png" style="width: 350;height: 134;"> </p> <p>The document&nbsp;appears in the proofing tool.<br></p> <p>Users who do not have proofing enabled on their account&nbsp;are still able to view the document and make comments to the proof.</p> </li> 
</ol>

## Generate a proof for a URL

You can generate a proof for a URL for the first time. Or, you can generate a new version of a URL proof where a proof has previously been generated.

>[!NOTE]
>
>You can generate an interactive proof for a URL&nbsp;only if your Workfront environment is integrated with a Workfront Proof&nbsp;Premium account. If you cannot use proofing as discussed in this section, contact your system administrator.

To generate a proof for a URL:

<ol> 
 <li value="1">Do any of the following to begin creating a new proof and display the New Proof page: 
  <ul> 
   <li>Click the green <span class="bold">New proof</span> button in the upper-left corner of any&nbsp;page.</li> 
   <li>In the <span class="bold">Dashboard</span> area, in the <span class="bold">Overview</span> tab, click the <span class="bold">New proof</span> link.</li> 
   <li>Submit via Dropzone (Enterprise feature).<br></li> 
  </ul></li> 
 <li value="2">(Conditional) In the <span class="bold">New proof</span> page that appears, to create a new version of an existing proof: 
  <ol style="list-style-type: lower-alpha;"> 
   <li value="1">Select the URL proof&nbsp;where you want to add a new version.</li> 
   <li value="2"><p>Click&nbsp;the <span class="bold">New Version</span> button at the top of the page.</p><p><img src="assets/screenshot-2018-05-15-10-59-56-350x80.png" alt="Screenshot_2018-05-15_10-59-56.png" style="width: 350;height: 80;"></p></li> 
  </ol></li> 
 <li value="3">In the New proof version page that displays, specify the URL of the website you want to proof in the&nbsp;<span class="bold">Add Files</span>&nbsp;area, then press <span class="bold">Enter</span>.</li> 
 <li value="4"> <p>(Optional) Repeat this process to add multiple websites to proof.</p> <p> <img src="assets/proof-website-350x65.png" alt="proof_website.png" style="width: 350;height: 65;"> </p> </li> 
 <li value="5"> <p>Click the website&nbsp;in the document list in the&nbsp;<span class="bold">Add Files</span>&nbsp;area.</p> <p> <img src="assets/proof-upload-website-modify-350x185.png" alt="proof_upload_website_modify.png" style="width: 350;height: 185;"> <br> </p> </li> 
 <li value="6"> <p>Specify a <span class="bold">Proof name</span> for the proof. </p> <p> By default, the proof name is the same as the site URL.</p> </li> 
 <li value="7"> <p>Select <span class="bold">Handle site contents </span>options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Capture screenshot</td> 
     <td>Creates a proof of a static image of the URL's&nbsp;front page.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Interactive</td> 
     <td> <p>Creates a proof that allows reviewers to navigate the site, view HTML5 images, Flash elements, and so forth.</p> <p>In order to create an interactive proof, the website must be hosted with a secure protocol (https). In addition, websites that cannot be embedded in an iframe cannot be generated as an interactive proof (iframe embedding restrictions are controlled by the website you are attempting to embed).</p> <p>After the initial proof is created, this setting cannot be changed when creating subsequent versions.</p> <p>For more information about interactive proofing, see&nbsp;<a href="#generati" class="MCXref xref">Generate a proof for interactive content</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Screenshot resolution</td> 
     <td> <p>(This option is not available for interactive proofs.) You can adjust the resolution that your content is displayed in, or you can select multiple resolutions.</p> <p>This enables users reviewing the proof&nbsp;to&nbsp;view how content will appear on different&nbsp;devices, such as various sizes of phones, tablets, and monitors.</p> <p>If you select multiple resolutions, a separate proof is created for each resolution you select.</p> <p>When users comment on the proof, the current screen resolution is automatically displayed in&nbsp;the comment to ensure other users are aware what resolution the comment is associated with.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Look for subpages</td> 
     <td>(This option is not available for interactive proofs.) Select this option to navigate through pages of the&nbsp;website. You can expand the website up to 2 levels deep from the main page. Mouse over a page to view the URL of the page. Select only those pages that you want to proof. Each page you select is created as an individual proof by default; or, enable the&nbsp;<span class="bold">Combine&nbsp;into single proof</span> option to combine all selected pages into a single proof.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="8"> <p>(Optional) Configure any advanced proofing options, such as sharing the proof, adding an Automated Workflow, or setting up access and subscription settings. For more details about these options, see the following articles:</p> 
  <ul> 
   <li><a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md" class="MCXref xref">Share a proof within Adobe Workfront</a> </li> 
   <li><a href="../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md" class="MCXref xref">Set up a proof with an Automated Workflow in Workfront Proof</a> </li> 
   <li><a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md" class="MCXref xref">Configure access and subscription settings for a proof</a> </li> 
  </ul> </li> 
 <li value="9"> <p>Click <span class="bold">Done</span>.</p> <p>If you are adding a new version to an existing URL proof, any options that were configured on the original proof or previous version are maintained in this version.If you are adding a new version to an existing URL proof, any options that were configured on the original proof or previous version are maintained in this version.</p> </li> 
 <li value="10">Click <span class="bold">Create Proof</span>.</li> 
</ol>

## Generate a proof for interactive content

A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).

For more information about Interactive content, see [Interactive content proofs overview](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Add interactive content as a URL](#uploading-rich-media-content-as-a-url) 
* [Add interactive content as a ZIP file](#uploading-rich-media-content-as-a-zip-file)

### `Add interactive content as a URL`

`For information about how to add an interactive URL proof, see  [Generate a proof for a URL](#generating-a-proof-for-a-url)`.

### `Add interactive content as a ZIP file`

1. Prepare your content by creating a .zip bundled file.

   For information about .zip bundled file specifications, see [About preparing interactive content in a ZIP file for proofing](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive)&nbsp;in the article [Interactive content proofs overview](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Do any of the following to begin creating a new proof and display the New Proof page:

  * Click the green `New proof` button in the upper-left corner of any&nbsp;page.
  * In the `Dashboard` area, in the `Overview` tab, click the `New proof` link.
  
  * Submit via Dropzone (Enterprise feature).

1. In the `New proof` page that appears, drag and drop your interactive .zip bundle into the  `Add files`area.

1. (Optional) Configure any advanced proofing options, such as sharing the proof, adding an automated workflow, or setting up access and subscription settings. For more details about these options, see the following articles:

  * [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) 
  * [Create an Automated Workflow for the proof](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-proof.md#create2) in the article [Configure a proof](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-proof.md#configuring-the-automated-workflow)
  
  * [Configure access and subscription settings for a proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Click  `Create Proof`.

   Workfront&nbsp;begins generating a proof of the .zip bundle. Depending on the bundle size, the lag time on a document upload varies. Larger files take longer to generate. You can navigate away from the page and Workfront&nbsp;continues to generate your file.&nbsp;The maximum file upload size is 4GB.

   After the proof generates, you can click the `Go to proof`button that appears to open the proof.

