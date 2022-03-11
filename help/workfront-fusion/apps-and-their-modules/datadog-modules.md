---
filename: datadog-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Datadog modules
description: In a Adobe Workfront Fusion scenario, you can connect your Datadog account to multiple third-party applications and services.
---

# Datadog modules

In a Adobe Workfront Fusion scenario, you can connect your Datadog account to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

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
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Datadog modules, you must have a Datadog account.

## Connect Datadog to Workfront Fusion

### Retrieve your API key and application key

To connect your Datadog account to Workfront Fusion you need to retrieve an API Key and an application key from your Datadog account.

1. Log in to your Datadog account.
1. In the left navigation panel, click `Integrations`, then click `APIs`.
1. On the main screen, click `API Keys`. 
1. Hover over the purple bar to reveal the API key.
1. Copy the API key to a secure location.
1. On the main screen, click `Application Keys`. 
1. Hover over the purple bar to reveal the application key.
1. Copy the application key to a secure location.

### Create a connection to Datadog in Workfront Fusion

You can create a connection to your Datadog account directly from inside a Datadog module.

<ol> 
 <li value="1"> <p>In any Datadog module, click <span class="bold">Add </span>next to the Connection field.</p> </li> 
 <li value="2"> <p>Fill the module's fields as follows:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Connection Type</td> 
     <td> <p> Select the Datadog Application option to get full access to Datadog API.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Connection Name</td> 
     <td> <p> Enter a name for the connection.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Domain </td> 
     <td> <p>Select the domain you want to connect to (US or EU).</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">API Key</td> 
     <td> <p> Enter your Datadog API key. </p> <p>For instructions on retrieving the API key, see <a href="#retrieve" class="MCXref xref">Retrieve your API key and application key</a> in this article.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Application Key</td> 
     <td> <p> Enter your Datadog application key. </p> <p>For instructions on retrieving the application key, see <a href="#retrieve" class="MCXref xref">Retrieve your API key and application key</a> in this article.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3"> <p>Click <span class="bold">Continue</span> to create the connection and go back to the module.</p> </li> 
</ol>

## Datadog modules and their fields

When you configure Datadog modules, Workfront Fusion displays the fields listed below. Along with these, additional Datadog fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Actions

* [Post Timeseries Points](#post) 
* [Make an API Call](#make)

#### Post Timeseries Points

The module allows you to post time-series data that can be graphed on Datadog’s dashboards.

The limit for compressed payloads is 3.2 megabytes (3200000), and 62 megabytes (62914560) for decompressed payloads.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Datadog account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Datadog to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Series</td> 
   <td> <p>Add time series you want to submit to Datadog.</p> 
    <ul> 
     <li> <p><span class="bold">Metric </span> </p> <p>Enter the name of the timeseries.</p> </li> 
     <li> <p><span class="bold">Type </span> </p> <p>Select the type of the metric.</p> </li> 
     <li> <p><span class="bold">Interval</span> </p> <p> If the type of the metric is rate or count, define the corresponding interval.</p> </li> 
     <li> <p><span class="bold">Points</span> </p> <p>Add points relating to a metric.</p> <p>This is a JSON array of points. Each point has the format: <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Note:  <p>The timestamp must be in seconds.</p> <p>The timestamp must be current. Current is defined as not more than 10 minutes in the future or more than 1 hour in the past.</p> <p> The numeric value format should be a float value.</p> </p> <p>This field must contain at least 1 item.</p> </li> 
     <li> <p><span class="bold">Host </span> </p> <p>Enter the name of the host that produced the metric.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Make an API Call

This action module allows you to perform a custom API call.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Datadog account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Datadog to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter a path relative to<code>https://api.datadoghq.com/api/</code>. Example:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds the authorization headers for you.</p> </td> 
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

` `**Example: **`` The following API call returns the all dashboards in your Datadog account:

URL:

```
/v1/dashboard
```

Method:

```
GET
```

![](assets/datadog-api-example.png)

The result can be found in the module's Output under Bundle > Body > dashboards.

In our example, 3 dashboards were returned:

![](assets/datadog-api-response-example.png)

