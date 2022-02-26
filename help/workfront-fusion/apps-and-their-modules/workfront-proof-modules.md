---
filename: workfront-proof-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Workfront Proof modules
description: In a Adobe Workfront Fusion scenario, you can connect your Workfront Proof account to multiple third-party applications and services.
---

# *Workfront Proof* modules

In a *Adobe Workfront Fusion* scenario, you can connect your *Workfront Proof* account to multiple third-party applications and services.

This is useful if you need to execute tasks currently not supported in proofing within *Workfront* or in *Workfront Proof*, such as updating proofs based on certain events and searching for a *proof*'s recipients.

The *Workfront Proof*connector does not count against the number of active apps available to your organization. All scenarios, even if they use only the *Workfront Proof*app, do count against your organization's total scenario count.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p>Plan, Work</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront Fusion</em> license**</td> 
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em> </p> <draft-comment>
     <p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p>
    </draft-comment><p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <em>Adobe Workfront Fusion</em> as well as <em>Adobe Workfront</em> to use functionality described in this article.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

&#42;&#42;For information on *Adobe Workfront Fusion* licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## *Workfront Proof* modules and their fields

When you configure *Workfront Proof* modules, *Workfront Fusion* displays the fields listed below. Along with these, additional *Workfront Proof* fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers

* [Watch Proofs](#watch) 
* [Watch for PDF Summary](#watch2) 
* [Watch for PDF Summary](#watch2)

#### Watch Proofs

This scheduled trigger module executes a scenario when someone creates or makes a decision on a proof.

The module returns a list of all of the records it finds during the period you specify, along with their types. It also returns the values of the fields you specify. If the module found decisions make on the proof, it includes both the previous and the current values, in separate fields. You can map *this information* in subsequent modules in the scenario.

This happens on a regularly scheduled interval that you specify.

You must have sufficient permissions to access the *proof or proofs* in *Workfront Proof* in order to retrieve this information.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of <em>Workfront Proof</em> record that you want the module to <em>watch</em>.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Outputs</td> 
    <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Limit</td> 
    <td> <p>Enter or map the maximum number of <em>record</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of <em>record</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch for PDF Summary

This instant trigger module executes a scenario when someone creates a PDF summary for a *proof*.

A webhook is required in this module.

The module returns all standard fields associated with the *proof*, along with any custom fields and values that the connection accesses. It also creates a new event subscription for PDF summaries and outputs the content from the “pdf_url” attribute sent in the payload. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Webhook</td> 
   <td>You can select an existing webhook or create a new one. For more information, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant triggers (webhooks)</a>. </td> 
  </tr> 
  <tr> 
   <td>Limit</td> 
   <td>Enter or map the maximum number of <em>record</em>s you want the module to <em>return</em> during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Watch Proof Activity

This trigger module executes a scenario whena specified activity occurs on a proof *proof*.

The module returns all standard fields associated with the *proof*, along with any custom fields and values that the connection accesses. It also creates a new event subscription for PDF summaries and outputs the content from the “pdf_url” attribute sent in the payload. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Activity type</td> 
   <td>Select whether you want to watch any new decision (including <em>proof</em> status changes), or overall <em>proof</em> status changes only.</td> 
  </tr> 
  <tr> 
   <td>Limit</td> 
   <td>Enter or map the maximum number of <em>record</em>s you want the module to <em>return</em> during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [Create Proof](#create) 
* [Custom API Call](#custom) 
* [Download Proof](#download) 
* [Read a Record](#read) 
* [Request PDF Summary](#request) 
* [Possible error](#possible) 
* [Update Proof](#update) 
* [Upload File](#upload)

#### Create Proof

This action module creates a new *proof* or a new version of a *proof* in *Workfront Proof*.

You specify the parameters for the new *proof* and the source *proof* if you are creating a new version.

The module returns the ID of the new *proof* or *proof* version.You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Proof Type</td> 
   <td> <p>Specify whether you want the <em>proof</em> that is created to have a basic workflow or an Automated Workflow.</p> <p>Then fill out the fields that display for the proof type you chose. For example, if you chose Automated Workflow, fill out the <span class="bold">Workflow Stages</span> field to configure the stages.</p> <p>You can use output from the Build module here if you include and run that module earlier in the scenario. For more information, see <a href="#build" class="MCXref xref">Build</a> in this article. <draft-comment>
      <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span>
     </draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span></p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Allow original file to be downloaded</td> 
    <td>Select whether you want to allow the original file that the proof was created from to be downloaded.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Allow original file to be downloaded</td> 
   <td>Select whether you want to allow the original file that the proof was created from to be downloaded.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Classic Proof Viewer</td> 
    <td>Select whether you are using the Classic Proof Viewer.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Classic Proof Viewer</td> 
   <td>Select whether you are using the Classic Proof Viewer.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Combine all files into single proof</td> 
    <td>Enable this option to combine all files into a single multi-page proof.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Combine all files into single proof</td> 
   <td>Enable this option to combine all files into a single multi-page proof.</td> 
  </tr> 
  <tr> 
   <td>Create a new <em>proof</em> version<draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      ?
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
     ?
    </MadCap:conditionalText></td> 
   <td>Select this option if you want the module to create a new version of an existing <em>proof</em>. Then, in the <span class="bold">Existing Proof ID</span> field that displays, map or enter the unique ID of the <em>proof</em>.</td> 
  </tr> 
  <tr> 
   <td>Custom Link Label</td> 
   <td>Enter or map a label for the custom proof link.</td> 
  </tr> 
  <tr> 
   <td>Custom Link URL</td> 
   <td>Enter or map the URL for the custom link.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Default email notifications for subscribers</td> 
    <td>Type one of the following numbers to indicate which of the following default email notification settings you want to use for the <em>proof</em> that is created.
     <ul>
      <li><span class="bold">1</span> - All new comments and replies</li>
      <li><span class="bold">2</span> - Replies to my comments</li>
      <li><span class="bold">3</span> - Daily summary</li>
      <li><span class="bold">4</span> - Hourly summary</li>
      <li><span class="bold">5</span> - Decisions only</li>
      <li><span class="bold">9</span> - Disabled</li>
     </ul></td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Default email notifications for subscribers</td> 
   <td>Type one of the following numbers to indicate which of the following default email notification settings you want to use for the <em>proof</em> that is created.
    <ul>
     <li><span class="bold">1</span> - All new comments and replies</li>
     <li><span class="bold">2</span> - Replies to my comments</li>
     <li><span class="bold">3</span> - Daily summary</li>
     <li><span class="bold">4</span> - Hourly summary</li>
     <li><span class="bold">5</span> - Decisions only</li>
     <li><span class="bold">9</span> - Disabled</li>
    </ul></td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Disable Excel Summary</td> 
    <td>Select whether you want to disable the ability to download <em>proof</em> comments to an Excel file.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Disable Excel Summary</td> 
   <td>Select whether you want to disable the ability to download <em>proof</em> comments to an Excel file.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Disable PDF Summary</td> 
    <td>Select whether you want to disable the ability to download <em>proof</em> comments to a PDF file.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Disable PDF Summary</td> 
   <td>Select whether you want to disable the ability to download <em>proof</em> comments to a PDF file.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Disable Subscription Email</td> 
    <td>Select whether you want to disable the subscription email for this proof.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Disable Subscription Email</td> 
   <td>Select whether you want to disable the subscription email for this proof.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Enable Embed Player</td> 
    <td>Select whether you want to enable the embedded player for this proof.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Enable Embed Player</td> 
   <td>Select whether you want to enable the embedded player for this proof.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Enable Subscriptions</td> 
    <td>Select whether people who are not participants are allowed to subscribe to the proof.<br>If you select this option, you can also select the Default Role for subscribers, as described in this table.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Enable Subscriptions</td> 
   <td>Select whether people who are not participants are allowed to subscribe to the proof.<br>If you select this option, you can also select the Default Role for subscribers, as described in this table.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Enable Subscriptions Validation</td> 
    <td>Select whether you want to enable subscription email validation. If this is enabled, the subscriber must click a link in an email to access a proof.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Enable Subscriptions Validation</td> 
   <td>Select whether you want to enable subscription email validation. If this is enabled, the subscriber must click a link in an email to access a proof.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Enable Team URL</td> 
    <td>Select whether you want the proof that is created to hide or show the team URL.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Enable Team URL</td> 
   <td>Select whether you want the proof that is created to hide or show the team URL.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>File Hash <span style="font-weight: normal;">or</span> File Hashes</td> 
    <td>Add the ID of the file or files from which you want to create a <em>proof</em> or <em>proofs</em>.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>File Hash <span style="font-weight: normal;">or</span> File Hashes</td> 
   <td>Add the ID of the file or files from which you want to create a <em>proof</em> or <em>proofs</em>.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>File Names</td> 
    <td>Add the file name or names for the <em>proof</em> that is created This is a required field.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>File Names</td> 
   <td>Add the file name or names for the <em>proof</em> that is created This is a required field.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Lock proof when all required decisions are made</td> 
    <td>Specify whether you want the <em>proof</em> that is created to lock after all required decisions are made.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Lock proof when all required decisions are made</td> 
   <td>Specify whether you want the <em>proof</em> that is created to lock after all required decisions are made.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Notify recipients about this proof</td> 
    <td>Select an option to indicate whether you want recipients notified when the <em>proof</em> is created.<draft-comment>
      <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> If you select yes, select an option to indicate/include (?) a Custom message subject, Custom message body</span>
     </draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> If you select yes, select an option to indicate/include (?) a Custom message subject, Custom message body</span></td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Notify recipients about this proof</td> 
   <td>Select an option to indicate whether you want recipients notified when the <em>proof</em> is created.<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> If you select yes, select an option to indicate/include (?) a Custom message subject, Custom message body</span></td> 
  </tr> 
  <tr> 
   <td>Proof name</td> 
   <td>Type a name for the <em>proof</em> that is created This is a required field. Use a pipe symbol (|) to separate names for multiple proofs.</td> 
  </tr> 
  <tr> 
   <td>Proof owner ID</td> 
   <td>Enter or map the ID&nbsp;of the proof owner. If this field is left blank, the proof owner is set to the current user.</td> 
  </tr> 
  <tr> 
   <td>Reference ID</td> 
   <td>Enter the reference ID for the proof.</td> 
  </tr> 
  <tr> 
   <td>Require electronic signature</td> 
   <td>Select whether you want to require an anyone who makes a decision on a proof to submit an electronic signature.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Require login</td> 
    <td> <p>Specify whether you want the <em>proof</em> that is created to require a login. </p> <p>This is the same as the Login Required setting explained in <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a></p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Require login</td> 
   <td> <p>Specify whether you want the <em>proof</em> that is created to require a login. </p> <p>This is the same as the Login Required setting explained in <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a></p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Resolution ID</td> 
    <td>Enter the ID&nbsp;of the resolution you want to use for your proof. For a list of resolution IDs, see the <em>Workfront Proof</em> <a href="http://api.proofhq.com/home/objects/soapworkflowproofobject">API documentation</a>.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Resolution ID</td> 
   <td>Enter the ID&nbsp;of the resolution you want to use for your proof. For a list of resolution IDs, see the <em>Workfront Proof</em> <a href="http://api.proofhq.com/home/objects/soapworkflowproofobject">API documentation</a>.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>SWF</td> 
    <td>Enter the type of SWF proof.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>SWF</td> 
   <td>Enter the type of SWF proof.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Show [item]</td> 
    <td>For each item, select whether you want to show it in the proof.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Show [item]</td> 
   <td>For each item, select whether you want to show it in the proof.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Workspace ID</td> 
    <td>Enter the ID&nbsp;of the workspace you want to create the proof in. </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Workspace ID</td> 
   <td>Enter the ID&nbsp;of the workspace you want to create the proof in. </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Recipients</td> 
    <td>Add the email addresses of the recipients you want for the <em>proof</em> that is created .</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Recipients</td> 
   <td>Add the email addresses of the recipients you want for the <em>proof</em> that is created .</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Deadline</td> 
    <td> <p>Specify the deadline you want for the <em>proof</em> that is created. Use the following date format:</p> <p>YYYY-MM-DD hh:mm</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Deadline</td> 
   <td> <p>Specify the deadline you want for the <em>proof</em> that is created. Use the following date format:</p> <p>YYYY-MM-DD hh:mm</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Custom API Call

This action module lets you make a custom authenticated call to the *Workfront Proof* API

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
without having to think through authentication
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  without having to think through authentication</MadCap:conditionalText>`. This way, you can create a data flow automation that can't be accomplished by the other *Workfront Proof* modules.

The module returns the status code, headers and body. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Method</td> 
    <td>Set the action for the API call. For available actions, see the <a href="http://api.proofhq.com/">Proof&nbsp;API documentation</a>.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Method</td> 
   <td>Set the action for the API call. For available actions, see the <a href="http://api.proofhq.com/">Proof&nbsp;API documentation</a>.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Body (XML)</td> 
    <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>"> 
       <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
      </div> </p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Body (XML)</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

` `**Example: **``  ![](assets/wfp-api-module-example-350x586.png)

#### Download Proof

This action module downloads the source file of a particular *proof* that you identify using its ID.

You specify the *proof*'s ID.

The module returns the content of the source file used to create the *proof*.You can map *this information* in subsequent modules in the scenario.

You must have sufficient permissions to access the *record* in *Workfront Proof* in order to retrieve this information.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Proof ID</td> 
   <td> <p>Type the unique ID of the <em>proof</em>, found on the Proof Details page. For more information, see <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Manage Proof Details in Workfront Proof</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Read a Record

This action module reads data from a single *proof* in *Workfront Proof*.

You specify the proof's ID and the information you want from the proof.

The module returns the values of the fields you choose for the proof, along with their types. You can map *this information* in subsequent modules in the scenario.

You must have sufficient permissions to access the *record* in *Workfront Proof* in order to retrieve this information.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Record Type</td> 
   <td>Select whether you want to read a <em>proof</em>, <em>proof</em> comments, or <em>proof</em> reviewers.</td> 
  </tr> 
  <tr> 
   <td>Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td>Enter or map the unique <em>Workfront Proof</em> ID of the <em>record</em> that you want the module to <em>read</em>.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>________</td> 
    <td>Select the type of information you want the module to read: proof, proof comments, proof reviewers, or Automated Workflow template. After you choose one of these 4 options, select the fields you want to include for that option.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td>________</td> 
   <td>Select the type of information you want the module to read: proof, proof comments, proof reviewers, or Automated Workflow template. After you choose one of these 4 options, select the fields you want to include for that option.</td> 
  </tr> 
 </tbody> 
</table>

#### Request PDF Summary

This action module requests the PDF summary for a particular *proof* in *Workfront Proof*.

You specify the *proof*'s ID.

The module returns PDF summary information. You can map *this information* in subsequent modules in the scenario.

You must have sufficient permissions to access the *record* in *Workfront Proof* in order to retrieve this information.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Proof ID</td> 
   <td> <p>Enter the unique <em>Workfront Proof</em> ID of the <em>proof</em> for which you want to request a PDF summary.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Callback URL</td> 
    <td>Enter or map the URL where you want the PDF&nbsp;summary sent.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Callback URL</td> 
   <td>Enter or map the URL where you want the PDF&nbsp;summary sent.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Proof versions</td> 
    <td>Specify whether you want to include all versions of the <em>proof</em> or a specific one.<draft-comment>
      <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> I'm guessing on this</span>
     </draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> I'm guessing on this</span></td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td>Proof versions</td> 
   <td>Specify whether you want to include all versions of the <em>proof</em> or a specific one.<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> I'm guessing on this</span></td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Webhook URL</td> 
    <td> <p>You can create a separate scenario that uses the Watch for PDF Summary trigger module with a new webhook to retrieve the URL.<draft-comment>
       <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Is this right?</span>
      </draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Is this right?</span></p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td>Webhook URL</td> 
   <td> <p>You can create a separate scenario that uses the Watch for PDF Summary trigger module with a new webhook to retrieve the URL.<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Is this right?</span></p> </td> 
  </tr> 
 </tbody> 
</table>

##### Possible error

* `Error`: “You do not have privilege to perform this request. The stage must contain at least one recipient.”
* `Solution`: Make sure you are not the only one assigned to the stages of the workflow. There must be another user assigned to the stages of the workflow.

#### Update Proof

This action module updates an existing *proof* in *Workfront Proof*.

You specify the *proof*'s ID and record type and what fields you want to include in the output.

The module returns any standard fields associated with the record

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
or records
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  or records</MadCap:conditionalText>`, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

You must have sufficient permissions to access the *record* in *Workfront Proof* in order to retrieve this information.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Proof ID</td> 
   <td> <p>Type the unique ID of the <em>proof</em>, found on the Proof Details page. For more information, see <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Manage Proof Details in Workfront Proof</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Deadline</td> 
   <td> <p>Specify the deadline you want for the <em>proof</em> that is created. Use the following date format:</p> <p>YYYY-MM-DD hh:mm</p> </td> 
  </tr> 
  <tr> 
   <td>Default email notifications for subscribers</td> 
   <td>Select which of the following default email notification settings you want to use for the <em>proof</em> that is created.
    <ul>
     <li> All new comments and replies</li>
     <li>Replies to my comments</li>
     <li>Daily summary</li>
     <li> Hourly summary</li>
     <li> Decisions only</li>
     <li> Disabled</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Default Role</td> 
   <td>Select the default role for the proof.</td> 
  </tr> 
  <tr> 
   <td>Disable Subscription Email</td> 
   <td>Select whether you want to disable the subscription email for this proof.</td> 
  </tr> 
  <tr> 
   <td>Enable Subscriptions</td> 
   <td>Select whether people who are not participants are allowed to subscribe to the proof.<br>If you select this option, you can also select the Default Role for subscribers, as described in this table.</td> 
  </tr> 
  <tr> 
   <td>Enable Subscriptions Validation</td> 
   <td>Select whether you want to enable subscription email validation. If this is enabled, the subscriber must click a link in an email to access a proof.</td> 
  </tr> 
  <tr> 
   <td>Enable Team URL</td> 
   <td>Select whether you want the proof that is created to hide or show the team URL.</td> 
  </tr> 
  <tr> 
   <td>Lock proof when all required decisions are made</td> 
   <td>Specify whether you want the <em>proof</em> that is created to lock after all required decisions are made.</td> 
  </tr> 
  <tr> 
   <td>Message</td> 
   <td>Enter or map a message that you want to accompany the proof.</td> 
  </tr> 
  <tr> 
   <td>Proof ID </td> 
   <td>Enter or map the ID&nbsp;of the proof you want to update.</td> 
  </tr> 
  <tr> 
   <td>Proof Name</td> 
   <td>Enter or map the name of the proof you want to update.</td> 
  </tr> 
  <tr> 
   <td>Require login</td> 
   <td> <p>Specify whether you want the <em>proof</em> that is created to require a login. </p> <p>This is the same as the Login Required setting explained in <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a></p> </td> 
  </tr> 
  <tr> 
   <td>Show Versions Like</td> 
   <td>Select whether you want to show a link to other versions of this proof.</td> 
  </tr> 
  <tr> 
   <td>Subject</td> 
   <td>Enter or map the subject of the proof</td> 
  </tr> 
 </tbody> 
</table>

#### Upload File

This action module uploads a file for use with the Create Proof module in *Workfront Proof*.

The module returns a hash ID for the uploaded file. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Source file</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Name</td> 
    <td>(Optional) Type a new file name for the uploaded file if you don't want to use the existing one. <draft-comment>
      <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
       <draft-comment>
        <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span>
       </draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span></span>
     </draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span></span></td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td>Name</td> 
   <td>(Optional) Type a new file name for the uploaded file if you don't want to use the existing one. <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span></span></td> 
  </tr> 
 </tbody> 
</table>

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Are there more main fields for this module?</p>
-->

Are there more main fields for this module?

### Searches

* [Search](#search) 
* [List Workflow Templates](#list)

#### Search

This search module looks for *records in an object* in *Workfront Proof* that match the search query you specify.

The module returns the *proof*'s ID if it's searching for a proof. Or it returns the recipients' user IDs, emails, names, positions, and email aliases, if it is searching for recipients.You can map *this information* in subsequent modules in the scenario.

You must have sufficient permissions to access the *record* in *Workfront Proof* in order to retrieve this information.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Search for</td> 
    <td> <p>Select the type of record you want the module to search for.</p> 
     <ul> 
      <li> <p><span class="bold">Proof </span> </p> <p>Enter the Proof Name of the proof you want to search for.</p> </li> 
      <li> <p><span class="bold">Recipient</span> </p> <p>Enter the email address of the recipient you want to search for.</p> </li> 
     </ul> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Search for</td> 
   <td> <p>Select the type of record you want the module to search for.</p> 
    <ul> 
     <li> <p><span class="bold">Proof </span> </p> <p>Enter the Proof Name of the proof you want to search for.</p> </li> 
     <li> <p><span class="bold">Recipient</span> </p> <p>Enter the email address of the recipient you want to search for.</p> </li> 
    </ul> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Result Set</td> 
    <td>Indicate whether the module will search for <span class="bold">All Matching Records</span> or only the <span class="bold">First Matching Record</span>.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Result Set</td> 
   <td>Indicate whether the module will search for <span class="bold">All Matching Records</span> or only the <span class="bold">First Matching Record</span>.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Sort By</td> 
    <td>Select the field that you want to sort results by.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Sort By</td> 
   <td>Select the field that you want to sort results by.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Sorting Direction</td> 
    <td> <p>Select whether you want to sort results ascending or descending.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Sorting Direction</td> 
   <td> <p>Select whether you want to sort results ascending or descending.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Workflow Templates

This search module lists all available workflow templates.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Limit</td> 
    <td> <p>Enter or map the maximum number of <em>template</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Limit</td> 
   <td> <p>Enter or map the maximum number of <em>template</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3><a name="Build"></a>Build</h3> <draft-comment>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">I don't see this in Fusion 2</p>
</draft-comment>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">I don't see this in Fusion 2</p>
<p>This action module <em>creates a new proof recipient or stage in an Automated Workflow</em><draft-comment>
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Workfront Proof</em>
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Workfront Proof</em>
</MadCap:conditionalText>.</p>
<p>The module returns reviewer or stage information (see the examples below the following table). You can map <em>this information</em> in subsequent modules in the scenario.</p>
<p>When you are configuring this module, the following fields display<draft-comment>
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront Proof</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>.</p>
<table>
<col>
<col>
<tbody>
<tr>
<td>Connection</td>
<td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td>
</tr> <draft-comment>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
________
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
________
</MadCap:conditionalText> </td>
<td>Select an option to specify whether you are adding a reviewer or a stage in an Automated Workflow.</td>
</tr>
</draft-comment>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
________
</MadCap:conditionalText> </td>
<td>Select an option to specify whether you are adding a reviewer or a stage in an Automated Workflow.</td>
</tr> <draft-comment>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td>Reviewer</td>
<td>If you are adding a reviewer, select <draft-comment>
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(or is it fill out?)</span>
</draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(or is it fill out?)</span> the fields containing the reviewer information you want to use.</td>
</tr>
</draft-comment>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td>Reviewer</td>
<td>If you are adding a reviewer, select <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(or is it fill out?)</span> the fields containing the reviewer information you want to use.</td>
</tr> <draft-comment>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td>Stage</td>
<td>If you are adding a stage, select <draft-comment>
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(or is it fill out?)</span>
</draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(or is it fill out?)</span> the fields containing the stage information you want to use.</td>
</tr>
</draft-comment>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td>Stage</td>
<td>If you are adding a stage, select <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(or is it fill out?)</span> the fields containing the stage information you want to use.</td>
</tr>
</tbody>
</table>
<div class="examples" data-mc-autonum="<b>Examples: </b>">
<span class="autonumber"><span><b>Examples: </b></span></span>
<ul>
<li> <p>For a reviewer, the module returns data such as the following:</p><pre>{</pre><pre>"primary_decision_maker": true,</pre><pre>"email_notification": 1,</pre><pre>"role": 3,</pre><pre>"email": "name@company.com"</pre><pre>}</pre> </li>
<li> <p>For a stage, the module returns data such as the following:</p><pre>{</pre><pre>"stage_id": 0,</pre><pre>"start_dependent_time": "13.00",</pre><pre>"start_dependent_stage_id": "2",</pre><pre>"deadline_time": "",</pre><pre>"name": "Stage Name",</pre><pre>"stage_one_decision_only": true,</pre><pre>"deadline_date": "01.01.2020",</pre><pre>"stage_reviewers": [],</pre><pre>"start_trigger": 1,</pre><pre>"stage_locking": 4,</pre><pre>"start_dependent_date": "01.02.2020",</pre><pre>"stage_private": true,</pre><pre>"deadline_calculate_on": 1</pre><pre>}</pre> </li>
</ul>
</div>
</div>
-->

### Build

I don't see this in Fusion 2

This action module *creates a new proof recipient or stage in an Automated Workflow*`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Workfront Proof</em></MadCap:conditionalText>`.

The module returns reviewer or stage information (see the examples below the following table). You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront Proof</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront Proof</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
     ________
    </MadCap:conditionalText> </td> 
   <td>Select an option to specify whether you are adding a reviewer or a stage in an Automated Workflow.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td>Reviewer</td> 
   <td>If you are adding a reviewer, select <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(or is it fill out?)</span> the fields containing the reviewer information you want to use.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td>Stage</td> 
   <td>If you are adding a stage, select <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(or is it fill out?)</span> the fields containing the stage information you want to use.</td> 
  </tr> 
 </tbody> 
</table>

` `**Examples: **``

* For a reviewer, the module returns data such as the following:
  <pre>{</pre><pre>"primary_decision_maker": true,</pre><pre>"email_notification": 1,</pre><pre>"role": 3,</pre><pre>"email": "name@company.com"</pre><pre>}</pre>

* For a stage, the module returns data such as the following:
  <pre>{</pre><pre>"stage_id": 0,</pre><pre>"start_dependent_time": "13.00",</pre><pre>"start_dependent_stage_id": "2",</pre><pre>"deadline_time": "",</pre><pre>"name": "Stage Name",</pre><pre>"stage_one_decision_only": true,</pre><pre>"deadline_date": "01.01.2020",</pre><pre>"stage_reviewers": [],</pre><pre>"start_trigger": 1,</pre><pre>"stage_locking": 4,</pre><pre>"start_dependent_date": "01.02.2020",</pre><pre>"stage_private": true,</pre><pre>"deadline_calculate_on": 1</pre><pre>}</pre>

