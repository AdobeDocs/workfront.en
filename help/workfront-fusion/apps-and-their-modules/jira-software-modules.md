

# Jira Software modules

In a *Adobe Workfront Fusion* scenario, you can connect your *Jira Software* account to multiple third-party applications and services.

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
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em> </p> </td> 
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

## Prerequisites

To use Jira modules you must have a Jira account.

## Connect Jira Software to *Workfront Fusion*

Your connection method is based on whether you are using Jira Cloud or Jira Server.

* [Connect Jira Cloud to Workfront Fusion](#connect) 
* [Connect Jira Server to Workfront Fusion](#connect2)

### Connect Jira Cloud to *Workfront Fusion*

Connect Jira Cloud to *Workfront Fusion*

To connect Jira Software to *Workfront Fusion*, you must create an API token and insert it together with your Service URL and Username to the Create a connection field in *Workfront Fusion*.

#### Create an API&nbsp;token in Jira

<ol> 
 <li value="1">Go to <a href="https://id.atlassian.com/manage/api-tokens">https://id.atlassian.com/manage/api-tokens</a> and log in.</li> 
 <li value="2">Click <span class="bold">Create API token</span>.</li> 
 <li value="3">Type a name for the token, such as <i>Workfront Fusion</i>.</li> 
 <li value="4"> <p>Copy the token using the <span class="bold">Copy to clipboard</span> button.</p> <note type="important">
   You can't view the token again after closing this dialog.
  </note> </li> 
 <li value="5">Store the generated token in a safe place.</li> 
 <li value="6">Continue with <a href="#configur2" class="MCXref xref">Configure the Jira API token in Workfront Fusion</a>.</li> 
</ol>

#### Configure the Jira API token in *Workfront Fusion*

1. In *Workfront Fusion*, add a Jira module to a scenario to open the `Create a connection` box.

1. Specify the following information:

  * `Service URL:`
  * `Username:`
  * `API token:`&nbsp;This is the API token you created in the [Create an API token in Jira](#create3) section of this article.

1. Click Continue to create the connection and return to the module.

### Connect Jira Server to *Workfront Fusion*

To authorize a connection between *Workfront Fusion* and Jira Server, you need your Consumer Key, Private Key, And Service URL. You might need to contact your Jira administrator for this information.

* [Generate Public and Private keys for your Jira connection](#generate) 
* [Configure the client app as a consumer in Jira](#configur) 
* [Create a connection to Jira Server or Jira Data Center in Workfront Fusion](#create2)

#### Generate Public and Private keys for your Jira connection

To acquire a private key for your *Workfront Fusion* Jira connection, you need to generate public and private keys.

<ol> 
 <li value="1"> <p>In your terminal, run the following <code>openssl </code>commands.</p> 
  <ul> 
   <li><pre>openssl genrsa -out jira_privatekey.pem 1024</pre> <p>This command generates a 1024 bit private key.</p> </li> 
   <li><pre>openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365</pre> <p>This command creates an X509 certificate.</p> </li> 
   <li><pre>openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8</pre> <p>This command extracts the private key (PKCS8 format) to the <code>jira_privatekey.pcks8</code> file.</p> </li> 
   <li><pre>openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem</pre> <p>This command extracts the public key from the certificate to the<code> jira_publickey.pem</code> file.</p> <note type="note"> 
     <p>If you are using Windows, you might need to save the public key to the <code>jira_publickey.pem</code> file manually:</p> 
     <ol> 
      <li value="1"> <p>In your terminal, run the following command:</p> <p>openssl x509 -pubkey -noout -in jira_publickey.cer </p> </li> 
      <li value="2">Copy the terminal output (including <code>-------BEGIN PUBLIC KEY--------</code> and <code>-------END PUBLIC KEY--------</code></li> 
      <li value="3">Paste the terminal output into a file named <code>jira_publickey.pem</code>.</li> 
     </ol> 
    </note> </li> 
  </ul> </li> 
 <li value="2"> <p>Continue to <a href="#configur" class="MCXref xref">Configure the client app as a consumer in Jira</a></p> </li> 
</ol>

#### Configure the client app as a consumer in Jira

<ol> 
 <li value="1"> <p>Log into your Jira instance.</p> </li> 
 <li value="2"> <p>In the left navigation panel, click <span class="bold">Jira Settings</span><img src="assets/jira-settings-icon.png"> > <span class="bold">Applications</span>> <span class="bold">Application links</span>.</p> </li> 
 <li value="3"> <p>In the <span class="bold">Enter the URL of the application you want to link</span> field, enter <code>https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1</code></p> </li> 
 <li value="4"> <p>Click <span class="bold">Create new link</span>. Ignore the "No response was received from the URL you entered" error message.</p> </li> 
 <li value="5"> <p>In the <span class="bold">Link applications</span> window, enter values into the <span class="bold">Consumer key</span> and <span class="bold">Shared secret</span> fields. You can choose the values for these fields. </p> </li> 
 <li value="6"> <p>Copy the values of the <span class="bold">Consumer key</span> and <span class="bold">Shared secret</span> fields to a secure location. You will require these values later in the configuration process.</p> </li> 
 <li value="7"> <p>Fill in the URL fields as follows:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Request Token URL</td> 
     <td><code><Jira base url>/plugins/servlet/oauth/request-token</code> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Authorization URL</td> 
     <td><code><Jira base url>/plugins/servlet/oauth/authorize</code> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Access Token URL</td> 
     <td><code><Jira base url>/plugins/servlet/oauth/access-token</code> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="8"> <p>Select the <span class="bold">Create incoming link</span> checkbox.</p> </li> 
 <li value="9"> <p>Click <span class="bold">Continue</span>.</p> </li> 
 <li value="10"> <p> the <span class="bold">Link applications</span> window, fill in the following fields:</p> 
  <table cellspacing="0"> <draft-comment>
    <col data-mc-conditions="">
   </draft-comment>
   <col data-mc-conditions=""> <draft-comment>
    <col data-mc-conditions="">
   </draft-comment>
   <col data-mc-conditions=""> 
   <tbody> 
    <tr> 
     <td role="rowheader"> <p>Consumer Key</p> </td> 
     <td> Paste in the consumer key that you copied to a secure location.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Consumer name</td> 
     <td>Enter a name of your choice. This name is for your own reference.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Public key</td> 
     <td>Paste in the public key from your <code>jira_publickey.pem</code> file.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="11"> <p>Click <span class="bold">Continue</span></p> </li> 
 <li value="12"> <p>Continue to <a href="#create2" class="MCXref xref">Create a connection to Jira Server or Jira Data Center in Workfront Fusion</a></p> </li> 
</ol>

#### Create a connection to Jira Server or Jira Data Center in *Workfront Fusion*

>[!NOTE]
>
>Use the Jira Server app to connect to Jira Server or Jira Data Center.

<ol> 
 <li value="1">In any Jira Server module in <em>Workfront Fusion</em>, click <span class="bold">Add</span> next to the connection field.</li> 
 <li value="2"> <p>In the Create a connection panel, fill in the following fields:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"> <p>Connection name</p> </td> 
     <td> <p>Enter a name for the connection</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Consumer Key</td> 
     <td>Paste in the consumer key that you copied to a secure location in <a href="#configur" class="MCXref xref">Configure the client app as a consumer in Jira</a></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Private Key</td> 
     <td>Paste in the private key from the <code>jira_privatekey.pcks8</code> file you created in <a href="#generate" class="MCXref xref">Generate Public and Private keys for your Jira connection</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Service URL</td> 
     <td>Enter your Jira instance URL. </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3">Click <span class="bold">Continue</span> to create the connection and go back to the module.</li> 
</ol>

## Jira Software modules and their fields

When you configure *Jira Software* modules, *Workfront Fusion* displays the fields listed below. Along with these, additional *Jira Software* fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers

#### Watch for records

This trigger module starts a scenario when a record is added, updated, or deleted.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook</td> 
   <td> <p>Select the webhook that you want to use to watch for records. </p> <p>To add a new webhook:</p> 
    <ol> 
     <li value="1">Click <span class="bold">Add</span></li> 
     <li value="2">Enter a name for the webhook.</li> 
     <li value="3"> <p>Select the connection you want to use for your webhook. </p> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </li> 
     <li value="4"> <p>Select the record type that you want the software to watch for:</p> 
      <ul> 
       <li>Comment </li> 
       <li>Issue</li> 
       <li>Project </li> 
       <li>Sprint</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [Add issue to sprint](#add) 
* [Custom API Call](#custom) 
* [Create a Record](#create) 
* [Delete a record](#delete) 
* [Download an attachment](#download) 
* [Read a record](#read) 
* [Update a record](#update)

#### Add issue to sprint

This action module *adds one or more issues to a sprint*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Jira Software</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Jira Software</em></MadCap:conditionalText>`.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Jira Software</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Jira Software</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sprint ID</td> 
   <td>Enter or map the Sprint ID of the sprint that you want to add an issue to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Issue ID or Keys</td> 
   <td>Add an Issue ID or Key for each issue you want to add to the sprint.</td> 
  </tr> 
 </tbody> 
</table>

#### Create a Record

This action module creates a new record in Jira.

The module returns any standard fields associated with the record

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
or records
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  or records</MadCap:conditionalText>`, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Jira Software</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Jira Software</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to create. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Attachment</li> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
     <li>Worklog</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Custom API Call

This action module lets you make a custom authenticated call to the *Jira Software* API

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
without having to think through authentication
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  without having to think through authentication</MadCap:conditionalText>`. This way, you can create a data flow automation that can't be accomplished by the other *Jira Software* modules.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Jira Software</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Jira Software</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter a path relative to<code>&lt;Instance URL&gt;/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p><em>Workfront Fusion</em> adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a record

This action module *deletes a particular record*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Jira Software</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Jira Software</em></MadCap:conditionalText>`.

You specify the

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
type and
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  type and</MadCap:conditionalText>` ID of the *record*.

The module returns the ID of the 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
<em>deleted</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <em>deleted</em></MadCap:conditionalText>` *record* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Jira Software</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Jira Software</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to delete. </p> 
    <ul> 
     <li>Attachment</li> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID or Key</td> 
   <td>Enter or map the ID or Key of the record you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### Download an attachment

This action module *downloads a particular attachment*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Jira Software</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Jira Software</em></MadCap:conditionalText>`.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Jira Software</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Jira Software</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter or map the ID of the attachment you want to download.</td> 
  </tr> 
 </tbody> 
</table>

#### Read a record

This action module reads *data from a single record* in *Jira Software*.

You specify the

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
type and
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  type and</MadCap:conditionalText>` ID of the *record*.

The module returns any standard fields associated with the record

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
or records
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  or records</MadCap:conditionalText>`, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Jira Software</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Jira Software</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of Jira record you want the module to read.</p> 
    <ul> 
     <li>Attachment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
     <li>User</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the outputs that you want to receive. Output options are available based on the type of record selected in the "Record Type" field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td> <p>Enter or map the unique <em>Jira Software</em> ID of the <em>record</em> that you want the module to <em>read</em>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a record

This action module *updates an existing record, such as an issue or project,*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Jira Software</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Jira Software</em></MadCap:conditionalText>`.

You specify the

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
type and
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  type and</MadCap:conditionalText>` ID of the *record*.

The module returns the ID of the 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
<em>updated</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <em>updated</em></MadCap:conditionalText>` *record* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Jira Software</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Jira Software</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to update. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint </li> 
     <li>Transition issue</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID or Key</td> 
   <td>Enter or map the ID or Key of the record you want to update.</td> 
  </tr> 
 </tbody> 
</table>

### Searches

* [List records](#list) 
* [Search for records](#search)

#### List records

This search module retrieves all items of a specific type that match your search query

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses.
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses.</MadCap:conditionalText>`You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Jira Software</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Jira Software</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to list. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Comment</li> 
     <li>Issue</li> 
     <li>Project</li> 
     <li>Sprint issue</li> 
     <li>Worklog</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Max Results</p> </td> 
   <td> <p>Enter or map the maximum number of <em>record</em>s you want the module to <em>retrieve</em> during each scenario execution cycle.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Offset</td> 
   <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
  </tr> 
 </tbody> 
</table>

#### Search for records

This search module looks for *records in an object* in *Jira Software* that match the search query you specify.

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
The module
<em>returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses</em>.
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> The module  <em>returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses</em>.</MadCap:conditionalText>` You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Jira Software</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Jira Software</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Jira Software</em> account to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect Jira Cloud to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record you want the module to search for. When you select a record type, other fields specific to that record type appear in the module.</p> 
    <ul> 
     <li>Issues</li> 
     <li> <p>Issues by JQL (Jira Query Lanuguage) </p> <p>For more information on JQL, see <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQL stands for Jira Query,project managers%2C and business users.">JQL</a> at the Atlassian help site. </p> </li> 
     <li>Project</li> 
     <li>Project by issue</li> 
     <li>User</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

