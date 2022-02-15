---
filename: generate-proofs
product: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
---




# Generate Proofs in `Workfront` Proof {#generate-proofs-in-workfront-proof}

`Workfront Proof` enables you to create `proofs` from documents or websites, and share those `proofs` with others. The following steps describe the various configuration options that are available:


## Generate a `proof` for a document {#generate-a-proof-for-a-document}




1. Do any of the following to begin creating a new `proof` and display the New Proof page:
    
    
    * Click the green **New `proof`** button in the upper-left corner of any&nbsp;page.
    * In the **Dashboard** area, in the **Overview** tab, click the **New `proof`** link.
    
    * Submit via Dropzone (Enterprise feature).
    * The **New Proof** page displays.  
    
    
    

1. To `proof` one or more documents, add documents to be proofed in either of the following ways (repeat this process to add multiple documents to be proofed): 
    
    
    * Drag a document from you file system into the drag-and-drop area in the **Add Files** area.
    * Click in the drag-and-drop area in the&nbsp;**Add Files**&nbsp;area, then browse to find and select the document you want to upload from the file system on your workstation.
    
    
      ![proof_document_upload.png](assets/proof-document-upload.png)  

    
    
    

1. To `proof` one or more websites, specify the URL of the website you want to `proof` in the&nbsp;**Add Files**&nbsp;area, then press **Enter**.  

