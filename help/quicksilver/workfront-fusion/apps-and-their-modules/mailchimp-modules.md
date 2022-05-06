

# MailChimp modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use MailChimp, as well as connect it to to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

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
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
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

## Prerequisites

Before you can use the MailChimp connector, you must ensure that the following prerequisites are met:

* You must have an active MailChimp account.

## MailChimp modules and their fields

### Campaigns

#### Create a campaign

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign Title</td> 
   <td> <p> Enter a name for the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List (Audience) ID</td> 
   <td> <p> Select the List ID to whom you want to send the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Segment (Tag) ID</td> 
   <td> <p> Select the Tag ID for the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject Line </td> 
   <td> <p>Enter the subject line of the campaign email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Preview Text </td> 
   <td> <p>Enter the preview text of the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">From Name </td> 
   <td> <p>Enter the name that appears in the From field of the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">From Email Address </td> 
   <td> <p>Enter the email address from which you want to send the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">To Name </td> 
   <td> <p>Enter the recipient's name.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Use Conversation </td> 
   <td> <p>Select the checkbox to use the MailChimp feature for conversation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder ID </td> 
   <td> <p>Select the Folder ID to which you want to add the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fill the Body Content</td> 
   <td> <p> Enter the campaign email message:</p> 
    <ul> 
     <li> <p>By Template ID</p> </li> 
     <li> <p>By HTML Format Text</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Template ID </td> 
   <td> <p>Select the Template ID for the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">HTML Content </td> 
   <td> <p>Enter the campaign's email body message in HTML format.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Campaign

This action module deletes a single campaign from MailChimp.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign ID</td> 
   <td> Select the Campaign ID you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

#### Edit a Campaign Template Content

This action module edits a defined content area of a custom HTML template.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a Campaign ID</td> 
   <td> <p> Select the option to edit the campaign:</p> 
    <ul> 
     <li> <p>Enter Manually</p> </li> 
     <li> <p>Select from List</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign ID</td> 
   <td> <p> Select or enter the Campaign ID you want to edit. You can only edit the campaign with editable campaigns.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Editable Content Area</p> </td> 
   <td> <p>Add the edits:</p> 
    <ul> 
     <li> <p><b>Content Area Name</b> </p> <p>Enter the section you want to edit. For example, if the content area is named mc:edit="section", select section.</p> </li> 
     <li> <p><b>Content of the Area</b> </p> <p>Enter the content you want to add in the HTML format.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Campaign

This action module gets metadata of a specified campaign

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign ID </td> 
   <td>Select the Campaign ID whose details you want to retrieve.</td> 
  </tr> 
 </tbody> 
</table>

#### Get a Campaign Report

This action module gets a campaign report for the specified campaign.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign ID </td> 
   <td>Select the Campaign ID whose report details you want to retrieve.</td> 
  </tr> 
 </tbody> 
</table>

#### Perform a Campaign Action

This action module performs a single campaign action.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign ID </td> 
   <td>Select the Campaign ID to perform the action.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Action</td> 
   <td> <p>Select the action to perform:</p> 
    <ul> 
     <li> <p>Cancel a Campaign</p> </li> 
     <li> <p>Send a Campaign</p> </li> 
     <li> <p>Schedule a Campaign</p> </li> 
     <li> <p>Unschedule a Campaign</p> </li> 
     <li> <p>Pause an RSS-Driven Campaign</p> </li> 
     <li> <p>Resume an RSS-Driven Campaign</p> </li> 
     <li> <p>Replicate a Campaign</p> </li> 
     <li> <p>Send a Test Mail</p> </li> 
     <li> <p>Resend a Campaign</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Campaigns

This search module searches for campaigns based on text you specify.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search </td> 
   <td> <p>Enter a word or phrase to search the campaigns based on the specified entry.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of campaign Integromat should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a Campaign

