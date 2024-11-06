---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Workfront modules
description: You can use the Adobe Workfront Fusion Adobe Workfront connector to automate your processes within Workfront. If you have a Workfront Fusion for Work Automation and Integration license, you can also use it to connect to third-party apps and services.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
---
# [!DNL Adobe Workfront] modules

You can use the [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] connector to automate your processes within [!DNL Workfront]. If you have a [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] license, you can also use it to connect to third-party apps and services.

The [!DNL Workfront] connector does not count against the number of active apps available to your organization. All scenarios, even if they use only the [!DNL Workfront] app, do count against your organization's total scenario count.

For more information on your organization's available apps and scenarios, see [Organizations](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] organizations and teams](../../workfront-fusion/organizations/organizations-and-teams.md).

If you need instructions on creating a scenario, see [Create a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] or higher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>


To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Workfront] to [!DNL Workfront Fusion] 

The [!DNL Workfront] connector uses OAuth 2.0 to connect to [!DNL Workfront].

You can create a connection to your [!DNL Workfront] account directly from inside a [!DNL Workfront Fusion] module.

1. In any Adobe Workfront module, click **Add** next to the Connection field.
1. Fill in the following fields:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Enter a name for the new connection.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>
          <p>Select whether are connecting to a production or non-production environment.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>Select whether you are connecting to a service account or a personal account.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Enter your [!DNL Workfront] Client ID. This can be found in the OAuth2 Applications area of the Setup area in Workfront. Open the specific application you are connecting to to see the Client ID.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Enter your [!DNL Workfront] Client ID. This can be found in the OAuth2 Applications area of the Setup area in Workfront. Open the specific application you are connecting to to see the Client ID.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentication URL]</td>
        <td>This can remain the default value, or you can enter the URL of your Workfront instance, followed by <code>/integrations/oauth2</code>. <p>Example: <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Host prefix]</td>
        <td>In most cases, this value should be <code>origin</code>.
      </tr>
    </tbody>
    </table>

1. Click **[!UICONTROL Continue]** to save the connection and return to the module.




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

   >[!NOTE]
   >
   >* If you do not see a SAML log in button, your organization has not enabled Single Sign-On (SSO). You can log in with your Username and Password.
   >   
   >   For more information on SSO, see [Overview of single sign-on in [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
   >   
   >* OAuth 2.0 connections to the [!DNL Workfront] API no longer rely on API keys. 
   >* To create a connection to a Workfront Sandbox environment, you must create an OAuth2 application in that environment, and then use the Client ID and Client Secret generated by that application in your connection. 
   >
   >   For instructions on creating an OAuth2 application in Workfront, see [Create an OAuth2 application using user credentials (Authorization code flow)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) in the article Create OAuth2 applications for Workfront integrations.

## [!DNL Workfront] modules and their fields

When you configure [!DNL Workfront] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Workfront] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).


![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>* If you do not see the most up-to-date fields in a Workfront module, this may be because of caching issues. Wait one hour and try again.
>* HTTP 429 status codes from Adobe Workfront should not cause deactivations, but instead trigger a short execution pause in the scenario.

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers 

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Watch Events]**

This trigger module executes a scenario in real time when objects of a specific type are added, updated, or deleted in Workfront

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Type]</td> 
      <td>Select the type of [!DNL Workfront] record that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Select whether you want to watch the old state or the new state.<ul><li><p><b>[!UICONTROL New state]</b></p><p>Trigger a scenario when the record changes <b>to</b> a given value.</p><p>For example, if the state is set to [!UICONTROL New State] and the filter is set to [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress], the webhook triggers a scenario when the [!UICONTROL Status] changes to [!UICONTROL In Progress], regardless of what the status was before. </p></li><li><p><b>[!UICONTROL Old state]</b></p><p>Trigger a scenario when the record changes <b>from</b> a given value.</p><p>For example, if the state is set to [!UICONTROL Old State] and the filter is set to [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress], the webhook triggers a scenario when a [!UICONTROL Status] that is currently [!UICONTROL In Progress] changes to another status. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>You can set filters to watch for only records that meet criteria you select.</p> <p>For each filter, enter the field you want the filter to evaluate, the operator, and the value that you want the filter to allow. You can use more than one filter by adding AND rules.</p> <p>Note: You cannot edit filters in existing [!DNL Workfront] webhooks. To set up different filters for [!DNL Workfront] event subscriptions, remove the current webhook and create a new one.</p> <p>For more information on event filters, see <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Event subscription filters in the [!DNL Workfront] &gt; [!UICONTROL Watch Events] modules</a> in this article.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.<p><b>NOTE</b>The Assignment record type does not include this option.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Origin]</td> 
      <td> <p>Choose whether you want the scenario to watch <strong>[!UICONTROL New Records Only]</strong>, <strong>[!UICONTROL Updated Records Only]</strong>, <strong>[!UICONTROL New and Updated Records]</strong>, or <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Note: If you choose <strong>[!UICONTROL New and Updated Records]</strong>, the webhook creation creates 2 event subscriptions (for the same webhook address).</p> </td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

