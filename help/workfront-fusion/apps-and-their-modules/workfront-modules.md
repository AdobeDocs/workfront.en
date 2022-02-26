---
filename: workfront-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Workfront modules
description: You can use the Adobe Workfront connector to automate your processes within Workfront. If you have a Workfront Fusion for Work Automation and Integration license, you can also use it to connect to third-party apps and services.
---

# *Adobe Workfront* modules

You can use the *Adobe Workfront* connector to automate your processes within *Workfront*. If you have a *Workfront Fusion for Work Automation and Integration* license, you can also use it to connect to third-party apps and services.

The *Workfront* connector does not count against the number of active apps available to your organization. All scenarios, even if they use only the *Workfront* app, do count against your organization's total scenario count.

For more information on your organization's available apps and scenarios, see [Organizations](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [Adobe Workfront Fusion organizations and teams](../../workfront-fusion/organizations/organizations-and-teams.md).

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md). For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

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

## Connect *Workfront* to *Workfront Fusion*

The Workfront connector uses OAuth 2.0 to connect to *Workfront*.

You can create a connection to your *Workfront* account directly from inside a *Workfront Fusion* module.

<ol> 
 <li value="1"> <p>In any Workfront app module, click <span class="bold">Add </span>next to the Connection box.</p> </li> 
 <li value="2"> <p>Enter the name of your instance into the URL. Example: <code>https://<your instance>.my.workfront.com</code>.</p> </li> 
 <li value="3"> <p>Click <span class="bold">Next</span>.</p> </li> 
 <li value="4"> <p>Click <span class="bold">SAML log in</span> to create the connection and go back to the module.</p> <p>Or</p> <p>Enter your Username and Password, then click <span class="bold">Log in</span> to create the connection and go back to the module.</p> <note type="note"> 
   <ul> 
    <li> <p>If you do not see a SAML log in button, your organization has not enabled Single Sign-On (SSO). You can log in with your Username and Password.</p> <p>For more information on SSO, see <a href="../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Overview of single sign-on in Adobe Workfront</a></p> </li> 
    <li> <p>OAuth 2.0 connections to the Workfront API no longer rely on API keys. </p> </li> 
   </ul> 
  </note> </li> 
</ol>

## *Workfront* modules and their fields

When you configure *Workfront* modules, *Workfront Fusion* displays the fields listed below. Along with these, additional *Workfront* fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers

* [Watch Events](#watch3) 
* [Watch Record](#watch) 
* [Watch Field](#watch2)

#### Watch Events

This trigger module executes a scenario in real time when objects of a specific type are added, updated, or deleted in *Workfront*

The module returns any standard fields associated with the record

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
or records
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  or records</MadCap:conditionalText>`, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

<ol> 
 <li value="1">Click <span class="bold">Add</span> to the right of the <span class="bold">Webhook</span> box.</li> 
 <li value="2"> <p>Configure the webhook in the <span class="bold">Add a hook</span> box that displays.</p> <p>When you are configuring this module, the following fields display<draft-comment>
    <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
     , along with any other available 
     <em>Workfront</em> fields, depending on the connection and options you choose
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
    , along with any other available 
    <em>Workfront</em> fields, depending on the connection and options you choose
   </MadCap:conditionalText>.</p> 
  <table> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Webhook name</td> 
     <td>(Optional) Type a new name for the webhook</td> 
    </tr> 
    <tr> 
     <td>Connection</td> 
     <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
    </tr> 
    <tr> 
     <td>Record Type</td> 
     <td>Select the type of <em>Workfront</em> record that you want the module to <em>watch</em>.</td> 
    </tr> <draft-comment>
     <tr data-mc-conditions=""> 
      <td> <p>Events filters</p> </td> 
      <td> <p>You can set filters to watch for only records that meet criteria you select.</p> <p>For each filter, enter the field you want the filter to evaluate, the operator, and the value that you want the filter to allow. You can use more than one filter by adding AND rules.</p> <note type="note">
        You cannot edit filters in existing Workfront webhooks. To set up different filters for Workfront event subscriptions, remove the current webhook and create a new one.
       </note> <p>For more information on event filters, see <a href="#event" class="MCXref xref">Event subscription filters in the Workfront > Watch Events modules</a> in this article.</p> </td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions=""> 
     <td> <p>Events filters</p> </td> 
     <td> <p>You can set filters to watch for only records that meet criteria you select.</p> <p>For each filter, enter the field you want the filter to evaluate, the operator, and the value that you want the filter to allow. You can use more than one filter by adding AND rules.</p> <note type="note">
       You cannot edit filters in existing Workfront webhooks. To set up different filters for Workfront event subscriptions, remove the current webhook and create a new one.
      </note> <p>For more information on event filters, see <a href="#event" class="MCXref xref">Event subscription filters in the Workfront > Watch Events modules</a> in this article.</p> </td> 
    </tr> <draft-comment>
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions=""> 
     <td>Exclude events made by this connection</td> 
     <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
    </tr> 
    <tr> 
     <td>Record Origin</td> 
     <td> <p>Choose whether you want the scenario to watch <span class="bold">New Records Only</span>, <span class="bold">Updated Records Only</span>, <span class="bold">New and Updated Records</span>, or <span class="bold">Deleted Records Only</span>.</p> <note type="note">
       If you choose 
       <span class="bold">New and Updated Records</span>, the webhook creation creates 2 event subscriptions (for the same webhook address).
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

Once the webhook is created, you should be able to view the address of the endpoint that events are sent to.

For more information, see the section [Examples of Event Payloads](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) in the Workfront Help article [Event Subscription API](../../wf-api/general/event-subs-api.md).

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront trigger module](#object).

#### Watch Field

This trigger module executes a scenario when *a field that you specify is updated*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Workfront</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Workfront</em></MadCap:conditionalText>`. The module *returns both the old and the new value of the field you specify*. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Record Type</td> 
   <td> <p>Select the type of <em>Workfront</em> record that you want the module to <em>watch</em>.</p> <p>For example, select Task if you want to start executing the scenario each time a record field is updated in a task.</p> </td> 
  </tr> 
  <tr> 
   <td>Field</td> 
   <td>Select the field that you want the module to watch for updates. These fields reflect the fields that your Workfront administrator has set up for tracking.</td> 
  </tr> 
  <tr> 
   <td>Outputs</td> 
   <td>Select the information you want included in the output bundle for this module.</td> 
  </tr> 
  <tr> 
   <td>Limit</td> 
   <td> <p>Enter or map the maximum number of <em>record</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront trigger module](#object).

#### Watch Record

This trigger module executes a scenario when *objects of a specific type are added, updated, or both*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Workfront</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Workfront</em></MadCap:conditionalText>`. The module *returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses*. You can map *this information* in subsequent modules in the scenario. In the output, the module indicates whether each record is new or updated.

Records that were both added and updated in the given time period are returned as new records.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <p>Choose whether you want the scenario to watch <span class="bold">New Records Only</span>, <span class="bold">Updated Records Only</span>, or <span class="bold">New and Updated Records</span>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>(Displays after you choose a <span class="bold">Filter</span>.) Select the type of <em>Workfront</em> record that you want the module to <em>watch</em>.</p> <p>For example, if you want to start the scenario each time a new Project is created, select Project</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Optional Filter</td> 
   <td> <p>(Advanced) Type an API code string to define any additional parameters or code that will refine your criteria. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of <em>record</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront trigger module](#object).

### Actions

* [Convert object](#convert) 
* [Create a record (attaching custom forms)](#create2) 
* [Create a record (attaching custom forms)](#create2) 
* [Custom API Call](#custom) 
* [Delete Record](#delete) 
* [Download Document](#download) 
* [Misc Action](#misc) 
* [Read a Record](#read) 
* [Update Record](#update2) 
* [Upload Document](#upload)

#### Convert object

This action module makes one of the following conversions:

* Convert Issue to Project
* Convert Issue to Task
* Convert Task to Project

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Object type</td> 
    <td> <p>Select the type of object that you want to convert. This is the type that the object has before the conversion.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Object type</td> 
   <td> <p>Select the type of object that you want to convert. This is the type that the object has before the conversion.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Convert to</td> 
    <td>Select the object that you want to convert it to. This is the type that the object has after the conversion.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Convert to</td> 
   <td>Select the object that you want to convert it to. This is the type that the object has after the conversion.</td> 
  </tr> 
  <tr> 
   <td>&lt;Object&gt; ID</td> 
   <td> <p>Enter the object's ID. </p> <p>Note: When entering the ID&nbsp;of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Template ID</td> 
    <td> <p>If you are converting to a project, select the Template ID&nbsp;that you want to use for the project.</p> <p>Note: When entering the ID&nbsp;of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Template ID</td> 
   <td> <p>If you are converting to a project, select the Template ID&nbsp;that you want to use for the project.</p> <p>Note: When entering the ID&nbsp;of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Custom forms</td> 
    <td>Select any custom forms that you want to add to the newly converted object, then enter values for the custom form's fields.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Custom forms</td> 
   <td>Select any custom forms that you want to add to the newly converted object, then enter values for the custom form's fields.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Options</td> 
    <td> <p>Enable any options you want when converting the object. Options are available depending on which object you are converting to or from.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Options</td> 
   <td> <p>Enable any options you want when converting the object. Options are available depending on which object you are converting to or from.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a record (attaching custom forms)

This action module creates an object, such as a project, task, or issue in *Workfront*, and allows you to add a custom form to the new object. The module allows you to select which of the object's fields are available in the module.

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
<em>new</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <em>new</em></MadCap:conditionalText>` *record* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

You could use this module, for example, to create a task in *Workfront* when a client adds a new row in a Google Sheets list of tasks that need to be done.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

Make sure you provide the minimum number of input fields. For example, if you want to create an issue, you need to provide a valid parent project ID in the Project ID field to indicate where the issue should live in *Workfront*. You can use the mapping panel to map this information from another module in your scenario, or you can enter it manually by typing in the name and then selecting it from the list.

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Record Type</td> 
   <td> <p>Select the type of <em>Workfront</em> record that you want the module to <em>create</em>.</p> <p>For example, if you want to <em>create</em> a Project, select Project from the dropdown list and then make sure that you have access to data (from previous modules in the scenario) that will populate the project.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Select fields to map</td> 
    <td> <p>Select the fields that you want available for data input. This allows you to use these fields without having to scroll through the ones you don't need.</p> <p>For fields in custom forms, use the <b>Attach Custom Form</b> field.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Select fields to map</td> 
   <td> <p>Select the fields that you want available for data input. This allows you to use these fields without having to scroll through the ones you don't need.</p> <p>For fields in custom forms, use the <b>Attach Custom Form</b> field.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Attach Custom Form</td> 
    <td>Select any custom forms that you want to add to the new object, then enter values for those fields.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Attach Custom Form</td> 
   <td>Select any custom forms that you want to add to the new object, then enter values for those fields.</td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront action module](#object2).

>[!NOTE]
>
>* When entering the ID&nbsp;of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.
>* When entering the text for a custom field or a Note object (Comment or reply), you can use HTML tags in the Note Text field to create rich text, such as bold or italic text.
>
>  For more information on rich text in updates, see [Add an update to a work item](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

#### Create Record

This action module creates an object, such as a project, task, or issue in *Workfront*. The module allows you to select which of the object's fields are available in the module.

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
<em>new</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <em>new</em></MadCap:conditionalText>` *record* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

You could use this module, for example, to create a task in *Workfront* when a client adds a new row in a Google Sheets list of tasks that need to be done.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

Make sure you provide the minimum number of input fields. For example, if you want to create an issue, you need to provide a valid parent project ID in the Project ID field to indicate where the issue should live in *Workfront*. You can use the mapping panel to map this information from another module in your scenario, or you can enter it manually by typing in the name and then selecting it from the list.

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Record Type</td> 
   <td> <p>Select the type of <em>Workfront</em> record that you want the module to <em>create</em>.</p> <p>For example, if you want to <em>create</em> a Project, select Project from the dropdown list and then make sure that you have access to data (from previous modules in the scenario) that will populate the project.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Select fields to map</td> 
    <td>Select the fields that you want available for data input. This allows you to use these fields without having to scroll through the ones you don't need.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Select fields to map</td> 
   <td>Select the fields that you want available for data input. This allows you to use these fields without having to scroll through the ones you don't need.</td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront action module](#object2).

>[!NOTE]
>
>* When entering the ID&nbsp;of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.
>* When entering the text for a custom field or a Note object (Comment or reply), you can use HTML tags in the Note Text field to create rich text, such as bold or italic text.
>
>  For more information on rich text in updates, see [Add an update to a work item](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

#### Custom API Call

This action module lets you make a custom authenticated call to the *Workfront* API

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
without having to think through authentication
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  without having to think through authentication</MadCap:conditionalText>`. This way, you can create a data flow automation that can't be accomplished by the other *Workfront* modules.

The module returns the following information:

* `Status Code`(number): This indicates the success or failure of your HTTP request. These are standard codes that you can look up on the internet.
* `Headers`(object): A more detailed context for the response/status code that doesn’t relate to the output body. Not all headers that appear in a response header are response headers, so some might not be useful to you.

  The response headers depend on the HTTP request you chose when configuring the module.

* `Body`(object): Depending on the HTTP request you chose when configuring the module, you may receive some data back. That data, such as the data from a GET request, is contained in this object.

You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Enter a path relative to<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API Version</td> 
   <td>Select the version of the Workfront API that you want the module to use.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object. This determines the content type of the request.</p> <p>For example,<code> {“Content-type”:“application/json”}</code></p> <p>Note: If you’re getting errors and it's difficult to determine their origin, consider modifying headers based on the Workfront documentation. If your Custom API Call returns a 422 HTTP Request Error, try using a “Content-Type”:“text/plain” header.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> <p>Tip: We recommend that you send information through the JSON body rather than as query parameters.</p> </td> 
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

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront action module](#object2).

#### Delete Record

This action module deletes an object, such as a project, task, or issue in *Workfront*.

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
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Force delete</td> 
   <td>Enable this option to ensure that the record is deleted, even if the Workfront UI would request confirmation of the deletion.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>ID</td> 
    <td> <p>Enter the unique <em>Workfront</em> ID of the <em>record</em> that you want the module to delete.</p> <p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Enter the unique <em>Workfront</em> ID of the <em>record</em> that you want the module to delete.</p> <p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>Record Type</td> 
   <td>Select the type of <em>Workfront</em> record that you want the module to <em>delete</em>.<draft-comment>
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this right?&nbsp;Or or you deleting a record FROM&nbsp;this record type, as it says in the legacy wf fusion wf article?</span>
    </draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this right?&nbsp;Or or you deleting a record FROM&nbsp;this record type, as it says in the legacy wf fusion wf article?</span></td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront action module](#object2).

#### Download Document

This action module downloads a document from *Workfront*.

You specify the

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
type and
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  type and</MadCap:conditionalText>` ID of the *record*.

The module returns the document's content, filename, file extension, and file size. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Document ID</td> 
   <td> <p>Map or manually enter the unique <em>Workfront</em> ID of the document that you want the module to download.</p> <p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront action module](#object2).

#### Misc Action

This action module lets you perform actions against the API.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Record Type</td> 
    <td> <p>Select the type of <em>Workfront</em> record that you want the module to <em>interact with</em>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Record Type</td> 
   <td> <p>Select the type of <em>Workfront</em> record that you want the module to <em>interact with</em>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>ID</td> 
    <td>Enter or map the unique <em>Workfront</em> ID of the <em>record</em> that you want the module to <em>interact with</em>.<draft-comment>
      <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span>
     </draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span><p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td>Enter or map the unique <em>Workfront</em> ID of the <em>record</em> that you want the module to <em>interact with</em>.<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Is this correct?</span><p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Action</td> 
    <td> <p>Select the action you want the module to perform.</p> <p>You may need to fill out additional fields, depending on the Record Type and Action you choose. Some combinations of these two settings may require only a record ID, while others (such as Project for the <span class="bold">Record Type</span> and Attach Template for the <span class="bold">Action</span>) require additional information (such as an Object ID and a Template ID).<draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        <span style="color: #ff1493;"> Is this paragraph correct? I got it from the </span>
        <a href="https://docs.google.com/document/d/1dWaLFHHq8D6iq2nbRd8k3cT2GyyPv_mI-sdWKoCe--o/edit" style="color: #ff1493;">requirements doc</a>
        <span style="color: #ff1493;">, #2</span>
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       <span style="color: #ff1493;"> Is this paragraph correct? I got it from the </span>
       <a href="https://docs.google.com/document/d/1dWaLFHHq8D6iq2nbRd8k3cT2GyyPv_mI-sdWKoCe--o/edit" style="color: #ff1493;">requirements doc</a>
       <span style="color: #ff1493;">, #2</span>
      </MadCap:conditionalText></p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Action</td> 
   <td> <p>Select the action you want the module to perform.</p> <p>You may need to fill out additional fields, depending on the Record Type and Action you choose. Some combinations of these two settings may require only a record ID, while others (such as Project for the <span class="bold">Record Type</span> and Attach Template for the <span class="bold">Action</span>) require additional information (such as an Object ID and a Template ID).<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      <span style="color: #ff1493;"> Is this paragraph correct? I got it from the </span>
      <a href="https://docs.google.com/document/d/1dWaLFHHq8D6iq2nbRd8k3cT2GyyPv_mI-sdWKoCe--o/edit" style="color: #ff1493;">requirements doc</a>
      <span style="color: #ff1493;">, #2</span>
     </MadCap:conditionalText></p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront action module](#object2).

#### Read a Record

This action module *retrieves data from a single record*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Workfront</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Workfront</em></MadCap:conditionalText>`.

You specify the

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
type and
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  type and</MadCap:conditionalText>` ID of the *record*. You can also specify which related records you want the module to read.

For example, if the record that the module is reading is a project, you can specify that you want the project's tasks read.

The module returns an array of data from the standard fields for the output you specified.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> <draft-comment>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td>
   </draft-comment>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> <draft-comment>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Record Type</td>
   </draft-comment>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Record Type</td> 
   <td>Choose the <em>Workfront</em> object type that you want the module to read.</td> 
  </tr> 
  <tr> <draft-comment>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   </draft-comment>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> <draft-comment>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">References</td>
   </draft-comment>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">References</td> 
   <td>Select any reference fields that you want to include in the output.</td> 
  </tr> 
  <tr> <draft-comment>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Collections</td>
   </draft-comment>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Collections</td> 
   <td>Select any reference fields that you want to include in the output.</td> 
  </tr> 
  <tr> <draft-comment>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">ID</td>
   </draft-comment>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">ID</td> 
   <td> <p>Enter the unique <em>Workfront</em> ID of the <em>record</em> that you want the module to read.</p> <p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront action module](#object2).

#### Update Record

This action module updates an object, such as a project, task, or issue. The module allows you to select which of the object's fields are available in the module.

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

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <em>updated</em></MadCap:conditionalText>` *object* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>ID</td> 
    <td> <p>Enter the unique <em>Workfront</em> ID of the <em>record</em> that you want the module to update.</p> <p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Enter the unique <em>Workfront</em> ID of the <em>record</em> that you want the module to update.</p> <p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>Record Type</td> 
   <td> <p>Select the type of <em>Workfront</em> record that you want the module to <em>update</em>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Select fields to map</td> 
    <td>Select the fields that you want available for data input. This allows you to use these fields without having to scroll through the ones you don't need.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Select fields to map</td> 
   <td>Select the fields that you want available for data input. This allows you to use these fields without having to scroll through the ones you don't need.</td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront action module](#object2).

>[!NOTE]
>
>* When entering the ID&nbsp;of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.
>* When entering the text for a custom field or a Note object (Comment or reply), you can use HTML tags in the Note Text field to create rich text, such as bold or italic text.
>
>  For more information on rich text in updates, see [Add an update to a work item](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

#### Upload Document

This action module uploads a document to a *Workfront* object, such as a project, task, or issue.

You specify the location for the document, the file you want to upload, and an optional new name for the file.

The module returns the ID of the 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
<em>uploaded</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <em>uploaded</em></MadCap:conditionalText>` *document* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Related Record ID</td> 
    <td>Enter the unique <em>Workfront</em> ID of the record to which you want to upload the document.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Related Record ID</td> 
   <td>Enter the unique <em>Workfront</em> ID of the record to which you want to upload the document.</td> 
  </tr> 
  <tr> 
   <td>Related Record Type</td> 
   <td>Select the type of <em>Workfront</em> record where you want the module to <em>upload the document</em>.</td> 
  </tr> 
  <tr> 
   <td>Source file</td> 
   <td> <p>Map the file you want to upload from the previous module (for example, the HTTP &gt; Get a File or Dropbox &gt; Get a file module). Or enter the file name and file data manually.</p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront action module](#object2).

### Searches

* [Read Related Records](#read2) 
* [Search](#search2)

#### Read Related Records

This search module reads records that match the search query you specify, in a particular parent object.

You specify which fields you want included in the output. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Record Type</td> 
    <td> <p>Select the type of the parent record (<em>Workfront</em> object) whose associated records you want to read.</p> <p>See a list of the <em>Workfront</em> objects types for which you can use this module in <a href="#object3" class="MCXref xref">Object types available for each Workfront search module</a> in this article.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Record Type</td> 
   <td> <p>Select the type of the parent record (<em>Workfront</em> object) whose associated records you want to read.</p> <p>See a list of the <em>Workfront</em> objects types for which you can use this module in <a href="#object3" class="MCXref xref">Object types available for each Workfront search module</a> in this article.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Parent Record ID</td> 
    <td> <p>Enter or map the ID of the parent record whose associated records you want to read.</p> <p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Parent Record ID</td> 
   <td> <p>Enter or map the ID of the parent record whose associated records you want to read.</p> <p>To get the ID, open the <em>Workfront</em> object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Collections</td> 
    <td>Select or map the type of child record that you want the module to read.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Collections</td> 
   <td>Select or map the type of child record that you want the module to read.</td> 
  </tr> 
  <tr> 
   <td>Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search

This search module looks for *records in an object* in *Workfront* that match the search query you specify.

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
<em>Workfront</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Workfront</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection</td> 
   <td> <p>For instructions about connecting your <em>Workfront</em> app to <em>Workfront Fusion</em>, see <a href="#connect" class="MCXref xref">Connect Workfront to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Record Type</td> 
   <td> <p>Select the type of <em>Workfront</em> record that you want the module to <em>search for</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>Result Set</td> 
   <td>Select an option to specify whether you want the module to get the first result that matches your search criteria or all the results that match it.</td> 
  </tr> 
  <tr> 
   <td>Maximal</td> 
   <td> <p>Enter or map the maximum number of <em>record</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td>Search criteria</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to <em>Workfront</em> logs the user into <em>Workfront</em>, and the search will not be successful.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Outputs</td> 
    <td> <p>Select the fields that you want to include in the output for this module.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Outputs</td> 
   <td> <p>Select the fields that you want to include in the output for this module.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>References</td> 
    <td>Select any reference fields that you want to include in the search.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>References</td> 
   <td>Select any reference fields that you want to include in the search.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Collections</td> 
    <td>Select any collections that you want to add to the search.</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Collections</td> 
   <td>Select any collections that you want to add to the search.</td> 
  </tr> 
 </tbody> 
</table>

See a list of the *Workfront* objects types for which you can use this module in [Object types available for each Workfront search module](#object3).

## *Workfront* object types available for each *Workfront* module

* [Object types available for each Workfront trigger module](#object) 
* [Object types available for each Workfront action module](#object2) 
* [Object types available for each Workfront search module](#object3)

### Object types available for each *Workfront* trigger module

| &nbsp; |Watch Record |Watch Field |Watch Events |
|---|---|---|---|
| Approval Process |&nbsp; |✓ |&nbsp; |
| Assignment |&nbsp; |✓ |✓ |
| Baseline |✓ |&nbsp; |&nbsp; |
| Billing Record |✓ |&nbsp; |&nbsp; |
| Billing Record |✓ |&nbsp; |&nbsp; |
| Billing Rate |&nbsp; |✓ |&nbsp; |
| Company |✓ |✓ |✓ |
| Dashboard |&nbsp; |&nbsp; |✓ |
| Document |✓ |✓ |✓ |
| Document Folder |✓ |✓ |&nbsp; |
| Document Request |✓ |&nbsp; |&nbsp; |
| Document Version |✓ |✓ |&nbsp; |
| Expense |✓ |✓ |✓ |
| Expense Type |&nbsp; |&nbsp; |&nbsp; |
| Group |✓ |✓ |&nbsp; |
| Hour |&nbsp; |✓ |✓ |
| Hour Type |&nbsp; |✓ |&nbsp; |
| Issue |✓ |✓ |✓ |
| Iteration |✓ |✓ |&nbsp; |
| Job Role |✓ |✓ |&nbsp; |
| Journal Entry |✓ |&nbsp; |&nbsp; |
| Milestone |&nbsp; |✓ |&nbsp; |
| Milestone Path |✓ |✓ |&nbsp; |
| Note |✓ |✓ |✓ |
| Note Tag |&nbsp; |✓ |&nbsp; |
| Portfolio |✓ |✓ |✓ |
| Program |✓ |✓ |✓ |
| Project |✓ |✓ |✓ |
| Project User |&nbsp; |✓ |&nbsp; |
| Reserved Time&#42;  |&nbsp; |✓ |&nbsp; |
| Report |&nbsp; |&nbsp; |✓ |
| Risk |&nbsp; |&nbsp; |&nbsp; |
| Risk Type |&nbsp; |&nbsp; |&nbsp; |
| Step Approver |&nbsp; |✓ |&nbsp; |
| Task |✓ |✓ |✓ |
| Team |&nbsp; |✓ |&nbsp; |
| Template |✓ |✓ |✓ |
| Template Task |✓ |✓ |&nbsp; |
| Timesheet |✓ |✓ |✓ |
| User |✓ |✓ |✓ |
| Update |&nbsp; |&nbsp; |&nbsp; |

### Object types available for each *Workfront* action module

>[!NOTE]
>
>The Download Document module is not included in this table because *Workfront* object types are not part of its configuration.

<table> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>&nbsp;</th> 
   <th>Create a record</th> 
   <th>Update a record</th> 
   <th>Delete a record</th> 
   <th>Upload Document</th> 
   <th>Read a record</th> 
   <th>Custom API Call</th> 
   <th>Misc Action</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Approval Process</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Assignment</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td>Billing Record</td> 
    <td>✓</td> 
    <td>✓</td> 
    <td>✓</td> 
    <td>&nbsp;</td> 
    <td>✓</td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td>Billing Record</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Billing Rate</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Company</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document Folder</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document Version</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Expense</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Expense Type</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Group</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hour</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Hour Type</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Issue</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteration</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Job Role</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Journal Entry</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Milestone</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Milestone Path</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Note</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Note Tag</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Project User</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Reserved Time* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Risk</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Risk Type</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Step Approver</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Task</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Template</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Template Task</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Timesheet</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Update</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
 </tbody> 
</table>

### Object types available for each *Workfront* search module

| &nbsp; |Search |Read Related Records |
|---|---|---|
| Approval Process |✓ |✓ |
| Assignment |✓ |✓ |
| Billing Record |✓ |&nbsp; |
| Billing Record |✓ |&nbsp; |
| Billing Rate |✓ |&nbsp; |
| Company |✓ |✓ |
| Document |✓ |✓ |
| Document Folder |✓ |✓ |
| Document Version |✓ |&nbsp; |
| Expense |✓ |&nbsp; |
| Expense Type |✓ |&nbsp; |
| Group |✓ |✓ |
| Hour |✓ |&nbsp; |
| Hour Type |✓ |&nbsp; |
| Issue |✓ |✓ |
| Iteration |✓ |&nbsp; |
| Job Role |✓ |&nbsp; |
| Journal Entry |✓ |&nbsp; |
| Milestone |✓ |&nbsp; |
| Milestone Path |✓ |&nbsp; |
| Note |✓ |&nbsp; |
| Note Tag |✓ |&nbsp; |
| Portfolio |✓ |✓ |
| Program |✓ |&nbsp; |
| Project |✓ |✓ |
| Project User |✓ |&nbsp; |
| Reserved Time&#42;  |✓ |&nbsp; |
| Risk |✓ |&nbsp; |
| Risk Type |✓ |&nbsp; |
| Step Approver |✓ |&nbsp; |
| Task |✓ |✓ |
| Team |✓ |&nbsp; |
| Template |✓ |&nbsp; |
| Template Task |✓ |&nbsp; |
| Timesheet |✓ |✓ |
| User |✓ |✓ |
| User Delegation |✓ |&nbsp; |

&#42; We recommend that you double check to ensure this works the way you would expect it to.

## Event subscription filters in the Workfront > Watch Events modules

>[!NOTE]
>
>We highly recommend using event subscription filters in your Watch Events modules.

The *Workfront* Watch Events module triggers scenarios based on a webhook that creates an event subscription in the *Workfront* API. The event subscription is a set of data that determines which events are sent to the webhook. For example, if you set up a Watch Events module that is watching for issues, then the event subscription sends only events related to issues.

By using event subscription filters, Fusion users can create event subscriptions that are a better fit for their use cases. For example, you can set up an event subscription in the *Workfront* API to send only issues that are in a specific project to the webhook, ensuring that the Watch Events module will only trigger for issues in that project. The ability to create narrower triggers improves scenario design by reducing the number of irrelevant triggers.

This is different from setting up a filter in the Workfront Fusion scenario. Without an event subscription filter, your webhook receives all events related to the object type you select. Most of these events would be irrelevant to the scenario, and must be filtered out before the scenario can continue.

>[!NOTE]
>
>You cannot edit filters in existing Workfront webhooks. To set up different filters for Workfront event subscriptions, remove the current webhook and create a new one.

` `**Example: **`` Consider a scenario that processes new issues that are assigned to a specific user, Ana.

### Filter events by using an event subscription filter (recommended)

Using the event filter, you can set up the webhook to trigger the scenario when an issue is assigned to Ana when the issue is created. Ana has the userID b378489d8f7cd3cee0539260720a84b7.

![](assets/event-filter-watch-events-350x277.png)

If 100 issues are created in a day, but only two of them are assigned to Ana, the scenario would execute twice.

### Filter events inside the scenario (not recommended)

To filter events so that only issues assigned to Ana are processed, you could create a filter after the Watch Events module.

![](assets/watch-events-non-event-filter-350x206.png)

If 100 issues are created in a day, but only two of them are assigned to Ana, the scenario would execute 100 times. 98 of the executions would stop at the filter, but the trigger module is still consuming data and performing operations in all of the executions.
For more information on event subscriptions, see [FAQs - Event Subscriptions](../../wf-api/general/event-subs-faq.md).

For more information on webhooks, see [Instant triggers (webhooks)](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

For more information on filters in scenarios, see [Add a filter to a scenario](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
