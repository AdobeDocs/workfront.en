---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Adobe Target, as well as connect it to multiple third-party applications and services. Adobe Target modules allow you to create, read, update, or delete records, list all records of a given type, search records based on criteria you specify, or perform a custom API call to the Adobe Target API.
author: Becky
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
---
# Adobe Target Modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use Adobe Target, as well as connect it to multiple third-party applications and services. Adobe Target modules allow you to ,reate, read, update, or delete records,list all records of a given type, search records based on criteria you specify, or perform a custom API call to the Adobe Target API.


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

Before you can use the Adobe Target connector, you must ensure that the following prerequisites are met:

*   You must have an active Adobe Target account.

## Create a connection to Adobe Target

To create a connection for your Adobe Target modules:

1.  Click Add next to the Connection box.
    
2.  Fill in the following fields:
    
  <table>
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
        <td role="rowheader">Organization ID</td>
        <td>Enter your Adobe Organization ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Technical account ID</td>
        <td>Enter your Adobe Technical account ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Tenant</td>
        <td>
          <p> To locate your Tenant, log in to the Adobe Experience Cloud, open Target, and click the Target card. Use the Tenant ID value as noted in the URL subdomain.</p>
          <p>For example, if your URL when logged in to Adobe Target is <code>&lt;https://mycompany.experiencecloud.adobe.com/...&gt;</code> then your Tenant ID is “mycompany.”</p>
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
    
1.  Click **Continue** to save the connection and return to the module.
    
## Adobe Target modules and their fields

When you configure Adobe Target modules, Workfront Fusion displays the fields listed below. Along with these, additional Adobe Target fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