1.  (Optional) Repeat this process to add multiple websites to `proof`.


   For more details about `proofing` websites, see&nbsp; [Generate a proof for a URL](#generating-a-proof-for-a-url).


   ![](assets/proof-website.png)



1. (Optional) Modify the file names of any uploaded files: 
    
    
    1. Mouse over the document name you want to modify in the document list in the **Add Files** area, then click&nbsp;the **Edit** icon.&nbsp;
    
    
       ![proof_edit.png](assets/proof-edit-600x91.png)  

    
    1. In the **Proof name** field, specify a new name, then click **Done**.
    
    1. (Optional) To delete any files from being uploaded, mouse over the document you want to delete in the document list in the&nbsp;**Add Files**&nbsp;area, then&nbsp;click&nbsp;the **Delete**&nbsp;icon.&nbsp;
    
    
       ![proof_delete.png](assets/proof-delete-600x91.png)  

    
    1. (Optional) Enable the option, **Combine all compatible files into single `proof`**.
    
    
       **When this option is enabled:** All static files and websites are available in a single `proof`, and you can upload up to 50 files at a given time.
    
    
       >[!NOTE]
       >
       >Interactive files, including videos and interactive websites, cannot be combined into a single `proof`.
    
    
       **When this option is disabled:** All documents and websites are generated as individual `proofs`, and you can upload up to 20 files at a given time.
    
    
       To combine all uploaded files and websites into a single `proof`:
    
        
        
        1. Enable the option, **Combine all compatible files into single `proof`**.
        1. In the **Proof name** field, specify a new name for the combined `proof`.
        
        1. In the **Add Files** area, reorder the included files by dragging a file to the desired order. The order of the files is the page order of the combined  `proof`. For more information about creating combined `proofs`, see [Create a multi-page proof](create-multi-page-proof.md).
        
        
        
    
    
    
1. (Optional) If you want to use an automated workflow that includes multiple stages, in the **Workflow** section, select from the following options:
    
    
    * **Basic:** Select this option to designate users who you want to have access to the `proof` immediately after it is created. You can share the `proof` with multiple users.
    
    
      For more information about sharing a `proof`, see "Adding Users to a Proof" in&nbsp; [Share a proof within Workfront](share-a-proof-in-workfront.md).
    
    * **Automated:** Select this option to manage content review and approval when you have complex review processes, or if you send content for review to the same groups of people regularly. With automated workflow, the `proof`&nbsp;moves from stage to stage&nbsp;until final approval. The relevant users are notified any time they are required to make an approval.
    
    
      For more information about creating an Automated Workflow, see [Set up a proof with an Automated Workflow in Workfront Proof](set-up-proof-auto-workflow.md#create2).
    
    
    

1. Select whether to send email notifications and a custom message to&nbsp;the users you selected in the previous step:
    
    
    * **Notify recipients about this `proof`:** Select this option to send an email notification to users. When **Basic sharing** is selected in the **Workflow** section, an email notification sends when the `proof` is created. When **Automated workflow** is selected in the **Workflow** section, an email notification sends when the `proof` enters the stage of the automated workflow that the user is associated with.
    
    * **Add custom message:** Select this option to include a custom message in the notification. You can specify a subject and message body. The message body can include rich text formatting, such as bold, bullets, and hyperlinks.
    
    
1.  Select any of the following `proof` settings:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Require login - <span class="WFVariablesproof-sing-n">proof</span> can only be shared with other users</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><b>Require login - <span class="WFVariablesproof-sing-n">proof</span> can only be shared with other users:</b>&nbsp;When this option is selected, only <span class="WFVariablesProdNameWFP">Workfront Proof</span>&nbsp;users are able to view the <span class="WFVariablesproof-sing-n">proof</span>.</p> <p>This option is disabled by default; any person with the URL is able to view the <span class="WFVariablesproof-sing-n">proof</span>.</p> <p>When this option is selected:</p> 
    <ul> 
     <li value="1">Users cannot sign in to the <span class="WFVariablesproof-sing-n">proof</span> unless they have been added to the <span class="WFVariablesproof-sing-n">proof</span>.</li> 
     <li value="2">Subscriptions cannot be enabled.</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Only one decision required for this <span class="WFVariablesproof-sing-n">proof</span></td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>When this option is selected, the review is completed after one of the decision makers makes their decision.</p> <p>This option is disabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Require decisions to be electronically signed</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Users are required to specify their user name and password at the time that they make a decision on&nbsp;a <span class="WFVariablesproof-sing-n">proof</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Lock <span class="WFVariablesproof-sing-n">proof</span> when all required decisions are made</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><b>:</b>&nbsp;When this setting is enabled, the <span class="WFVariablesproof-sing-n">proof</span> state is locked after all decisions have been made. The state is automatically changed from unlocked to locked when the final approver makes their decision.</p> <p>This option is disabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Download original file</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><b>:</b>&nbsp;When this option is selected, reviewers are able to download the original file from which the <span class="WFVariablesproof-sing-n">proof</span> was created.</p> <p>When this option is deselected, the Download icon is no longer visible.<br>This option is enabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Share <span class="WFVariablesproof-sing-n">proof</span> via public URL or embed code</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">When this option is selected, the <span class="WFVariablesproof-sing-n">proof</span> can be shared via a public URL or embed code.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">Subscribe to <span class="WFVariablesproof-sing-n">proof</span> via public URL or embed code</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>When this option is selected, people who have not been added explicitly to the <span class="WFVariablesproof-sing-n">proof</span> can subscribe to the <span class="WFVariablesproof-sing-n">proof</span>. The person subscribing to the <span class="WFVariablesproof-sing-n">proof</span> is granted the role and email that you define in the following settings:</p> 
    <ul> 
     <li value="1"><b>Subscriber role</b>: The default <span class="WFVariablesproof-sing-n">proof</span> role that is&nbsp;assigned to all reviewers that subscribe to the <span class="WFVariablesproof-sing-n">proof</span>.</li> 
     <li value="2"><b>Email alert settings for subscribers</b>: The default email alert that is assigned to all reviewers that subscribe to the <span class="WFVariablesproof-sing-n">proof</span>.</li> 
     <li value="3"> <p><b>Proof access via email link required for</b>: Configure whether the subscriber receives an email with a link to the <span class="WFVariablesproof-sing-n">proof</span>. You can select <b>No email</b> (email link is not required to access the <span class="WFVariablesproof-sing-n">proof</span>), <b>Proof notification email only</b> (the subscriber receives a link to the <span class="WFVariablesproof-sing-n">proof</span> via email without any verification), or <b>Validation and <span class="WFVariablesproof-sing-n">proof</span> notification emails</b> (Subscriber receives a link to the <span class="WFVariablesproof-sing-n">proof</span> via email and must click the link to access a <span class="WFVariablesproof-sing-n">proof</span>; the purpose of this option is to ensure that the person has entered a correct email address to which they have access).</p> <p>Note: If the <span class="WFVariablesproof-plur-n">proofs</span> have Automated Workflow attached all subscriptions will generate confirmation emails to the <span class="WFVariablesproof-sing-n">proof</span> Owner, so they could decide which stage the person should be added to.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click **Create Proof**.


   `Workfront` begins generating a `proof` of the selected documents or websites. Depending on the file size and type, the lag time on a document upload varies. Be patient as bigger files take longer to generate. You can navigate away from the page and `Workfront`&nbsp;continues to generate your file.&nbsp;The maximum file upload size is 4GB.


   After the `proof` is generated, click **Go to `proof`** to launch the `proofing` tool.&nbsp;


   ![Screenshot_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-485x186.png)




   The document appears in the `proofing` tool.  



   Users who do not have `proofing` enabled on their account are still able to view the document and make comments to the `proof`.





## Generate a `proof` for a URL {#generate-a-proof-for-a-url}

You can generate a `proof` for a URL for the first time. Or, you can generate a new version of a URL `proof` where a `proof` has previously been generated.


>[!NOTE]
>
>You can generate an interactive `proof` for a URL only if your `Workfront` environment is integrated with a `Workfront Proof` Premium account. If you cannot use `proofing` as discussed in this section, contact your system administrator.


To generate a `proof` for a URL:



1. Do any of the following to begin creating a new `proof` and display the New Proof page: 
    
    
    * Click the green **New `proof`** button in the upper-left corner of any&nbsp;page.
    * In the **Dashboard** area, in the **Overview** tab, click the **New `proof`** link.
    
    * Submit via Dropzone (Enterprise feature).  
    
    

1. (Conditional) In the **New `proof`** page that appears, to create a new version of an existing `proof`: 
    
    
    1. Select the URL `proof`&nbsp;where you want to add a new version.
    1. Click&nbsp;the **New Version** button at the top of the page.
    
    
       ![Screenshot_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56.png)    
    

    
    
    

1. In the New `proof` version page that displays, specify the URL of the website you want to `proof` in the&nbsp;**Add Files**&nbsp;area, then press **Enter**.

1.  (Optional) Repeat this process to add multiple websites to `proof`.


   ![proof_website.png](assets/proof-website.png)



1.  Click the website&nbsp;in the document list in the&nbsp;**Add Files**&nbsp;area.


   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-538x284.png)   


1.  Specify a **Proof name** for the `proof`. 


   By default, the `proof` name is the same as the site URL.

1.  Select **Handle site contents **options:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Capture screenshot</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Creates a <span class="WFVariablesproof-sing-n">proof</span> of a static image of the URL's&nbsp;front page.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Interactive</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Creates a <span class="WFVariablesproof-sing-n">proof</span> that allows reviewers to navigate the site, view HTML5 images, Flash elements, and so forth.</p> <p>In order to create an interactive <span class="WFVariablesproof-sing-n">proof</span>, the website must be hosted with a secure protocol (https). In addition, websites that cannot be embedded in an iframe cannot be generated as an interactive <span class="WFVariablesproof-sing-n">proof</span> (iframe embedding restrictions are controlled by the website you are attempting to embed).</p> <p>After the initial <span class="WFVariablesproof-sing-n">proof</span> is created, this setting cannot be changed when creating subsequent versions.</p> <p>For more information about interactive <span class="WFVariablesproof-gerund">proofing</span>, see&nbsp;<a href="#generati" class="MCXref xref">Generate a proof for interactive content</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Screenshot resolution</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>(This option is not available for interactive <span class="WFVariablesproof-plur-n">proofs</span>.) You can adjust the resolution that your content is displayed in, or you can select multiple resolutions.</p> <p>This enables users reviewing the <span class="WFVariablesproof-sing-n">proof</span>&nbsp;to&nbsp;view how content will appear on different&nbsp;devices, such as various sizes of phones, tablets, and monitors.</p> <p>If you select multiple resolutions, a separate <span class="WFVariablesproof-sing-n">proof</span> is created for each resolution you select.</p> <p>When users comment on the <span class="WFVariablesproof-sing-n">proof</span>, the current screen resolution is automatically displayed in&nbsp;the comment to ensure other users are aware what resolution the comment is associated with.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray">Look for subpages</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">(This option is not available for interactive <span class="WFVariablesproof-plur-n">proofs</span>.) Select this option to navigate through pages of the&nbsp;website. You can expand the website up to 2 levels deep from the main page. Mouse over a page to view the URL of the page. Select only those pages that you want to <span class="WFVariablesproof-sing-n">proof</span>. Each page you select is created as an individual <span class="WFVariablesproof-sing-n">proof</span> by default; or, enable the&nbsp;<b>Combine&nbsp;into single <span class="WFVariablesproof-sing-n">proof</span></b> option to combine all selected pages into a single <span class="WFVariablesproof-sing-n">proof</span>.</td> 
  </tr> 
 </tbody> 
</table>


1.  (Optional) Configure any advanced `proofing` options, such as sharing the `proof`, adding an Automated Workflow, or setting up access and subscription settings. For more details about these options, see the following articles:

    
    
    * [Share a proof within Workfront](share-a-proof-in-workfront.md) 
    * [Set up a proof with an Automated Workflow in Workfront Proof](set-up-proof-auto-workflow.md) 
    * [Configure access and subscription settings for a proof](configure-access-subscription-settings-proof.md) 
    
    

1.  Click **Done**.


   If you are adding a new version to an existing URL `proof`, any options that were configured on the original `proof` or previous version are maintained in this version.If you are adding a new version to an existing URL `proof`, any options that were configured on the original `proof` or previous version are maintained in this version.

1. Click **Create Proof**.




## Generate a `proof` for interactive content {#generate-a-proof-for-interactive-content}

A Pro `Workfront` Plan or higher is required to use this feature. For more information about the various plans available, see [ `Workfront` Plans](https://www.workfront.com/plans).


For more information about Interactive content, see [Interactive content proofs](interactive-content-proofs.md).



* [Add interactive content as a URL](#uploading-rich-media-content-as-a-url) 
* [Add interactive content as a ZIP file](#uploading-rich-media-content-as-a-zip-file) 




### **Add interactive&nbsp;content as a URL**  {#add-interactive-content-as-a-url}

`For information about how to add an interactive URL `proof`, see  [Generate a proof for a URL](#generating-a-proof-for-a-url)`.


### **Add interactive&nbsp;content as a ZIP file**  {#add-interactive-content-as-a-zip-file}




1.  Prepare your content by creating a .zip bundled file.


   For information about .zip bundled file specifications, see [About preparing interactive content in a ZIP file for proofing](interactive-content-proofs.md#howtoprepareaninteractiveziparchive)&nbsp;in the article [Interactive content proofs](interactive-content-proofs.md).

1. Do any of the following to begin creating a new `proof` and display the New Proof page: 
    
    
    * Click the green **New proof** button in the upper-left corner of any&nbsp;page.
    * In the **Dashboard** area, in the **Overview** tab, click the **New `proof`** link.
    
    * Submit via Dropzone (Enterprise feature).  
    
    

1. In the **New `proof`** page that appears, drag and drop your interactive .zip bundle into the&nbsp;**Add files&nbsp;**area.

1.  (Optional) Configure any advanced `proofing` options, such as sharing the `proof`, adding an automated workflow, or setting up access and subscription settings. For more details about these options, see the following articles:

    
    
    * [Share a proof within Workfront](share-a-proof-in-workfront.md) 
    * [Create an Automated Workflow for the proof](configure-proof.md#create2) in the article [Configure a proof](configure-proof.md#configuring-the-automated-workflow)
    
    * [Configure access and subscription settings for a proof](configure-access-subscription-settings-proof.md) 
    
    

1.  Click&nbsp;**Create Proof**.


   `Workfront` begins generating a `proof` of the .zip bundle. Depending on the bundle size, the lag time on a document upload varies. Larger files take longer to generate. You can navigate away from the page and `Workfront`&nbsp;continues to generate your file.&nbsp;The maximum file upload size is 4GB.


   After the `proof` generates, you can click the **Go to proof **button that appears to open the `proof`.  