This action module updates a single campaign.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign ID</td> 
   <td>Select the Campaign ID whose details you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign Title</td> 
   <td> <p> Enter a name for the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List (Audience) ID</td> 
   <td> <p> Select the List ID to whom you want to send the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Segment (Tag) ID</td> 
   <td> <p> Select the Tag ID for the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject Line </td> 
   <td> <p>Enter the subject line of the campaign email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Preview Text </td> 
   <td> <p>Enter the preview text of the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">From Name </td> 
   <td> <p>Enter the name that appears in the From field of the email.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">From Email Address </td> 
   <td> <p>Enter the email address from which you want to send the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">To Name </td> 
   <td> <p>Enter the recipient's name.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Use Conversation </td> 
   <td> <p>Select the checkbox to use the MailChimp feature for conversation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder ID </td> 
   <td> <p>Select the Folder ID to which you want to add the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fill the Body Content</td> 
   <td> <p> Enter the campaign email message:</p> 
    <ul> 
     <li> <p>By Template ID</p> </li> 
     <li> <p>By HTML Format Text</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Template ID </td> 
   <td> <p>Select the Template ID for the campaign.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">HTML Content </td> 
   <td> <p>Enter the campaign's email body message in HTML format.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Campaigns

This trigger module starts a scenario when a new campaign is created or sent.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch Campaigns </td> 
   <td> <p>Select the options for the campaigns you want to watch:</p> 
    <ul> 
     <li> <p>By Created Time</p> </li> 
     <li> <p>By Updated Time</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type</td> 
   <td> <p> Select the campaign type:</p> 
    <ul> 
     <li> <p>Regular</p> </li> 
     <li> <p>Plaintext</p> </li> 
     <li> <p>Absplit</p> </li> 
     <li> <p>RSS</p> </li> 
     <li> <p>Variate</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID </td> 
   <td> <p>Select the campaign List ID you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder ID </td> 
   <td> <p>Select the Folder ID whose campaigns you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Member's Email </td> 
   <td> <p>Enter the email address of the member whose campaigns you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of campaigns Integromat should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Subscriber

#### Add/Update a Subscriber

This action module adds or changes a contact's details.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID </td> 
   <td> <p>Select the List-ID whose subscribers details you want to add or update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email ID</td> 
   <td> <p> Enter the email address of the subscriber whose details you want to add or update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">First Name </td> 
   <td> <p>Enter the first name of the subscriber.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Last Name </td> 
   <td> <p>Enter the last name of the subscriber.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Birthday </td> 
   <td> <p>Enter the birthdate of the subscriber in the MM/DD format.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Create a new customer or update an existing one </td> 
   <td> <p>Select the checkbox to create a new customer or update an existing customer with the above details.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status </td> 
   <td> <p>Select the status for the subscriber:</p> 
    <ul> 
     <li> <p>Subscribed</p> </li> 
     <li> <p>Unsubscribed</p> </li> 
     <li> <p>Cleaned</p> </li> 
     <li> <p>Pending</p> </li> 
     <li> <p>Transactional</p> </li> 
     <li> <p>Archived</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">VIP</td> 
   <td> <p> Select whether the subscriber is a VIP.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email Type</td> 
   <td> <p> Select the email type of the subscriber:</p> 
    <ul> 
     <li> <p>HTML</p> </li> 
     <li> <p>Plain Text</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Language Code</td> 
   <td> <p> Select the language applicable to the subscriber.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tags </td> 
   <td> <p>Add the tags to the subscriber.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Note </td> 
   <td> <p>Enter any additional information about the subscriber you want to mention.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Subcriber

This action module archives or permanently deletes a subscriber.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID </td> 
   <td> <p>Select the List-ID whose subscribers details you want to delete.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email ID </td> 
   <td> <p>Select the email address of the subscriber whose details you want to delete.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a Subscriber permanently </td> 
   <td> <p>Select the checkbox to delete the subscriber permanently.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Edit a Subscriber

