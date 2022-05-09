---
filename: adobe-sign-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Acrobat Sign modules
description: With the Adobe Acrobat Sign modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe Acrobat Sign account, create, read, or update agreements and other records, search for records using criteria you set, and upload documents.
---

# Adobe Acrobat Sign modules

With the Adobe Acrobat Sign modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe Acrobat Sign account, create, read, or update agreements and other records, search for records using criteria you set, and upload documents.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Adobe Acrobat Sign connector usage recommendations

The Adobe Sign app makes automating eSignature business processes in Fusion much easier and more powerful.

New users to Adobe Sign should pay close attention some of the constraints around updating agreements. Agreements are not typically changed once started. We recommend that new users of Adobe Sign focus on creating new agreements using the agreement creation module. This will make Fusion automations easier and work better with Adobe Sign.

Adobe Sign agreements need a field to work with. There are some options for doing this but the easiest and most common is uploading a transient document and then mapping that document to your agreement.

![](assets/adobe-sign-recommendations-350x168.png)

## Adobe Acrobat Sign modules and their fields

When you configure Adobe Acrobat Sign modules, Workfront Fusion displays the fields listed below. Along with these, additional Adobe Acrobat Sign fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers {#triggers}

* [Watch for agreements](#watch-for-agreements) 
* [Watch for events](#watch-for-events)

#### Watch for agreements {#watch-for-agreements}

This trigger module starts a scenario when an agreement is created or updated.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td>Select whether you want to watch for new records, updated records, or both.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type </td> 
   <td>Select the type of record that you want the record to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Find text</td> 
   <td> <p>Enter terms that you want to search for. The module returns records that include these terms as field values.</p> <p>For more information on searching fields in Adobe Acrobat Sign, see "How text searching works" in <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Adobe Sign Search - How it works</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned agreements</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch for events {#watch-for-events}

This trigger module starts a scenario when an event that you select occurs.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook</td> 
   <td>Select the webhook that you want to use, or click <b>Add</b> and fill in the following fields.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter a name for the webhook</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Scopes</td> 
   <td> 
    <ul> 
     <li> <p>Account</p> </li> 
     <li> <p>Group</p> </li> 
     <li> <p>User</p> </li> 
     <li> <p>Resource</p> <p>If you select Resource, Enter the Resource ID and the Resource type.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Resource level</td> 
   <td> <p>Select the type of resource that you want to watch.</p> 
    <ul> 
     <li> <p>Agreements</p> </li> 
     <li> <p>Widgets</p> </li> 
     <li> <p>Megasigns</p> </li> 
     <li> <p>Library Documents</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Webhook subscription events</td> 
   <td>Select the Adobe Sign events that you want the module to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Application display name</td> 
   <td>The display name of the application through which the webhook is created.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Application name</td> 
   <td>The display name of the application through which the webhook is created.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Problem notification emails</td> 
   <td> <p>This setting works only for admin accounts</p> <p>For each email address that you want to sent problem notification emails to, click <b>Add</b> and enter the email address.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Agreement conditional parameters</td> 
   <td>If you want to add any conditional parameters, select <b>Yes</b> on the record type that you want to add parameters to, then select <b>Yes</b> on any parameters you want to enable.</td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Create a record](#create-a-record) 
* [Create an agreement](#create-an-agreement) 
* [Create related records](#create-related-records) 
* [Custom API Call](#custom-api-call) 
* [List records](#list-records) 
* [Read a record](#read-a-record) 
* [Read related records](#read-related-records) 
* [Update a record](#update-a-record) 
* [Update related record](#update-related-record) 
* [Upload document](#upload-document)

#### Create a record {#create-a-record}

This action module creates a new record of the selected type.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td> <p>Select the type of record you want to create.</p> 
    <ul> 
     <li> <p><b>Group</b> </p> </li> 
     <li> <p><b>Library document</b> </p> </li> 
     <li> <p><b>User</b> </p> </li> 
     <li> <p><b>Web form (Widget)</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Group info</td> 
   <td> <p>Enter or map the group's Name and ID, and indicate whether this group is the default group for the account.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Library document info</td> 
   <td> <p>Fill in the following fields:</p> 
    <ul> 
     <li> <p><b>Files to send</b> </p> <p>For each file you want to add, click <b>Add item</b> and fill in the fields.</p> 
      <ul> 
       <li><b>Transient document ID</b> <p>Enter the ID&nbsp;of the transient document</p> </li> 
       <li> <p><b>URL file transfer</b> </p> <p>Fill in the following fields:</p> 
        <ul> 
         <li> <p><b>Mime-Type</b> </p> <p>Enter the mime type of the original file. Multipurpose Internet Mail Extension (MIME) types are labels that allow software to identify different types of data shared on the internet. Web servers and browsers use the MIME type to determine what should be done with a file. For example, a file with the MIME type <code>text/html</code> will be processed in a browser differently than a file with MIME type <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>Name</b> </p> <p>Enter a name for the file.</p> </li> 
         <li> <p><b>URL</b> </p> <p>Enter the URL of the file that you want to send.</p> </li> 
        </ul> </li> 
       <li> <p><b>Notarize</b> </p> <p>Select whether this document needs to be notarized.</p> </li> 
      </ul> </li> 
     <li> <p><b>Library template name</b> </p> <p>Enter or map the name of the library template</p> </li> 
     <li> <p><b>Sharing mode</b> </p> <p>Specify who should have access to the library document.</p> </li> 
     <li> <p><b>Library document state</b> </p> <p>Select whether the document is in authoring state or active.</p> </li> 
     <li> <p><b>Library template type</b> </p> <p>For each library template type you want to use, click <b>Add item</b> and select the template type.</p> </li> 
     <li> <p><b>Last event date</b> </p> <p>Enter the last date that an event occurred on the library document.</p> <p>For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p> </li> 
     <li> <p><b>Library document status</b> </p> <p>Select the status of the library document.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">User info</td> 
   <td> <p>Fill in the following fields:</p> 
    <ul> 
     <li> <p><b>Email</b> </p> <p>Enter the email address of the user.</p> </li> 
     <li> <p><b>Is account admin</b> </p> <p>Check this option if the created user is an account administator.</p> </li> 
     <li> <p><b>User ID</b> </p> <p>Enter the unique ID of the user</p> </li> 
     <li> <p><b>Account ID</b> </p> <p>Enter the unique ID of the Adobe Acrobat Sign account associated with this user.</p> </li> 
     <li> <p><b>First name</b> </p> <p>Enter the first name of the user.</p> </li> 
     <li> <p><b>Last name</b> </p> <p>Enter the last name of the user</p> </li> 
     <li> <p><b>Company</b> </p> <p>Enter the name of the user's company.</p> </li> 
     <li> <p><b>Initials</b> </p> <p>Enter the initials of the user.</p> </li> 
     <li> <p><b>Locale</b> </p> <p>Enter the locale of the user. This determines the language of the UI. </p> </li> 
     <li> <p><b>Phone</b> </p> <p>Enter the phone number of the user</p> </li> 
     <li> <p><b>Primary group ID</b> </p> <p>Enter the group to which the new user is added. If nothing is entered, the user will be added to the default group for the account.</p> </li> 
     <li> <p><b>Job title</b> </p> <p>Enter the job title of the user.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Web form info</td> 
   <td> <p>Fill in the following fields</p> 
    <ul> 
     <li> <p><b>File info</b> </p> <p>For each file you want to add to the web form, click Add and fill in the following fields:</p> 
      <ul> 
       <li> <p>File type</p> <p>Document</p> </li> 
       <li> <p>Transient document</p> </li> 
       <li> <p>URL file info</p> </li> 
      </ul> </li> 
     <li> <p><b>Web form name</b> </p> <p>Enter a name for the web form. This name is used to identify the web form in places such as emails and websites.</p> </li> 
     <li> <p><b>Web form state</b> </p> <p>Select the state in which the new web form should be created.</p> </li> 
     <li> <p><b>Web form participant set info</b> </p> 
      <ul> 
       <li> <p><b>Member info</b> </p> <p>For each member that you want to add to the participant set, click <b>Add item</b>. </p> 
        <ul> 
         <li> <p><b>Email</b> </p> <p>Leave this option blank.</p> </li> 
         <li> <p><b>Security option</b> </p> <p>If you want to add a security option for authenticating this user, select <b>Yes</b>, then select the security option and fill in any fields it requires.</p> </li> 
        </ul> </li> 
       <li> <p><b>Role</b> </p> <p>Select the role. All members of this participant set share the role.</p> </li> 
      </ul> </li> 
     <li> <p><b>Web form additional participant sets info</b> </p> 
      <ul> 
       <li> <p><b>Member info</b> </p> <p>For each member that you want to add to the participant set, click <b>Add item</b>.</p> 
        <ul> 
         <li> <p><b>Email</b> </p> <p>Leave this option blank.</p> </li> 
         <li> <p><b>Security option</b> </p> <p>If you want to add a security option for authenticating this user, select <b>Yes</b>, then select the security option and fill in any fields it requires.</p> </li> 
        </ul> </li> 
       <li> <p><b>Role</b> </p> </li> 
       <li> <p><b>Web form participant ID&nbsp;</b> </p> <p>Enter the ID of the web form participant.</p> </li> 
       <li> <p><b>Order</b> </p> <p>Specify the order of when this participant set should interact with the web form. For example, the participant group that has the an order value of 1 must go first, 2 must go next, and so on. Order numbers must begin with one, and have no gaps in the series. </p> </li> 
       <li> <p><b>Provider participant set info</b> </p> <p>If the participant is unknown, enter whether the provider must provide details for the participant, and enter a message with the details that you require for the unknown participant.</p> </li> 
      </ul> </li> 
     <li> <p><b>Authentication failure info</b> </p> <p>If you want to provide a failure or error page for your users, select <b>Yes</b>, then fill in the following fields:</p> 
      <ul> 
       <li> <p><b>URL</b> </p> <p>Enter the URL for the error page</p> </li> 
       <li> <p><b>Deframe</b> </p> <p>Enable this option if you want the error page to appear inside the web form</p> </li> 
       <li> <p><b>Delay</b> </p> <p>Enter the delay, in seconds, before the user is redirected to the error page.</p> </li> 
      </ul> </li> 
     <li> <p><b>CC info</b> </p> <p>For each email address that you want to receive an email when the final agreement on the web form is signed, click <b>Add item</b> and enter the email address.</p> </li> 
     <li> <p><b>Completion info</b> </p> <p style="font-style: normal;">If you want to provide a success page for your users, select <b>Yes</b>, then fill in the following fields:</p> 
      <ul> 
       <li> <p><b>URL</b> </p> <p>Enter the URL for the success page</p> </li> 
       <li> <p><b>Deframe</b> </p> <p>Enable this option if you want the success page to appear inside the web form</p> </li> 
       <li> <p><b>Delay</b> </p> <p>Enter the delay, in seconds, before the user is redirected to the success page.</p> </li> 
      </ul> </li> 
     <li> <p><b>Group ID</b> </p> <p>Enter the ID of the group to which the web form belongs. If nothing is entered, the web form belongs to the primary group of the account user.</p> </li> 
     <li> <p><b>Last event date</b> </p> <p>Enter the date that the last event occurred on the web form. Use the format <code>yyyy-MM-dd'T'HH:mm:ssZ</code>.</p> </li> 
     <li> <p><b>Locale</b> </p> <p>Enter the locale of the user. This determines the language of the UI. </p> </li> 
     <li> <p><b>Security option</b> </p> <p>Enter the password used to secure the document. You must separately communicate this password to any relevant parties.</p> </li> 
     <li> <p><b>Vaulting info</b> </p> <p>If your a ccount is set up for document vaulting and the option to enable per agreement, you can enable this option to vault this agreement.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Create an agreement {#create-an-agreement}

This action module creates an agreement, sends it out for signature, and returns the agreement ID.

>[!NOTE]
>
>We recommend uploading the document to sign as a transient document, then mapping it to the File to send field in the Create an agreement module. For an example, see [Upload document](#upload-document) in this article.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Files to send</td> 
   <td> <p>For each item you want to include in the agreement, click <b>Add Item</b> and fill in the following fields:</p> 
    <ul> 
     <li> <p><b>File Type</b> </p> 
      <ul> 
       <li> <p><b>Document</b> </p> <p>Fill in the following fields:</p> 
        <ul> 
         <li> <p><b>Created date</b> </p> <p>Enter or map the date that the document was created in the format <code>yyyy-MM-dd'T'HH:mm:ssZ</code>. For example, <code>2016-02-25T18:46:19Z</code> represents UTC time.</p> </li> 
         <li> <p><b>ID</b> </p> <p>Enter or map the ID&nbsp;of the document.</p> </li> 
         <li> <p><b>Label</b> </p> <p>Enter or map a unique label for the file. In case of custom workflow this will map a file to corresponding file element in workflow definition. This must be specified in case of custom workflow agreement creation request.</p> </li> 
         <li> <p><b>Number of pages</b> </p> <p>Enter or map the number of pages in the document.</p> </li> 
         <li> <p><b>Mime-Type</b> </p> <p>Enter or map the mime type of the original file. Multipurpose Internet Mail Extension (MIME) types are labels that allow software to identify different types of data shared on the internet. Web servers and browsers use the MIME type to determine what should be done with a file. For example, a file with the MIME type <code>text/html</code> will be processed in a browser differently than a file with MIME type <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>Name</b> </p> <p>Enter or map a name for the document.<br></p> </li> 
        </ul> </li> 
       <li> <p><b>Library document ID</b> </p> <p>Enter the ID&nbsp;of the library document</p> </li> 
       <li> <p><b>Transient document ID</b> </p> <p>Enter the ID&nbsp;of the transient document</p> </li> 
       <li> <p><b>URL file transfer</b> </p> <p>Fill in the following fields:</p> 
        <ul> 
         <li> <p><b>Mime-Type</b> </p> <p>Enter the mime type of the original file. Multipurpose Internet Mail Extension (MIME) types are labels that allow software to identify different types of data shared on the internet. Web servers and browsers use the MIME type to determine what should be done with a file. For example, a file with the MIME type <code>text/html</code> will be processed in a browser differently than a file with MIME type <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>Name</b> </p> <p>Enter a name for the file.</p> </li> 
         <li> <p><b>URL</b> </p> <p>Enter the URL of the file that you want to send.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>Label</b> </p> <p>Enter a label for the file.</p> </li> 
     <li> <p><b>Notarize</b> </p> <p>Enable this option to indicate that the file must be notarized.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Agreement name</td> 
   <td>Enter a name for the new agreement. This name is used to identify the agreement in places such as emails and websites.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Participant sets info</td> 
   <td> <p>For each participant set you want to add, click <b>Add item</b> and fill in the following fields.</p> 
    <ul> 
     <li> <p><b>Members</b> </p> <p>For each person that you want to add to the participant set, click <b>Add item</b> and enter the person's email address.</p> </li> 
     <li> <p><b>Order</b> </p> <p>Specify the order of when this participant set should sign the agreement. For example, the participant group that has the an order value of 1 must sign first, 2 must sign next, and so on. Order numbers must begin with one, and have no gaps in the series. </p> </li> 
     <li> <p><b>Role</b> </p> <p>Select a role for this participant set. All participants in the set receive this role.</p> </li> 
     <li> <p><b>ID</b> </p> <p>Enter or map the ID&nbsp;of this participant set.</p> </li> 
     <li> <p><b>Label</b> </p> <p>Enter or map a unique label for the participant set. For custom workflows, label specified in the participation set should map it to the participation step in the custom workflow.</p> </li> 
     <li> <p><b>Name</b> </p> <p>Enter a name for the participant set. This name must be unique within the agreement.</p> </li> 
     <li> <p><b>Private message</b> </p> <p>Enter or map a message for this participant set. All participants in the set receive this message.</p> </li> 
     <li> <p><b>Visible pages</b> </p> <p>If limited document visibility is enabled for this agreement, specify which files are visible to this participant set. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Signature type</td> 
   <td> <p>Select the type of signature that the agreement requires.</p> 
    <ul> 
     <li> <p><b>E-sign</b> </p> <p>The agreement must be electronically signed.</p> </li> 
     <li> <p><b>Written</b> </p> <p>The agreement must be signed by hand, and the signed agreement must be scanned and uploaded.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">State</td> 
   <td> <p>Select a state for this agreement.</p> 
    <ul> 
     <li> <p><b>Authoring</b> </p> <p>You can still edit or add fields to this agreement.</p> </li> 
     <li> <p><b>Draft</b> </p> <p>You can incrementally build this agreement before sending it out.</p> </li> 
     <li> <p><b>In Process</b> </p> <p>This agreement will be sent immediately.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">CCs</td> 
   <td> <p>You can send this agreement to interested parties that do not need to sign, such as stakeholders. They receive an email at the beginning of the signing process and another when the final signature is received. They also receive a PDF copy of the agreement. </p> <p>For each person that you want to CC&nbsp;on this agreement, click <b>Add item</b> and fill in the following fields:</p> 
    <ul> 
     <li> <p><b>Email</b> </p> <p>Enter or map the email address that you want to CC on the agreement.</p> </li> 
     <li> <p><b>Label</b> </p> <p>Enter or map a label for this email address, as seen in the workflow description</p> </li> 
     <li> <p><b>Visible pages</b> </p> </li> 
     <li> <p>If limited document visibility is enabled for this agreement, specify which files are visible to this participant set. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email option</td> 
   <td> <p>For each type of email, select whether that type of email is sent to all participants or none.</p> 
    <ul> 
     <li> <p><b>Completion emails</b> </p> <p>Send an email when this agreement is completed, cancelled, expired, or rejected.</p> </li> 
     <li> <p><b>In-Flight emails</b> </p> <p>Sent an email when this agreement is delegated or replaced.</p> </li> 
     <li> <p><b>Agreement initiation emails</b> </p> <p>Send an email when this agreement is created or when an action on it is requested.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">External ID</td> 
   <td> <p>Enter or map an ID&nbsp;for this agreement. You can specify this when the agreement is created, and use it to locate the agreement in later modules or queries.</p> <p>Note: The External ID value is visible to all participants through the API, so it should not be used to contain a sensitive token.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Merge field info</td> 
   <td> <p>For each field in the agreement that you want to put a default value for, click <b>Add item</b> and enter the default value and the field name.</p> <p>The values will be presented to the signers for editable fields For read-only fields the provided values will not be editable during the signing process.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Notary info</td> 
   <td> <p>Fill in the following fields:</p> 
    <ul> 
     <li> <p><b>Appointment</b> </p> <p>Enter or map a proposed time and date for the appointment to notarize this agreement.</p> </li> 
     <li> <p><b>Note</b> </p> <p>Enter or map any notes that you want to include about the notary session.</p> </li> 
     <li> <p><b>Payment</b> </p> <p>Select whether the notary is paid by the signer or the sender of the agreement.</p> </li> 
     <li> <p><b>Notary Type</b> </p> <p>Select the type of notary</p> 
      <ul> 
       <li> <p>Provider notary</p> <p>The notary is provided by the notary provider.</p> </li> 
       <li> <p>BYON notary</p> <p>The notary is provided by the customer.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Post sign option</td> 
   <td> <p>Select whether you want the signers to be directed to a success page after the agreement is signed. If you select <b>Yes</b>, fill in the following fields:</p> 
    <ul> 
     <li> <p><b>Redirect delay</b> </p> <p>Enter or map a number representing the number of seconds before the signer is redirected to the success page. If this value is greater than 0, the user will first see the standard Adobe Sign success message, and then after a delay will be redirected to your success page.</p> </li> 
     <li> <p><b>Redirect URL</b> </p> <p>Enter or map a publicly accessible URL to which the user will be sent after successfully completing the signing process.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Security option</td> 
   <td> <p>Enter or map the secondary password that will be used to secure the PDF document. </p> <p>Important: Adobe Sign will never share this password, so you must separately communicate it to any relevant parties.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vaulting info</td> 
   <td>If your account is set up for document vaulting and the option to enable per agreement, you can enable this option to vault this agreement.</td> 
  </tr> 
 </tbody> 
</table>

#### Create related records  {#create-related-records}

This action module creates records linked to a module you select.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td>Select the record type of the original record that you want to associate the created records with.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Agreement/Library document/User/Widget ID</td> 
   <td>Enter or map the ID&nbsp;of the object that you want to associate the created record with.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Agreement related field</td> 
   <td> <p>Select the type of related field that you want to create</p> 
    <ul> 
     <li> <p><b>Form fields</b> </p> <p>Enter the Template ID&nbsp;of the template that contains the fields you want to create</p> </li> 
     <li> <p><b>Reminders</b> </p> <p>Fill in the following fields:</p> 
      <ul> 
       <li> <p><b>Recipient participant ID</b> </p> <p>For each participant that you want to receive a reminder, click Add item, and enter the ID&nbsp;of the participant.</p> </li> 
       <li> <p><b>Status</b> </p> <p>For new records, the status must be Active.</p> </li> 
       <li> <p><b>First reminder delay</b> </p> <p>Enter the delay in hours before sending the first reminder. The minimum value allowed is 1 hour and the maximum value can’t be more than the difference of agreement creation and expiry time of the agreement in hours. If this delay is not set, the first reminder will be based on the frequency.</p> </li> 
       <li> <p><b>Reminder frequency</b> </p> <p>Set the frequency at which you want the reminder sent. If frequency is not provided, the reminder will be sent once.</p> </li> 
       <li> <p><b>Last sent date</b> </p> <p>This field is set by the system.</p> </li> 
       <li> <p><b>Next sent date</b> </p> <p>This field must be blank or set to ONCE.</p> </li> 
       <li> <p><b>Note</b> </p> <p>Enter a note to be included with the reminder. This is useful to tell the participant why their participation is required.</p> </li> 
       <li> <p><b>Start reminder counter from</b> </p> <p>Select whether the reminder is sent based on when the agreement is created on when it becomes available.</p> </li> 
      </ul> </li> 
     <li> <p><b>Signer identity report</b> </p> <p>Enter the password used to secure the PDF document.</p> </li> 
     <li> <p><b>Views</b> </p> <p>Enter the following fields</p> 
      <ul> 
       <li> <p><b>Name</b> </p> <p>Select the name of the view you want to create.</p> </li> 
       <li> <p><b>Auto login user</b> </p> <p>Select <b>Yes</b> to automatically login the user to the returned URL.</p> </li> 
       <li> <p><b>Frame Parent</b> </p> <p>Enter or map a comma-separated list of parent domain URLs where the returned URLs may be iframed. If left empty, the Adobe Acrobat Sign pages are not viewable in iframe.</p> </li> 
       <li> <p><b>Locale</b> </p> <p>Enter the language that you want to create the view in. </p> </li> 
       <li> <p><b>No chrome flag</b> </p> <p>Select <b>Yes</b> to show the embedded page without a navigation header or footer.</p> </li> 
       <li> <p><b>Can edit files</b> </p> <p>Select <b>Yes</b> if you want the file upload section to be edited by adding or removing files. This is not an access control machanism. The default is Yes.</p> </li> 
       <li> <p><b>Library document</b> </p> <p>Select <b>Yes</b> if you want library document links to be visible. The default is Yes.</p> </li> 
       <li> <p><b>Local file</b> </p> <p>Select <b>Yes</b> if you want the local file upload button to appear. The default is Yes.</p> </li> 
       <li> <p><b>Web connectors</b> </p> <p>Select <b>Yes</b> if you want the links to attach documents from web sources to appear. The default is Yes.</p> </li> 
       <li> <p><b>Is preview selected</b> </p> <p>Select <b>Yes</b> to set the Compose page to Authoring mode.</p> </li> 
      </ul> </li> 
     <li> <p><b>Member share</b> </p> <p>For each member that you want to share the agreement with, Click <b>Add item</b> and enter the member's email address and a message to that member.</p> </li> 
     <li> <p>Delegate participant set</p> 
      <ul> 
       <li> <p><b>Participant set ID</b> </p> <p>Enter the ID of the participant set</p> </li> 
       <li> <p><b>Member info</b> </p> <p>For each member you want to add, click Add item and enter the email address and phone information for the member.</p> </li> 
       <li> <p><b>Private message</b> </p> <p>Enter a message. All members of the participant set receive this message.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Library view info</td> 
   <td> <p>Fill in the following fields:</p> 
    <ul> 
     <li> <p><b>Name</b> </p> <p>Enter a name for the library template. This name is used in emails and websites.</p> </li> 
     <li> <p><b>Auto login user</b> </p> <p>Select <b>Yes</b> to automatically login the user to the returned URL.</p> </li> 
     <li> <p><b>Frame parent</b> </p> <p>Enter or map a comma-separated list of parent domain URLs where the returned URLs may be iframed. If left empty, the Adobe Acrobat Sign pages are not viewable in iframe.</p> </li> 
     <li> <p><b>Locale</b> </p> <p>Enter the language that you want to create the view in. </p> </li> 
     <li> <p><b>No chrome flag</b> </p> <p>Select <b>Yes</b> to show the embedded page without a navigation header or footer.</p> </li> 
     <li> <p><b>Send view configuration</b> </p> <p>Select <b>Yes</b> if you want to configure the Send view, then fill in the following fields.</p> 
      <ul> 
       <li> <p><b>Agreement name</b> </p> <p>Enter or map the agreement name for the library document on the compose page.</p> </li> 
       <li> <p><b>Can edit files</b> </p> <p>Select <b>Yes</b> if you want the file upload section to be edited by adding or removing files. This is not an access control machanism. The default is Yes.</p> </li> 
       <li> <p><b>Local file</b> </p> <p>Select <b>Yes</b> if you want library document links to be visible. The default is Yes.</p> </li> 
       <li> <p><b>Web connectors</b> </p> <p>Select <b>Yes</b> if you want the links to attach documents from web sources to appear. The default is Yes.</p> </li> 
       <li> <p><b>Is preview selected</b> </p> <p>Select <b>Yes</b> to set the Compose page to Authoring mode.</p> </li> 
      </ul> <p>&nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">User view info</td> 
   <td> <p>Fill in the following fields</p> 
    <ul> 
     <li> <p><b>Name</b> </p> <p>Select the name of the requested user view.</p> </li> 
     <li> <p><b>Auto login user</b> </p> <p>Select <b>Yes</b> to automatically log the user in. Select <b>No</b> to require credentials. The default is No.</p> </li> 
     <li> <p><b>Frame parent</b> </p> <p>Enter or map a comma-separated list of parent domain URLs where the returned URLs may be iframed. If left empty, the Adobe Acrobat Sign pages are not viewable in iframe.</p> </li> 
     <li> <p><b>No chrome flag</b> </p> <p>Select <b>Yes</b> to show the embedded page without a navigation header or footer.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Widget related fields</td> 
   <td> <p>Select the related record that you want to create.</p> 
    <ul> 
     <li> <p>Views</p> <p>Fill in the following fields.</p> 
      <ul> 
       <li> <p><b>Name</b> </p> <p>Select the name of the requested web form view</p> </li> 
       <li> <p><b>Auto login user</b> </p> <p>Select <b>Yes</b> to automatically log the user in. Select <b>No</b> to require credentials. The default is No.</p> </li> 
       <li> <p><b>Frame parent</b> </p> <p>Enter or map a comma-separated list of parent domain URLs where the returned URLs may be iframed. If left empty, the Adobe Acrobat Sign pages are not viewable in iframe.</p> </li> 
       <li> <p><b>Locale</b> </p> <p>Enter the language that you want to create the view in. </p> </li> 
       <li> <p><b>No chrome flag</b> </p> <p>Select <b>Yes</b> to show the embedded page without a navigation header or footer.</p> </li> 
       <li> <p>Personalized signing view configuration</p> <p>If you want to configure a personalized signing view, select <b>Yes</b> and fill in the following fields:</p> 
        <ul> 
         <li> <p><b>Email</b> </p> <p>Enter the email address of the person who receives the newly created web form</p> </li> 
         <li> <p><b>Comment</b> </p> <p>Enter a comment describing how the API caller established the signer's identity. This information appears in the Adobe Acrobat Sign audit trail.</p> </li> 
         <li> <p><b>Expiration</b> </p> <p>Enter an expiration date for the personalization of this web form. </p> <p>For a list of For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in Adobe Workfront Fusion</a>.</p> </li> 
         <li> <p><b>Reusable</b> </p> <p>Select <b>Yes</b> if you want the intended signer to be able to sign the form more than once.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>Member share</b> </p> <p>For each member that you want to share the agreement with, Click <b>Add item</b> and enter the member's email address and a message to that member.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Custom API Call {#custom-api-call}

This module allows you to perform a custom API call.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>URL</p> </td> 
   <td> <p>Enter a path relative to <code>https://api.[region].adobesign.com/api/rest/v6/</code></p> <p>Note: For the list of available endpoints, refer to the Adobe Sign API Reference.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String </td> 
   <td> <p>Enter the request query string.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Upload a transient document</td> 
   <td> <p>If you want to upload a transient document, enter the source file for the document you want to upload.</p> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List records {#list-records}

This action module lists all records of the selected type that the account has access to.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td>Select the type of record that you want to retrieve related records for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Locale</td> 
   <td> <p>Enter the locale of the user. This determines the language of the UI. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">External ID</td> 
   <td>Enter or map the External ID&nbsp;(an ID assigned outside of Adobe Acrobat Sign) for the agreements you want to return.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Group ID</td> 
   <td>Enter the ID&nbsp;of the group associated with the records you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Show hidden (records)</td> 
   <td>Enable this option if you want to include hidden records in your results.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cursor / Start index</td> 
   <td> <p>Enter the number of the first record that the module should return. </p> <p>Note: This field is combined with the Maximum number of returned records field for pagination. For example, if the Maximum number of returned events is 100, and the Start index is 101, the module returns records 101-200, or the second page of results.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned records</td> 
   <td> <p>Enter or map the maximum number of records you want the module to [action] during each scenario execution cycle.</p> <p>Note: This field is combined with the Cursor or Start Index field for pagination. For example, if the Maximum number of returned events is 100, and the Start index is 101, the module returns records 101-200, or the second page of results.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Parent domain URLs</td> 
   <td> <p>Enter or map a comma-separated list of parent domain URLs where the returned URLs may be iframed. If left empty, the Adobe Acrobat Sign pages are not viewable in iframe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Read a record  {#read-a-record}

This action module retrieves information from a single record.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td>Select the type of record that you want to retrieve related records for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record ID</td> 
   <td>Enter or map the ID&nbsp;of the record you want to retrieve.</td> 
  </tr> 
 </tbody> 
</table>

#### Read related records {#read-related-records}

Read additional information related to a single record.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td>Select the type of record that you want to retrieve related records for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record ID (Example: Account ID)</td> 
   <td>Enter or map the ID&nbsp;of the record you want to retrieve related records for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Other fields</td> 
   <td>Enter information in specific fields based on record type and related fields.</td> 
  </tr> 
 </tbody> 
</table>

#### Update a record  {#update-a-record}

This action module updates a single record in Adobe Acrobat Sign.

>[!IMPORTANT]
>
>* As a best practice, if you are anticipating substantial changes to an agreement, we recommend creating a new agreement rather than updating the existing agreement.
>* Some updates feature required fields. As you configure your update, be sure to fill out all required fields. Required fields are bold in Workfront Fusion modules.
>

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record ID </td> 
   <td>Enter or map the ID&nbsp;of the record you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td>Select the type of record that you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Other fields</td> 
   <td> <p>Enter information in specific fields based on record type and related fields.</p> 
    <ul> 
     <li> <p><b>Agreement</b> </p> <p>As a best practice, if you are anticipating substantial changes to an agreement, we recommend creating a new agreement rather than updating the existing agreement.</p> </li> 
     <li> <p><b>Library document</b> </p> <p>Select the fields you want to update, then fill in the selected fields:</p> 
      <ul> 
       <li> <p><b>Status</b> </p> <p>Select the new status for the library document.</p> </li> 
       <li> <p><b>Name</b> </p> <p>Enter or map the name of the library template</p> </li> 
       <li> <p><b>Sharing mode</b> </p> <p>Specify who should have access to the library document.</p> </li> 
       <li> <p><b>Library template type</b> </p> <p>For each library template type you want to use, click <b>Add item</b> and select the template type.</p> </li> 
      </ul> </li> 
     <li> <p><b>User</b> </p> <p>Select the fields you want to update, then fill in the selected fields:</p> 
      <ul> 
       <li> <p><b>First name</b> </p> <p>Enter the first name of the user.</p> </li> 
       <li> <p><b>Last name</b> </p> <p>Enter the last name of the user</p> </li> 
       <li> <p><b>Company</b> </p> <p>Enter the name of the user's company.</p> </li> 
       <li> <p><b>Phone</b> </p> <p>Enter the phone number of the user</p> </li> 
       <li> <p><b>Primary group ID</b> </p> <p>Enter the group to which the new user is added. If nothing is entered, the user will be added to the default group for the account.</p> </li> 
       <li> <p><b>Job title</b> </p> <p>Enter the job title of the user.</p> </li> 
      </ul> </li> 
     <li> <p><b>Web form (widget)</b> </p> <p>Enter information in specific fields based on record type and related fields.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Update related record {#update-related-record}

This action module updates records related to a specific object.

>[!IMPORTANT]
>
>* As a best practice, if you are anticipating substantial changes to an agreement, we recommend creating a new agreement rather than updating the existing agreement.
>* Some updates feature required fields. As you configure your update, be sure to fill out all required fields. Required fields are bold in Workfront Fusion modules.
>

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td>Select the record type of the record that the related fields are associated with.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Agreement/Library document/User/Widget ID</td> 
   <td>Enter or map the ID&nbsp;of the object that you want to associate the created record with.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Other fields</td> 
   <td> <p>Enter information in specific fields based on record type and related fields.</p> 
    <ul> 
     <li> <p><b>Agreement</b> </p> <p>As a best practice, if you are anticipating substantial changes to an agreement, we recommend creating a new agreement rather than updating the existing agreement.</p> </li> 
     <li> <p><b>Library document</b> </p> <p>Select the fields you want to update, then fill in the selected fields:</p> 
      <ul> 
       <li> <p><b>State</b> </p> <p>Select the new status for the library document.</p> </li> 
       <li> <p><b>Note</b> </p> <p>Enter or map the text of the note.</p> </li> 
       <li> <p><b>Visibility</b> </p> <p>Select whether the library document is shown or gidden.</p> </li> 
      </ul> </li> 
     <li> <p><b>User</b> </p> <p>Select the fields you want to update, then fill in the selected fields:</p> 
      <ul> 
       <li> <p><b>Group info list</b> </p> <p>Fill in the following fields</p> 
        <ul> 
         <li> <p><b>Status</b> </p> <p>Select the new status for the user.</p> </li> 
         <li> <p><b>ID</b> </p> <p>Enter the unique ID&nbsp;of the group</p> </li> 
         <li> <p><b>Is group admin</b> </p> <p>Select <b>Yes</b> to make this user a group administrator.</p> </li> 
         <li> <p><b>Is primary group</b> </p> <p>Select <b>Yes</b> to update this group to the user's primary group.</p> </li> 
         <li> <p><b>Created date</b> </p> <p>Enter the date the group was created.</p> <p>For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in Adobe Workfront Fusion</a>.</p> </li> 
         <li> <p><b>Name</b> </p> <p>Enter or map the name of the group.</p> </li> 
         <li> <p><b>Library document creation visible</b> </p> <p>These settings determine whether the user can create library documents</p> 
          <ul> 
           <li> <p>Allow</p> </li> 
           <li> <p>Inherit group setting from group or account</p> </li> 
          </ul> </li> 
         <li> <p><b>Send restricted to workflows</b> </p> <p>These settings determine whether the user can create agreements only using workflows.</p> 
          <ul> 
           <li> <p>Value</p> <p>Allow</p> </li> 
           <li> <p>Inherited</p> <p>Inherit group setting from group or account</p> </li> 
          </ul> </li> 
         <li> <p><b>User can send</b> </p> 
          <ul> 
           <li> <p>Value</p> <p>Allow</p> </li> 
           <li> <p>Inherited</p> <p>Inherit group setting from group or account</p> </li> 
          </ul> </li> 
        </ul> </li> 
      </ul> 
      <ul> 
       <li> <p><b>State</b> </p> <p>Select the new state for the user, and enter a comment regarding why you want to activate or deactivate the user.</p> </li> 
       <li> <p><b>Locale</b> </p> <p>Enter the locale of the user. This determines the language of the UI. </p> </li> 
      </ul> </li> 
     <li> <p><b>Web form (widget)</b> </p> <p>Enter information in specific fields based on record type and related fields.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

#### Upload document {#upload-document}

Upload a transient document. A transient document is available for 7 days after it is uploaded.

>[!NOTE]
>
>We recommend uploading the document to sign as a transient document, then mapping it to the File to send field in the Create an agreement module.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record ID</td> 
   <td>Enter or map the ID&nbsp;of the record you want to update</td> 
  </tr> 
  <tr> 
   <td role="rowheader">MIME type</td> 
   <td>Enter the mime type of the original file. Multipurpose Internet Mail Extension (MIME) types are labels that allow software to identify different types of data shared on the internet. Web servers and browsers use the MIME type to determine what should be done with a file. For example, a file with the MIME type <code>text/html</code> will be processed in a browser differently than a file with MIME type <code>image/jpeg</code>.</td> 
  </tr> 
 </tbody> 
</table>

**Example:** In this workflow, the document to sign (previously downloaded from Workfront) is uploaded as a transient document.

![](assets/sign-example-1-350x308.png)

The Upload document modules gives the document an Adobe Acrobat Sign ID that can be referenced in later modules. When the agreement is created, the uploaded document's ID is included in the Files to send field.

![](assets/sign-example-2-350x356.png)

### Searches {#searches}

#### Search agreements

This search module searches for agreements based on criteria you provide.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Acrobat Sign account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Text filter</td> 
   <td> <p>Search for text in the agreement metadata. </p> 
    <ul> 
     <li> <p><b>Find text</b> </p> <p>Enter text that you want to find in agreement metadata. Each word is treated as a separate text item. </p> </li> 
     <li> <p><b>Find text in</b> </p> <p>Select the metadata fields that you want to find text in. If you select nothing, the modules searches all metadata.</p> </li> 
    </ul> <p>The module returns any agreement that contains any of the entered text in any of the selected fields. Example: entering "spring campaign" and selecting the Title and Note options returns any agreements with the words "Spring" or "Campaign" in either Title or Note.</p> <p>For more information on searching fields in Adobe Acrobat Sign, see "How text searching works" in <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Adobe Sign Search - How it works</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Created date</td> 
   <td>Select dates. The module returns only records where the created date matches this criteria.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Expiration date</td> 
   <td>Select dates. The module returns only records where the expiration date matches this criteria.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Modified date</p> </td> 
   <td>Select dates. The module returns only records where the modified date matches this criteria.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">External ID</td> 
   <td> <p> External ID is a sender-assigned ID to the agreement that can be of any form, but usually in form of "&lt;groupID&gt;:&lt;ID&gt;".</p> <p>For each External ID you want to add, click <b>Add</b> and enter or map the External ID.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Group ID</td> 
   <td> <p>Group ID is an identifier assigned when the group was created.</p> <p>For each External ID you want to add, click <b>Add</b> and enter or map the External ID.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Asset ID</td> 
   <td> <p>This is the ID&nbsp;assigned to the specific agreement. </p> <p>For each External ID you want to add, click <b>Add</b> and enter or map the External ID.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Parent ID</td> 
   <td> <p>This is the ID&nbsp;assigned to the agreement's parent object. </p> <p>For each External ID you want to add, click <b>Add</b> and enter or map the External ID.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Participant email</td> 
   <td> <p>The email address of a participant. </p> <p>For each External ID you want to add, click <b>Add</b> and enter or map the External ID.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Role</td> 
   <td>Select roles that you want the returned results to include.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort by</td> 
   <td>If you want the module to sort the results, select the field that you want to sort results by.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort order</td> 
   <td>If you want the module to sort the results, select whether you want to sort ascending or descending.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status</td> 
   <td>Select the statuses that you want the returned results to include.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type</td> 
   <td>Select the agreement types that you want the returned results to include.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subtypes</td> 
   <td>Select the agreement subtypes that you want the returned results to include. Only Library&nbsp;template agreements feature subtypes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">User ID</td> 
   <td> <p>The User ID of the user that the agreement is shared with.</p> <p>For each User ID you want to add, click <b>Add</b> and enter or map the User ID.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Visibility</td> 
   <td>Select the visibility level that you want the returned results to include.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Start index</td> 
   <td> <p>Enter the position of the first result that you want to return. Combine this with the maximum returned results to paginate results</p> <p>Example: if you return 100 results at a time, enter 100 to return results 100-200.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned results</td> 
   <td> <p>Enter or map the maximum number of records you want the module to [action] during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

