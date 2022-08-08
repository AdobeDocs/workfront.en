---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Adobe Journey Optimizer, as well as connect it to multiple third-party applications and services. 
author: Becky
---

# Adobe Journey Optimizer Modules

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

In an Adobe Workfront Fusion scenario, you can automate workflows that use Adobe Journey Optimizer, as well as connect it to multiple third-party applications and services. Adobe Journey Optimizer modules allow you to ,reate, read, update, or delete records,list all records of a given type, search records based on criteria you specify, or perform a custom API call to the Adobe Journey Optimizer API.


If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Adobe Workfront plan*</td>
      <td>
        <p>Pro or higher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Adobe Workfront license*</td>
      <td>
        <p>Plan, Work</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Adobe Workfront Fusion license**</td>
      <td >
        <p>Workfront Fusion for Work Automation and Integration</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">Access level configurations*</td>
      <td>
        <p>You must be a Workfront Fusion administrator for your organization.</p>
        <p>You must be a Workfront Fusion administrator for your team.</p>
      </td>
    </tr>
  </tbody>
</table>


&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

Before you can use the Adobe Journey Optimizer connector, you must ensure that the following prerequisites are met:

*   You must have an active Adobe Journey Optimizer account.

## Create a connection to Adobe Journey Optimizer

To create a connection for your Adobe Journey Optimizer modules:

1.  In any Adobe Journey Optimizer module, click **Add** next to the Connection box.
    
1.  Fill in the following fields:
      
    <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">Connection name</td>
          <td>
            <p>Enter a name for this connection.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">Client ID</td>
          <td>Enter your Adobe Client ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
        </tr>
        <tr>
          <td role="rowheader">Client Secret</td>
          <td>Enter your Adobe Client Secret. This can be found in the Credentials details section of the Adobe Developer Console</td>
        </tr>
        <tr>
          <td role="rowheader">Technical account ID</td>
          <td>Enter your Adobe Technical account ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
        </tr>
        <tr>
          <td role="rowheader">Organization ID</td>
          <td>Enter your Adobe Organization ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
        </tr>
        <tr>
          <td role="rowheader">Meta Scopes</td>
          <td>
            Enter any meta scopes needed for the connection.
          </td>
        </tr>
        <tr>
          <td role="rowheader">Private key</td>
          <td>
            <p>Enter the private key that was generated when your credentials were created in the Adobe Developer Console. </p>
            <p>To extract your private key or certificate:</p>
            <ol>
              <li value="1">
                <p>Click <b>Extract</b>.</p>
              </li>
              <li value="2">
                <p>Select the type of file you are extracting.</p>
              </li>
              <li value="3">
                <p>Select the file that contains the private key or certificate.</p>
              </li>
              <li value="4">
                <p>Enter the password for the file.</p>
              </li>
              <li value="5">
                <p>Click <b>Save</b> to extract the file and return to the connection setup.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. Click **Continue** to save the connection and return to the module.

## Adobe Journey Optimizer modules and their fields

When you configure Adobe Journey Optimizer modules, Workfront Fusion displays the fields listed below. Along with these, additional Adobe Journey Optimizer fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Create a record

This action module creates a placement, decision rule, tag, personalized offer, collection, or fallback offer.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
     <td>For instructions on creating a connection to Adobe Journey Optimizer, see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to Adobe Journey Optimizer</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        Record Type
      </td>
      <td>
        Select the type of record that you want to create
        <ul>
        <li><b>Placement</b>: Continue to <a href="#placement-fields" >Placement fields</a>.</li>
        <li><b>Decision rule</b>: Continue to <a href="#decision-rule-fields" >Decision rule fields</a>.</li>
        <li><b>Decision</b>: Continue to <a href="#decision-fields" >Decision fields</a>.</li>
        <li><b>Tag</b>: Continue to <a href="#tag-fields" >Tag fields</a>.</li>
        <li><b>Collection</b>: Continue to <a href="#collection-fields" >Collection fields</a>.</li>
        <li><b>Fallback offer</b>: Continue to <a href="fallback-offer-fields" >Fallback offer fields</a>.</li>
        <li><b>Personalized offer</b>: Continue to <a href="#personalized-offer-fields" >Personalized offer fields</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### Placement fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
     <td>Enter or map a name for the placement.</td>
    </tr>
    <tr>
      <td role="rowheader">
        Description
      </td>
      <td>Enter or map a description for the placement.
      </td>
    </tr>
  </tbody>