This action module edits an existing subscriber.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID </td> 
   <td> <p>Select the List-ID whose subscribers details you want to add or update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email ID</td> 
   <td> <p> Enter the email address of the subscriber whose details you want to add or update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">First Name </td> 
   <td> <p>Enter the first name of the subscriber.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Last Name </td> 
   <td> <p>Enter the last name of the subscriber.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Birthday </td> 
   <td> <p>Enter the birthdate of the subscriber in the MM/DD format.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Create a new customer or update an existing one </td> 
   <td> <p>Select the checkbox to create a new customer or update an existing customer with the above details.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status </td> 
   <td> <p>Select the status for the subscriber:</p> 
    <ul> 
     <li> <p>Subscribed</p> </li> 
     <li> <p>Unsubscribed</p> </li> 
     <li> <p>Cleaned</p> </li> 
     <li> <p>Pending</p> </li> 
     <li> <p>Transactional</p> </li> 
     <li> <p>Archived</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">VIP</td> 
   <td> <p> Select whether the subscriber is a VIP.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email Type</td> 
   <td> <p> Select the email type of the subscriber:</p> 
    <ul> 
     <li> <p>HTML</p> </li> 
     <li> <p>Plain Text</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Language Code</td> 
   <td> <p> Select the language applicable to the subscriber.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tags </td> 
   <td> <p>Add the tags to the subscriber.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Note </td> 
   <td> <p>Enter any additional information about the subscriber you want to mention.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Subscriber

This action module gets metadata of a subscriber by email.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID </td> 
   <td> <p>Select the List-ID whose subscribers details you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email ID </td> 
   <td> <p>Select the email address of the subscriber whose details you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Subscribers

This search module searches for subscribers based on criteria you select.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID </td> 
   <td> <p>Select the Campaign ID whose unsubscribers you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status </td> 
   <td> <p>Select the status of the subscribers you want to search:</p> 
    <ul> 
     <li> <p>Subscribed</p> </li> 
     <li> <p>Unsubscribed</p> </li> 
     <li> <p>Cleaned</p> </li> 
     <li> <p>Pending</p> </li> 
     <li> <p>Transactional</p> </li> 
     <li> <p>Archived</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">VIP Only </td> 
   <td> <p>Select the checkbox if you want to search only VIP subscribers.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email Type </td> 
   <td> <p>Select the email type of the subscribers you want to search:</p> 
    <ul> 
     <li> <p>HTML</p> </li> 
     <li> <p>Plain Text</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Since Date Added </td> 
   <td> <p>Enter the date to search the subscribers added on or after the specified date.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Before Date Added </td> 
   <td> <p>Enter the date to search the subscribers added on or before the specified date.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Since Last Changed Date</td> 
   <td> <p> Enter the date to search the subscribers changed on or after the specified date.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Before Last Changed Date</td> 
   <td> <p> Enter the date to search the subscribers changed on or before the specified date.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort By </td> 
   <td> <p>Select the option to sort the subscribers:</p> 
    <ul> 
     <li> <p>Date Added - Ascending</p> </li> 
     <li> <p>Date Added - Descending</p> </li> 
     <li> <p>Date Signup - Ascending</p> </li> 
     <li> <p>Date Signup - Descending</p> </li> 
     <li> <p>Date Updated - Ascending</p> </li> 
     <li> <p>Date Updated - Descending</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of subscribers Integromat should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Subscribers

This trigger module starts a scenario when a new subscriber joins a list.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID </td> 
   <td> <p>Select the List-ID whose subscribers you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status</td> 
   <td> <p> Select the status of the subscribers you want to watch:</p> 
    <ul> 
     <li> <p>Subscribed</p> </li> 
     <li> <p>Unsubscribed</p> </li> 
     <li> <p>Cleaned</p> </li> 
     <li> <p>Pending</p> </li> 
     <li> <p>Transactional</p> </li> 
     <li> <p>Archived</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">VIP Only </td> 
   <td> <p>Select the checkbox if you want to watch only VIP subscribers.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email Type </td> 
   <td> <p>Select the email type of the subscribers you want to watch:</p> <p>HTML</p> <p>Plain Text</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of subscribers Integromat should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Unsubscribes

This trigger module starts a scenario when a subscriber unsubscribes from a campaign.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your MailChimp account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to Adobe Workfront Fusion - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign ID</td> 
   <td>Select the Campaign ID whose unsubscribers you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of subscribers Integromat should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

List

Create a List

Delete a List

Get a List

Search Lists

Update a List

Watch List Events

Watch Lists

Segment

Add a Member to a Segment

List Segment Members

Remove a Member from a Segment

Watch List Segments

Activity

List List Members' Activities

List List's Activities

Member Tag

Add/Remove Member Tags

List Member Tags

Other

Make an API Call

Watch Files

&nbsp;