For more information, see the section [Examples of Event Payloads](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) in the [!DNL Workfront] Help article [Event Subscription API](../../wf-api/general/event-subs-api.md).

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Watch Field]**

This trigger module executes a scenario when a field that you specify is updated. The module returns both the old and the new value of the field you specify. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to watch.</p> <p>For example, select [!UICONTROL Task] if you want to start executing the scenario each time a record field is updated in a task.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Select the field that you want the module to watch for updates. These fields reflect the fields that your [!DNL Workfront] administrator has set up for tracking.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td>Select the information you want included in the output bundle for this module.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Watch Record]**

This trigger module executes a scenario when objects of a specific type are added, updated, or both. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario. In the output, the module indicates whether each record is new or updated.

Records that were both added and updated in the given time period are returned as new records.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Choose whether you want the scenario to watch <strong>[!UICONTROL New Records Only]</strong>, <strong>[!UICONTROL Updated Records Only]</strong>, or <strong>[!UICONTROL New and Updated Records]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>(Displays after you choose a <strong>Filter</strong>.) Select the type of [!DNL Workfront] record that you want the module to watch.</p> <p>For example, if you want to start the scenario each time a new Project is created, select [!UICONTROL Project]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optional Filter]</td> 
   <td> <p>(Advanced) Type an API code string to define any additional parameters or code that will refine your criteria. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++


### Actions

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL Convert object]**

This action module makes one of the following conversions:

* Convert Issue to Project
* Convert Issue to Task
* Convert Task to Project

>[!NOTE]
>
>As of July 2024, custom forms can be included when converting an object.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Object type]</td> 
   <td> <p>Select the type of object that you want to convert. This is the type that the object has before the conversion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Convert to]</td> 
   <td>Select the object that you want to convert it to. This is the type that the object has after the conversion.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;Object&gt; ID]</td> 
   <td> <p>Enter the object's ID. </p> <p>Note: When entering the ID of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Template ID]</td> 
   <td> <p>If you are converting to a project, select the Template ID that you want to use for the project.</p> <p>Note: When entering the ID of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom forms]</td> 
   <td>Select any custom forms that you want to add to the newly converted object, then enter values for the custom form's fields.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Options]</td> 
   <td> <p>Enable any options you want when converting the object. Options are available depending on which object you are converting to or from.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copy native fields]</td> 
   <td> <p>Enable this option to copy any native fields from the original object to the new object.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copy custom forms]</td> 
   <td> <p>Enable this option to copy any native fields from the original object to the new object.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a record (attaching custom forms)]** 

This action module creates an object, such as a project, task, or issue in [!DNL Workfront], and allows you to add a custom form to the new object. The module allows you to select which of the object's fields are available in the module.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

You could use this module, for example, to create a task in [!DNL Workfront] when a client adds a new row in a [!DNL Google Sheets] list of tasks that need to be done.

When you are configuring this module, the following fields display.

Make sure you provide the minimum number of input fields. For example, if you want to create an issue, you need to provide a valid parent project ID in the Project ID field to indicate where the issue should live in Workfront. You can use the mapping panel to map this information from another module in your scenario, or you can enter it manually by typing in the name and then selecting it from the list.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to create.</p> <p>For example, if you want to create a Project, select [!UICONTROL Project] from the dropdown list and then make sure that you have access to data (from previous modules in the scenario) that will populate the project.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Select the fields that you want available for data input. This allows you to use these fields without having to scroll through the ones you don't need.</p> <p>For fields in custom forms, use the <b>[!UICONTROL Attach Custom Form]</b> field.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Attach Custom Form]</td> 
   <td>Select any custom forms that you want to add to the new object, then enter values for those fields.</td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* When entering the ID of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.