*   [Actions](#Actions)
    
*   [Searches](#Searches)
    

### Actions

*   [Create a record](#Create2)
    
*   [Make a custom API call](#Make)
    
*   [Delete a record](#Delete)
    
*   [Read a record](#Read)
    
*   [Update a record](#Update)
    

#### Create a record

This action module creates an AB or XT activity, an offer, or an audience.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">Connection</td>
    <td>For instructions on creating a connection to Adobe Target, see <a href="#Create" class="MCXref_0">Create a connection to Adobe Target</a> in this article.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Record type</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Select the type of record that you want to create.</p>
      <ul>
        <li>
          <p>AB&#160;Activity</p>
          <p>Continue to <a href="#AB%C2%A0Activ" class="MCXref_0">AB&#160;Activity fields</a>.</p>
        </li>
        <li>
          <p>XT Activity</p>
          <p>Continue to <a href="#XT" class="MCXref_0">XT Activity fields</a>.</p>
        </li>
        <li>
          <p>Offer</p>
          <p>Continue to <a href="#Offer" class="MCXref_0">Offer fields</a>.</p>
        </li>
        <li>
          <p>Audience</p>
          <p>Continue to <a href="#Audience" class="MCXref_0">Audience fields</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### AB Activity fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">Options</td>
      <td>
        <p>For each option that you want to add to the activity, click <b>Add item</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p><b>Option local ID</b>
            </p>
            <p>Enter or map a string to be used to track the option across API requests.</p>
          </li>
          <li>
            <p><b>Name</b>
            </p>
            <p>Enter or map a name for the option. The name must be no more than 250 characters.</p>
          </li>
          <li>
            <p><b>Offer ID</b>
            </p>
          </li>
          <li>
            <p>Select or map the Offer associated with the option.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Locations</td>
      <td>
        <p>For each Mbox that you want to add to the activity, click <b>Add item</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>Audience IDs</p>
            <p>Fir each audience that you want to add to the Mbox, click <b>Add item</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>Location local ID</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>Name</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Experiences</td>
      <td>
        <p>A list of locations on the page where the content offer is served. A location contains the following:
</p>
        <ul>
          <li>
            <p><b>Experience local ID</b>
            </p>
            <p>Enter or map the ID&#160;of the experience</p>
          </li>
          <li>
            <p><b>Name</b>
            </p>
            <p>Enter or map the name of the experience

</p>
          </li>
          <li>
            <p><b>Audience IDs</b>
            </p>
            <p>For each audience that you want to see the experience, click <b>Add item</b> and enter the Audience ID.

</p>
          </li>
          <li>
            <p><b>Visitor Percentage</b>
            </p>
            <p>Enter or map the percentage of visitors that is allocated to the experience</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Metrics</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Third Party ID</td>
      <td>Enter or map an ID to identify this activity. You can choose this ID. This ID&#160;must not be the same as another activity, and can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">Starts at</td>
      <td>Enter or map the date and time to start the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">Ends at</td>
      <td>Enter or map the date and time to end the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">State</td>
      <td>
        <p>Enter or map the state of the activity.</p>
        <ul>
          <li>
            <p>Approved</p>
          </li>
          <li>
            <p>Deactivated</p>
          </li>
          <li>
            <p>Paused</p>
          </li>
          <li>
            <p>Saved </p>
          </li>
          <li>
            <p>Deleted</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Priority</td>
      <td>Enter a number that defines the priority of the activity. Higher numbers have higher priority. This value must be between 0 and 999. The default value is 5.</td>
    </tr>
    <tr>
      <td role="rowheader">Auto-allocate traffic</td>
      <td>
        <p>Enable this option to auto-allocate traffic. Auto-allocating sends more traffic to the more successful experience.</p>
        <p>Select or map the evaluation criteria by which to judge which experience is more successful.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Workspace</td>
      <td>Enter or map the workspace that the activity is associated with</td>
    </tr>
    <tr>
      <td role="rowheader">Property IDs </td>
      <td>For each property that you want to add to the activity, click <b>Add item</b> and select or map the property's ID.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Reporting audiences</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>For each reporting audience that you want to add to the activity, click Add item and enter the following information:</p>
        <ul>
          <li>
            <p><b>Reporting Audience local ID</b>
            </p>
            <p>Enter or map a string to be used to track the Reporting Audience across API requests.</p>
          </li>
          <li>
            <p><b>Audience ID</b>
            </p>
            <p>Enter or map the Segment to be used in reporting</p>
          </li>
          <li>
            <p><b>Metric local ID</b>
            </p>
            <p>Enter or map a string to be used to track the metric across API requests.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### XT Activity fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">Options</td>
      <td>
        <p>For each option that you want to add to the activity, click <b>Add item</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p><b>Option local ID</b>
            </p>
            <p>Enter or map a string to be used to track the option across API requests.</p>
          </li>
          <li>
            <p><b>Name</b>
            </p>
            <p>Enter or map a name for the option. The name must be no more than 250 characters.</p>
          </li>
          <li>
            <p><b>Offer ID</b>
            </p>
          </li>
          <li>
            <p>Select or map the Offer associated with the option.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Locations</td>
      <td>
        <p>For each Mbox that you want to add to the activity, click <b>Add item</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>Audience IDs</p>
            <p>Fir each audience that you want to add to the Mbox, click <b>Add item</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>Location local ID</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>Name</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Experiences</td>
      <td>
        <p>A list of locations on the page where the content offer is served. A location contains the following:
</p>
        <ul>
          <li>
            <p><b>Experience local ID</b>
            </p>
            <p>Enter or map the ID&#160;of the experience</p>
          </li>
          <li>
            <p><b>Name</b>
            </p>
            <p>Enter or map the name of the experience

</p>
          </li>
          <li>
            <p><b>Audience IDs</b>
            </p>
            <p>For each audience that you want to see the experience, click <b>Add item</b> and enter the Audience ID.

</p>
          </li>
          <li>
            <p><b>Visitor Percentage</b>
            </p>
            <p>Enter or map the percentage of visitors that is allocated to the experience</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Metrics</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Third Party ID</td>
      <td>Enter or map an ID to identify this activity. You can choose this ID. This ID&#160;must not be the same as another activity, and can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">Starts at</td>
      <td>Enter or map the date and time to start the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">Ends at</td>
      <td>Enter or map the date and time to end the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">State</td>
      <td>
        <p>Enter or map the state of the activity.</p>
        <ul>
          <li>
            <p>Approved</p>
          </li>
          <li>
            <p>Deactivated</p>
          </li>
          <li>
            <p>Paused</p>
          </li>
          <li>
            <p>Saved </p>
          </li>
          <li>
            <p>Deleted</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Priority</td>
      <td>Enter a number that defines the priority of the activity. Higher numbers have higher priority. This value must be between 0 and 999. The default value is 5.</td>
    </tr>
    <tr>
      <td role="rowheader">Auto-allocate traffic</td>
      <td>
        <p>Enable this option to auto-allocate traffic. Auto-allocating sends more traffic to the more successful experience.</p>
        <p>Select or map the evaluation criteria by which to judge which experience is more successful.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Workspace</td>
      <td>Enter or map the workspace that the activity is associated with</td>
    </tr>
    <tr>
      <td role="rowheader">Property IDs </td>
      <td>For each property that you want to add to the activity, click <b>Add item</b> and select or map the property's ID.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Reporting audiences</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>For each reporting audience that you want to add to the activity, click Add item and enter the following information:</p>
        <ul>
          <li>
            <p><b>Reporting Audience local ID</b>
            </p>
            <p>Enter or map a string to be used to track the Reporting Audience across API requests.</p>
          </li>
          <li>
            <p><b>Audience ID</b>
            </p>
            <p>Enter or map the Segment to be used in reporting</p>
          </li>
          <li>
            <p><b>Metric local ID</b>
            </p>
            <p>Enter or map a string to be used to track the metric across API requests.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Offer fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">Content</td>
      <td>
        <p>Enter or map the content of the Offer that will be shown to the user.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Workspace</td>
      <td>
        <p>Enter or map the ID of the workspace associated with the offer. If left blank, the offer is associated with the default workspace of the account. This functionality applies only to Target Premium accounts.</p>
      </td>
    </tr>
  </tbody>
</table>

##### Audience fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
      <td>Enter or map a name for this audience. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">Content</td>
      <td>
        <p>Enter or map a description of this audience.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Target Rule</td>
      <td>
        <p>Enable the toggle to make rules AND, that is, all rules must be applied.</p>
        <p>For each rule that you want to apply to the audience, click <b>Add item</b> and enter the JSON of the rule you want to apply. </p>
        <div class="example"><span class="autonumber"><span><b>Example: </b></span></span>
          <p>Examples:</p>
          <p ><code>{</code></p>
                    <p ><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;"page": "url",</code>
                    </p>
                    <p><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;"equals":[</code>
                    </p>
                    <p ><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;"http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;]</code>
                    </p>
                    <p ><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;},</code>
                    </p>
                    <p ><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;{</code>
                    </p>
                    <p><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;"geo": "region",</code>
                    </p>
                    <p><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;"matches": [</code>
                    </p>
                    <p ><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;"california"</code>
                    </p>
                    <p ><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;]</code>
                    </p>
                    <p ><code>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;}</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Workspace</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Enter or map the ID of the workspace associated with the audience. If left blank, the offer is associated with the default workspace of the account. This functionality applies only to Target Premium accounts.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Make a custom API call

This module makes a custom API call to the Adobe Target API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>For instructions on creating a connection to Adobe Target, see <a href="#Create" class="MCXref_0">Create a connection to Adobe Target</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">Target Base URL</td>
      <td>Enter or map your Target base URL.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Path</p>
      </td>
      <td>
        <p>Enter a path relative to {baseURL}/</p>
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
  </tbody>
</table>

#### Delete a record

This action module deletes a single AB activity, XT activity, Offer, or Audience.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">Connection</td>
    <td>For instructions on creating a connection to Adobe Target, see <a href="#Create" class="MCXref_0">Create a connection to Adobe Target</a> in this article.</td>
  </tr>
  <tr>
    <td role="rowheader">Record type</td>
    <td>Select the type of record that you want to delete.</td>
  </tr>
  <tr>
    <td role="rowheader">Record ID</td>
    <td>Enter or map the ID&#160;of the record you want to delete.</td>
  </tr>
</tbody>
</table>

#### Read a record

This action module retrieves data for a single Activity, Offer, Audience, Property, or Report.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">Connection</td>
    <td>For instructions on creating a connection to Adobe Target, see <a href="#Create" class="MCXref_0">Create a connection to Adobe Target</a> in this article.</td>
  </tr>
  <tr>
    <td role="rowheader">Record type</td>
    <td>Select the type of record that you want to read.</td>
  </tr>
  <tr>
    <td role="rowheader">Record ID</td>
    <td>Enter or map the ID&#160;of the record you want to read.</td>
  </tr>
</tbody>
</table>

#### Update a record

This action module updates an Activity, Offer, or Audience.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>For instructions on creating a connection to Adobe Target, see <a href="#Create" class="MCXref_0">Create a connection to Adobe Target</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">Record type</td>
      <td>
        <p>Select the type of record that you want to update.</p>
        <ul>
          <li>
            <p><b>AB Activity</b>
            </p>
            <p>See field descriptions in <a href="#AB%C2%A0Activ" class="MCXref_0">AB&#160;Activity fields</a> under <a href="#Create2" class="MCXref_0">Create a record</a>.</p>
          </li>
          <li>
            <p><b>XT&#160;Activity</b>
            </p>
            <p>See field descriptions in <a href="#XT" class="MCXref_0">XT Activity fields</a> under <a href="#Create2" class="MCXref_0">Create a record</a>.</p>
          </li>
          <li>
            <p><b>Other Activity</b>
            </p>
            <p>Select the field that you want to update a value for, then enter the new value for the field.</p>
          </li>
          <li>
            <p><b>Offer</b>
            </p>
            <p>See field descriptions in <a href="#Offer" class="MCXref_0">Offer fields</a> under <a href="#Create2" class="MCXref_0">Create a record</a>.</p>
          </li>
          <li>
            <p><b>Audience</b>
            </p>
            <p>See field descriptions in <a href="#Audience" class="MCXref_0">Audience fields</a> under <a href="#Create2" class="MCXref_0">Create a record</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Record ID</td>
      <td>Enter or map the ID&#160;of the record you want to update.</td>
    </tr>
  </tbody>
</table>

### Searches

*   [Get records](#Get)
    
*   [Search](#Search)
    

#### Get records

This search module retrieves a list of records of the selected type.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>For instructions on creating a connection to Adobe Target, see <a href="#Create" class="MCXref_0">Create a connection to Adobe Target</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">Record type</td>
      <td>Select the type of record that you want to update.</td>
    </tr>
    <tr>
      <td role="rowheader">Sort by</td>
      <td>For each field that you want to sort by, click <b>Add item</b> and select the field and whether the returned results should be ascending or descending.</td>
    </tr>
    <tr>
      <td role="rowheader">Starts At</td>
      <td>
        <p>Enter the earliest date that you want to retrieve records for. </p>
        <p>For a list of supported date and time formats, see Type coercion.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ends At</td>
      <td>
        <p>Enter the latest date that you want to retrieve records for. </p>
        <p>For a list of supported date and time formats, see Type coercion.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Search

This search module searches for Activities, Offers, or Audiences based on criteria you specify.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">Connection</td>
    <td>For instructions on creating a connection to Adobe Target, see <a href="#Create" class="MCXref_0">Create a connection to Adobe Target</a> in this article.</td>
  </tr>
  <tr>
    <td role="rowheader">Record type</td>
    <td>Select the type of record that you want to update.</td>
  </tr>
  <tr>
    <td role="rowheader">Sort by</td>
    <td>For each field that you want to sort by, click <b>Add item</b> and select the field and whether the returned results should be ascending or descending.</td>
  </tr>
  <tr>
    <td role="rowheader">Search criteria</td>
    <td>For each rule you want to set up, select the field, the operator, and the value. Click the <b>Add AND&#160;rule</b> to create additional rules.</td>
  </tr>
  <tr>
    <td role="rowheader">Offset</td>
    <td>
      <p>Enter the number of the first response that you want the module to return. The first returned response has an offset of <code>0</code>. Use this field in combination with the Maximum number of returned results field to paginate the responses.</p>
      <p>For example, to see the third page of responses, when each page has ten responses, set Offset to 20 and Maximum number of returned results to 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Maximum number of returned results</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle. Use this field in combination with the Offset field to paginate the responses.</p>
      <p>For example, to see the third page of responses, when each page has ten responses, set Offset to 20 and Maximum number of returned results to 10.</p>
    </td>
  </tr>
</tbody>
</table>