</table>


#### Decision rule fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
     <td>Enter or map a name for the description rule.</td>
    </tr>
    <tr>
      <td role="rowheader">
        Description
      </td>
      <td>Enter or map a description for the decision rule.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Condition
      </td>
      <td>Enter or map the condition the decision rule.
      </td>
    </tr>
  </tbody>
</table>

#### Decision fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
     <td>Enter or map a name for the description rule.</td>
    </tr>
    <tr>
      <td role="rowheader">Status</td>
      <td>Select the status for the decision.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Start date</td>
      <td><p>Enter or map the start date for the decision.</p><p>For a list of supported date formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">End date</td>
      <td><p>Enter or map the end date for the decision.</p><p>For a list of supported date formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">Placements</td>
      <td>Select the placements to add to this decision
      </td>
    </tr>
   <tr>
      <td role="rowheader">Collection</td>
      <td>Select the offer collection that contains the offers that this decision will consider.
      </td>
    </tr>
   <tr>
      <td role="rowheader">Fallback offer</td>
      <td>Select the fallback offer that will be presented to customers that do not match the rules for this decision.
      </td>
    </tr>
  </tbody>
</table>

#### Tag fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
     <td>Enter or map a name for the tag.</td>
    </tr>
  </tbody>
</table>

#### Collection fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
     <td>Enter or map a name for the collection.</td>
    </tr>
    <tr>
      <td role="rowheader">
        Filter Type
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Elements
      </td>
      <td>Select the tags to include in the colelction.
      </td>
    </tr>
  </tbody>
</table>

#### Fallback offer fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
     <td>Enter or map a name for the fallback offer.</td>
    </tr>
    <tr>
      <td role="rowheader">
        Status
      </td>
      <td> Select the status of the fallback offer.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Placement
      </td>
      <td>Enter or map the placement for the fallback offer.
      </td>
    </tr>
  </tbody>
</table>

#### Personalized offer fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
     <td>Enter or map a name for the description rule.</td>
    </tr>
    <tr>
      <td role="rowheader">Status</td>
      <td>Select the status for the decision.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Placement</td>
      <td>Select the placement for the personalized offer.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Start date</td>
      <td><p>Enter or map the start date for the personalized offer.</p><p>For a list of supported date formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">End date</td>
      <td><p>Enter or map the end date for the personalized offer.</p><p>For a list of supported date formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">Decision rules</td>
      <td>Select the decision rules to add to this personalized offer.
      </td>
    </tr>
   <tr>
      <td role="rowheader">Priority</td>
      <td>Select the priority of this offer. Priority affects whether this offer will be presented rather than another offer.
      </td>
    </tr>
   <tr>
      <td role="rowheader">Capping constraint</td>
      <td>Enter or map the number of times this offer will be presented.
      </td>
    </tr>
  </tbody>
</table>

### Make a custom API call

This module makes a custom API call to the Adobe Journey Optimizer API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
     <td>For instructions on creating a connection to Adobe Journey Optimizer, see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to Adobe Journey Optimizer</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Path</p>
      </td>
      <td>
        <p>Enter a path relative to {baseURL} starting with<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Method</p>
      </td>
      <td>
        <p>Select the HTTP request method you need to configure the API call. For more information, see HTTP request methods.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Headers</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion adds authorization headers and x-api-key headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Query String  </td>
      <td>
        <p>Enter the request query string.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Body</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">Limit  </td>
      <td>
        <p>Enter the maximum number of results that you want the module to return in one execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

### Get records

This search module lists records of the selected type, returning results based on criteria you specify.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
     <td>For instructions on creating a connection to Adobe Journey Optimizer, see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to Adobe Journey Optimizer</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Record type</p>
      </td>
      <td>
        <p>Select the type of record that you want to list.</p>
        <ul>
        <li>Placements</li>
        <li>Decision rules</li>
        <li>Tags</li>
        <li>Personalized offers</li>
        <li>Collections</li>
        <li>Fallback offers</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Query operator</p>
      </td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader"></td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader"> </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader"></td>
   <td>
    </td>
     </tr>
     <tr>
      <td role="rowheader">  </td>
      <td>
      </td>
    </tr>
  </tbody>
</table>