>* When entering the text for a custom field or a [!UICONTROL Note] object (Comment or reply), you can use HTML tags in the [!UICONTROL Note Text] field to create rich text, such as bold or italic text.
>
>  For more information on rich text in updates, see [Add an update to a work item](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Create Record]**

This action module creates an object, such as a project, task, or issue in Workfront. The module allows you to select which of the object's fields are available in the module.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

You could use this module, for example, to create a task in [!DNL Workfront] when a client adds a new row in a Google Sheets list of tasks that need to be done.

When you are configuring this module, the following fields display.

Make sure you provide the minimum number of input fields. For example, if you want to create an issue, you need to provide a valid parent project ID in the Project ID field to indicate where the issue should live in Workfront. You can use the mapping panel to map this information from another module in your scenario, or you can enter it manually by typing in the name and then selecting it from the list.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to create.</p> <p>For example, if you want to create a Project, select [!UICONTROL Project] from the dropdown list and then make sure that you have access to data (from previous modules in the scenario) that will populate the project.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td>Select the fields that you want available for data input. This allows you to use these fields without having to scroll through the ones you don't need.</td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* When entering the ID of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.
>* When entering the text for a custom field or a [!UICONTROL Note] object (Comment or reply), you can use HTML tags in the [!UICONTROL Note Text] field to create rich text, such as bold or italic text.
>
>  For more information on rich text in updates, see [Add an update to a work item](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Custom API Call]**

This action module lets you make a custom authenticated call to the [!DNL Workfront] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL Workfront] modules.

The module returns the following information:

* **[!UICONTROL Status Code]** (number): This indicates the success or failure of your HTTP request. These are standard codes that you can look up on the internet.
* **[!UICONTROL Headers]** (object): A more detailed context for the response/status code that doesn't relate to the output body. Not all headers that appear in a response header are response headers, so some might not be useful to you.

  The response headers depend on the HTTP request you chose when configuring the module.

* **[!UICONTROL Body]** (object): Depending on the HTTP request you chose when configuring the module, you may receive some data back. That data, such as the data from a GET request, is contained in this object.

You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Enter a path relative to<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Select the version of the [!DNL Workfront] API that you want the module to use.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object. This determines the content type of the request.</p> <p>For example,<code> {"Content-type":"application/json"}</code></p> <p>Note: If you're getting errors and it's difficult to determine their origin, consider modifying headers based on the [!DNL Workfront] documentation. If your Custom API Call returns a 422 HTTP Request Error, try using a <code>"Content-Type":"text/plain"</code> header.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> <p>Tip: We recommend that you send information through the JSON body rather than as query parameters.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Delete Record]**

This action module deletes an object, such as a project, task, or issue in Workfront.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Force delete]</td> 
   <td>Enable this option to ensure that the record is deleted, even if the [!DNL Workfront] UI would request confirmation of the deletion.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Enter the unique [!DNL Workfront] ID of the record that you want the module to delete.</p> <p>To get the ID, open the [!DNL Workfront] object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Select the type of [!DNL Workfront] record that you want the module to delete.</td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>We recommend the following scenario configuration to avoid the possibility of records not being deleted due to asynchronous operations.
>
>1. Delete the record synchronously.
>1. Add error handling to the Delete Record module to Ignore the error caused by the 40 second timeout. 


+++

+++ **[!UICONTROL Download Document]**

This action module downloads a document from Workfront.

You specify the ID of the record.

The module returns the document's content, filename, file extension, and file size. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document ID]</td> 
   <td> <p>Map or manually enter the unique [!DNL Workfront] ID of the document that you want the module to download.</p> <p>To get the ID, open the [!DNL Workfront] object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Misc Action]**

This action module lets you perform actions against the API.

>[!NOTE]
>
>As of July 2024, the `convertToProject` action includes the field `copyCategories`. When set to `TRUE`, any custom forms will be included in the project that the issue is converted to.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to interact with.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>Select the action you want the module to perform.</p> <p>You may need to fill out additional fields, depending on the [!UICONTROL Record Type] and [!UICONTROL Action] you choose. Some combinations of these two settings may require only a record ID, while others (such as Project for the <strong>[!UICONTROL Record Type]</strong> and [!UICONTROL Attach Template] for the <strong>[!UICONTROL Action]</strong>) require additional information (such as an Object ID and a Template ID).</p><p>For options available to some actions, see <a href="#misc-action-options" class="MCXref xref">Misc action options</a> in this article.</p> <p>For details about individual fields, see the <a href="http://developer.workfront.com/">Workfront developer documentation</a>. <p><strong>Note</strong>: The developer documentation site includes information only through API version 14, but still contains valuable information for API calls. </p> 
    <ol> 
     <li value="1"> <p>Select the record type from the left navigation on the [!DNL Workfront] developer documentation page. The following types have their own pages:</p> 
      <ul> 
       <li> <p>[!UICONTROL Projects]</p> </li> 
       <li> <p>[!UICONTROL Tasks]</p> </li> 
       <li> <p>[!UICONTROL Issues]</p> </li> 
       <li> <p>[!UICONTROL Users]</p> </li> 
       <li> <p>[!UICONTROL Documents]</p> </li> 
      </ul> <p>For all other record types, select <b>[!UICONTROL Other objects and endpoints]</b>, and locate the record type on the alphabetically sorted pages.</p> </li> 
     <li value="2"> <p>On the page of the appropriate record type, search (Ctrl-F or Cmd-F) for the action.</p> </li> 
     <li value="3"> <p>View descriptions for available fields under the selected action.</p> </li> 
    </ol> <p>Note:  <p>When creating a proof through the [!DNL Workfront] [!UICONTROL Misc Action] module, best practice is to create a proof without any advanced options, then update the proof using the [!DNL Workfront Proof] SOAP API.</p> <p>For more information on creating a proof with the [!DNL Workfront] API (which this module uses), see <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Add advanced proofing options when creating a proof through the [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Enter or map the unique [!DNL Workfront] ID of the record that you want the module to interact with.<p>To get the ID, open the [!DNL Workfront] object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

#### Misc action options

##### Task

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Action</th> 
   <th>Options</th> 
  </tr> 
  <tr> 
   <td>Copy</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearConstraints</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Clears financial data</p></li>
   <li>clearPermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>Clears reminder notifications</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Move</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearDocuments</li>
   <li>clearConstraints</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Clears financial data</p></li>
   <li>clearPermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>Clears reminder notifications</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

##### Issue

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Action</th> 
   <th>Options</th> 
  </tr> 
  <tr> 
   <td>Copy</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearPermissions</li>
   <li>clearProgress</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Convert to task</td> 
   <td>
   <ul>
   <li>preserveIssue<p>Keep the original issue and tie its resolution to this task</p></li>
   <li>preservePrimaryContact<p>Allow the issues's primary contact access to this task</p></li>
   <li>preserveCompletionDate<p>Keep the Planned Completion Date of the issue</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Convert to project</td> 
   <td>
   <ul>
   <li>preserveIssue<p>Keep the original issue and tie its resolution to this task</p></li>
   <li>preservePrimaryContact<p>Allow the issues's primary contact access to this task</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



##### Project

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Action</th> 
   <th>Options</th> 
  </tr> 
  <tr> 
   <td>Copy</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Clears financial data</p></li>
   <li>clearPermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>Clears reminder notifications</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Attach template / Save as template</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearBillingRates</li>
   <li>clearConstraints</li>
   <li>clearDeliverables<p>Clears goals</p></li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Clears financial data</p></li>
   <li>clearHourTypes</li>
   <li>clearIssueSetup<p>Clears queue propterties and issues setup</p></li>
   <li>clearPredecessors</li>
   <li>clearRisks</li>
   <li>clearSharingOptions</li>
   <li>clearTimedNotifications<p>Clears reminder notifications</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



+++

+++ **[!UICONTROL Read a Record]**

This action module retrieves data from a single record.

You specify the ID of the record. You can also specify which related records you want the module to read.

For example, if the record that the module is reading is a project, you can specify that you want the project's tasks read.

The module returns an array of data from the standard fields for the output you specified.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>
  
   <td>Choose the [!DNL Workfront] object type that you want the module to read.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>
  
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL References]</td>
   <td>Select any reference fields that you want to include in the output.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Collections]</td>
   <td>Select any reference fields that you want to include in the output.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Enter the unique [!DNL Workfront] ID of the record that you want the module to read.</p> <p>To get the ID, open the [!DNL Workfront] object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Update Record]**

This action module updates an object, such as a project, task, or issue. The module allows you to select which of the object's fields are available in the module.

You specify the ID of the record.

The module returns the ID of the  object and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Enter the unique [!DNL Workfront] ID of the record that you want the module to update.</p> <p>To get the ID, open the [!DNL Workfront] object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to update.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Select the fields that you want available for data input. This allows you to use these fields without having to scroll through the ones you don't need.</td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* When entering the ID of an object, you can begin typing the name of the object, then select it from the list. The module then enters the appropriate ID into the field.
>* When entering the text for a custom field or a [!UICONTROL Note] object (Comment or reply), you can use HTML tags in the [!UICONTROL Note Text] field to create rich text, such as bold or italic text.
>
>  For more information on rich text in updates, see [Add an update to a work item](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Upload Document]**

This action module uploads a document to a [!DNL Workfront] object, such as a project, task, or issue. This module uploads the document in chunks, which makes the upload process smoother for Workfront. 

You specify the location for the document, the file you want to upload, and an optional new name for the file.

The module returns the ID of the document and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>Enter the unique [!DNL Workfront] ID of the record to which you want to upload the document.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Related Record Type]</td> 
   <td>Select the type of [!DNL Workfront] record where you want the module to upload the document.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder ID]</td> 
   <td>Depending on the type of related record, you may need to enter or map a folder ID.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Upload Document (Legacy)]**

This action module uploads a document to a [!DNL Workfront] object, such as a project, task, or issue. It uploads the entire document at once. 

You specify the location for the document, the file you want to upload, and an optional new name for the file.

The module returns the ID of the document and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>Enter the unique [!DNL Workfront] ID of the record to which you want to upload the document.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Related Record Type]</td> 
   <td>Select the type of [!DNL Workfront] record where you want the module to upload the document.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder ID]</td> 
   <td>Depending on the type of related record, you may need to enter or map a folder ID.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

### Searches

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Read Related Records]**

This search module reads records that match the search query you specify, in a particular parent object.

You specify which fields you want included in the output. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of the parent record (Workfront object) whose associated records you want to read.</p> <p>See a list of the [!DNL Workfront] object types for which you can use this module in <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] object types available for each [!DNL Workfront] module</a> in this article.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Parent Record ID]</td> 
   <td> <p>Enter or map the ID of the parent record whose associated records you want to read.</p> <p>To get the ID, open the [!DNL Workfront] object in your browser and copy the text at the end of the URL after "ID=." For example: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Select or map the type of child record that you want the module to read.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search]**

This search module looks for records in an object in [!DNL Workfront] that match the search query you specify.

You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to search for.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Select an option to specify whether you want the module to get the first result that matches your search criteria or all the results that match it.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria fields]</td> 
   <td> <p>Select the fields that you want to use for your search criteria. These fields will then be available in the Search criteria dropdown.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to [!DNL Workfront] logs the user into Workfront, and the search will not be successful.</p> <p>Note: <code>In</code> and <code>NotIn</code>work with arrays. The inputs should be in array format.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Select the fields that you want to include in the output for this module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL References]</td> 
   <td>Select any reference fields that you want to include in the search.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Select any collections that you want to add to the search.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search (Legacy)]**

This search module looks for records in an object in [!DNL Workfront] that match the search query you specify.

You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to search for.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Select an option to specify whether you want the module to get the first result that matches your search criteria or all the results that match it.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to [!DNL Workfront] logs the user into Workfront, and the search will not be successful.</p> <p>Note: <code>In</code> and <code>NotIn</code>work with arrays. The inputs should be in array format.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Select the fields that you want to include in the output for this module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL References]</td> 
   <td>Select any reference fields that you want to include in the search.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>Select any collections that you want to add to the search.</td> 
  </tr> 
 </tbody> 
</table>

See a list of the [!DNL Workfront] object types for which you can use this module in [[!DNL Workfront] object types available for each [!DNL Workfront] module](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] object types available for each [!DNL Workfront] module

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Object types available for each [!DNL Workfront] trigger module**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Watch Record]</th> 
   <th>[!UICONTROL Watch Field]</th> 
   <th>[!UICONTROL Watch Events]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Approval Process</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Assignment</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Baseline</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> Billing Record </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Billing Rate</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Company</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dashboard</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document Folder</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Document Request</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Document Version</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Expense</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Expense Type</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Group</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hour</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hour Type</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Issue</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteration</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Job Role</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Journal Entry</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Milestone</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Milestone Path</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Note</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Note Tag</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Project User</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Proof Approval</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Reserved Time* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Report</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risk</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risk Type</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Step Approver</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Task</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Template</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Template Task</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Timesheet</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Update</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Object types available for each [!DNL Workfront] action module**

>[!NOTE]
>
>The [!UICONTROL Download Document] module is not included in this table because [!DNL Workfront] object types are not part of its configuration.

<table style="table-layout:auto"> 
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
   <th> </th> 
   <th>[!UICONTROL Create a record]</th> 
   <th>[!UICONTROL Update a record]</th> 
   <th>[!UICONTROL Delete a record]</th> 
   <th>[!UICONTROL Upload Document]</th> 
   <th>[!UICONTROL Read a record]</th> 
   <th>[!UICONTROL Custom API Call]</th> 
   <th>[!UICONTROL Misc Action]</th> 
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
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Baseline</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
   <tr> 
   <td>Billing Record</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Billing Rate</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Exchange rate</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>External Document</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
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
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hour Type</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Job Role</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Journal Entry</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
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
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Milestone Path</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Reserved Time* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risk</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risk Type</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Step Approver</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Template</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Object types available for each [!DNL Workfront] search module**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Search]</th> 
   <th>[!UICONTROL Read Related Records]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Approval Process</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Assignment</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Billing Record</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Billing Rate</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Company</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document Folder</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Document Version</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Expense</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Expense Type</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Group</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hour</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hour Type</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Issue</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteration</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Job Role</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Journal Entry</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Milestone</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Milestone Path</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Note</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Note Tag</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Project User</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Reserved Time* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risk</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risk Type</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Step Approver</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Task</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Template</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Template Task</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Timesheet</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>User Delegation</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

 We recommend that you double check to ensure this works the way you would expect it to.

+++

## Event subscription filters in the [!DNL Workfront] > [!UICONTROL Watch Events] modules 

>[!NOTE]
>
>We highly recommend using event subscription filters in your [!UICONTROL Watch Events] modules.

The [!DNL Workfront] [!UICONTROL Watch Events] module triggers scenarios based on a webhook that creates an event subscription in the [!DNL Workfront] API. The event subscription is a set of data that determines which events are sent to the webhook. For example, if you set up a [!UICONTROL Watch Events] module that is watching for issues, then the event subscription sends only events related to issues.

By using event subscription filters, Fusion users can create event subscriptions that are a better fit for their use cases. For example, you can set up an event subscription in the [!DNL Workfront] API to send only issues that are in a specific project to the webhook, ensuring that the [!UICONTROL Watch Events] module will only trigger for issues in that project. The ability to create narrower triggers improves scenario design by reducing the number of irrelevant triggers.

This is different from setting up a filter in the [!DNL Workfront Fusion] scenario. Without an event subscription filter, your webhook receives all events related to the object type you select. Most of these events would be irrelevant to the scenario, and must be filtered out before the scenario can continue.

The following operators are available in the Workfront > Watch events filter:

* Equals
* Not equals
* Greater than
* Less than
* Greater than or equal to
* Less than or equal to
* Contains
* Exists
    * This operator does not require a value, and the value field is absent.
* Does not exist
    * This operator does not require a value, and the value field is absent.
* Changed
    * This operator does not require a value, and the value field is absent.
    * This operator ignores the State field.
    * When using `Changed`, select **Updated Events Only** in the **Record Origin** field. 

>[!IMPORTANT]
>
>You cannot edit filters in existing [!DNL Workfront] webhooks. To set up different filters for [!DNL Workfront] event subscriptions, remove the current webhook and create a new one.

>[!INFO]
>
>**Example:** Consider a scenario that processes new issues that are assigned to a specific user, Ana.
>
>### Filter events by using an event subscription filter (recommended)
>
>Using the event filter, you can set up the webhook to trigger the scenario when an issue is assigned to Ana when the issue is created. Ana has the userID b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>If 100 issues are created in a day, but only two of them are assigned to Ana, the scenario would execute twice.
>
>### Filter events inside the scenario (not recommended)
>
>To filter events so that only issues assigned to Ana are processed, you could create a filter after the [!UICONTROL Watch Events] module.
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>If 100 issues are created in a day, but only two of them are assigned to Ana, the scenario would execute 100 times. 98 of the executions would stop at the filter, but the trigger module is still consuming data and performing operations in all of the executions.

For more information on event subscriptions, see [FAQs - Event Subscriptions](../../wf-api/general/event-subs-faq.md).

For more information on webhooks, see [Instant triggers (webhooks) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

For more information on filters in scenarios, see [Add a filter to a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
 