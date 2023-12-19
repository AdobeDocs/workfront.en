---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] modules allow you to create, read, update, or delete records, list all records of a given type, search records based on criteria you specify, or perform a custom API call to the [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
---
# [!DNL Adobe Target] Modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] modules allow you to ,reate, read, update, or delete records,list all records of a given type, search records based on criteria you specify, or perform a custom API call to the [!DNL Adobe Target] API.


If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] or higher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>
      <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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
    </tr>
  </tbody>
</table>


To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisites

Before you can use the [!DNL Adobe Target] connector, you must ensure that the following prerequisites are met:

* You must have an active [!DNL Adobe Target] account.

## Create a connection to [!DNL Adobe Target]

To create a connection for your [!DNL Adobe Target] modules:

1. Click **[!UICONTROL Add]** next to the Connection box.

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
          <p>Enter a name for this connection.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Enter your [!DNL Adobe] Client ID. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Enter your [!DNL Adobe] Client Secret. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Enter your [!DNL Adobe] Organization ID. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Enter your [!DNL Adobe] Technical account ID. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tenant]</td>
        <td>
          <p> To locate your Tenant, log in to the [!DNL Adobe Experience Cloud], open [!DNL Target], and click the [!DNL Target] card. Use the Tenant ID value as noted in the URL subdomain.</p>
          <p>For example, if your URL when logged in to [!DNL Adobe Target] is <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> then your Tenant ID is "mycompany."</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>Enter <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>Enter the private key that was generated when your credentials were created in the [!DNL Adobe Developer Console]. </p>
          <p>To extract your private key or certificate:</p>
          <ol>
            <li value="1">
              <p>Click <b>[!UICONTROL Extract]</b>.</p>
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
              <p>Click <b>[!UICONTROL Save]</b> to extract the file and return to the connection setup.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Click **[!UICONTROL Continue]** to save the connection and return to the module.

## [!DNL Adobe Target] modules and their fields

When you configure [!DNL Adobe Target] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Adobe Target] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)

* [Searches](#searches)


### Actions

* [[!UICONTROL Create a record]](#create-a-record)

* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)

* [[!UICONTROL Delete a record]](#delete-a-record)

* [[!UICONTROL Read a record]](#read-a-record)

* [[!UICONTROL Update a record]](#update-a-record)


#### [!UICONTROL Create a record]

This action module creates an AB or XT activity, an offer, or an audience.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>For instructions on creating a connection to [!DNL Adobe Target], see <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Create a connection to [!DNL Adobe Target]</a> in this article.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Record type]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Select the type of record that you want to create.</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>Continue to <a href="#ab-activity-fields" class="MCXref xref" >AB Activity fields</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT Activity]</p>
          <p>Continue to <a href="#xt-activity-fields" class="MCXref xref" >XT Activity fields</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Offer]</p>
          <p>Continue to <a href="#offer-fields" class="MCXref xref" >Offer fields</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>Continue to <a href="#audience-fields" class="MCXref xref" >Audience fields</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### AB Activity fields

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>For each option that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the option across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the option. The name must be no more than 250 characters.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Select or map the Offer associated with the option.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locations]</td>
      <td>
        <p>For each Mbox that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>A list of locations on the page where the content offer is served. A location contains the following:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Enter or map the ID of the experience</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map the name of the experience

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>For each audience that you want to see the experience, click <b>[!UICONTROL Add item]</b> and enter the Audience ID.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>Enter or map the percentage of visitors that is allocated to the experience</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Enter or map an ID to identify this activity. You can choose this ID. This ID must not be the same as another activity, and can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>Enter or map the date and time to start the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>Enter or map the date and time to end the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Enter or map the state of the activity.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Enter a number that defines the priority of the activity. Higher numbers have higher priority. This value must be between 0 and 999. The default value is 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>Enable this option to auto-allocate traffic. Auto-allocating sends more traffic to the more successful experience.</p>
        <p>Select or map the evaluation criteria by which to judge which experience is more successful.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Enter or map the workspace that the activity is associated with</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>For each property that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and select or map the property's ID.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>For each reporting audience that you want to add to the activity, click [!UICONTROL Add item] and enter the following information:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the Reporting Audience across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Enter or map the Segment to be used in reporting</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the metric across API requests.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### XT Activity fields

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>For each option that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the option across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the option. The name must be no more than 250 characters.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Select or map the Offer associated with the option.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locations]</td>
      <td>
        <p>For each Mbox that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>A list of locations on the page where the content offer is served. A location contains the following:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Enter or map the ID of the experience</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map the name of the experience

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>For each audience that you want to see the experience, click <b>[!UICONTROL Add item]</b> and enter the Audience ID.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>Enter or map the percentage of visitors that is allocated to the experience</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Enter or map an ID to identify this activity. You can choose this ID. This ID must not be the same as another activity, and can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>Enter or map the date and time to start the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>Enter or map the date and time to end the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Enter or map the state of the activity.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Enter a number that defines the priority of the activity. Higher numbers have higher priority. This value must be between 0 and 999. The default value is 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>Enable this option to auto-allocate traffic. Auto-allocating sends more traffic to the more successful experience.</p>
        <p>Select or map the evaluation criteria by which to judge which experience is more successful.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Enter or map the workspace that the activity is associated with</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>For each property that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and select or map the property's ID.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>For each reporting audience that you want to add to the activity, click [!UICONTROL Add item] and enter the following information:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the Reporting Audience across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Enter or map the Segment to be used in reporting</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the metric across API requests.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Offer fields

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Enter or map the content of the Offer that will be shown to the user.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Enter or map the ID of the workspace associated with the offer. If left blank, the offer is associated with the default workspace of the account. This functionality applies only to [!DNL Target] Premium accounts.</p>
      </td>
    </tr>
  </tbody>
</table>

##### Audience fields

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this audience. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Enter or map a description of this audience.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target Rule]</td>
      <td>
        <p>Enable the toggle to make rules AND, that is, all rules must be applied.</p>
        <p>For each rule that you want to apply to the audience, click <b>[!UICONTROL Add item]</b> and enter the JSON of the rule you want to apply. </p>
        <div class="example"><span class="autonumber"><span><b>Example: </b></span></span>
          <p>Examples:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Enter or map the ID of the workspace associated with the audience. If left blank, the offer is associated with the default workspace of the account. This functionality applies only to [!DNL Target Premium] accounts.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Make a custom API call]

This module makes a custom API call to the [!DNL Adobe Target] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Target], see <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Create a connection to [!DNL Adobe Target]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] Base URL]</td>
      <td>Enter or map your [!DNL Target] base URL.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Enter a path relative to {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adds authorization headers and x-api-key headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Enter the request query string.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a record]

This action module deletes a single AB activity, XT activity, Offer, or Audience.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>For instructions on creating a connection to [!DNL Adobe Target], see <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Create a connection to [!DNL Adobe Target]</a> in this article.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Select the type of record that you want to delete.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Enter or map the ID of the record you want to delete.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Read a record]

This action module retrieves data for a single Activity, Offer, Audience, Property, or Report.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>For instructions on creating a connection to [!DNL Adobe Target], see <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Create a connection to [!DNL Adobe Target]</a> in this article.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Select the type of record that you want to read.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Enter or map the ID of the record you want to read.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Update a record]

This action module updates an Activity, Offer, or Audience.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Target], see <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Create a connection to [!DNL Adobe Target]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>
        <p>Select the type of record that you want to update.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>See field descriptions in <a href="#ab-activity-fields" class="MCXref xref" >AB Activity fields</a> under <a href="#create-a-record" class="MCXref xref" >Create a record</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT Activity]</b>
            </p>
            <p>See field descriptions in <a href="#xt-activity-fields" class="MCXref xref" >XT Activity fields</a> under <a href="#create-a-record" class="MCXref xref" >Create a record</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Other Activity]</b>
            </p>
            <p>Select the field that you want to update a value for, then enter the new value for the field.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer]</b>
            </p>
            <p>See field descriptions in <a href="#offer-fields" class="MCXref xref" >Offer fields</a> under <a href="#create-a-record" class="MCXref xref" >Create a record</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>See field descriptions in <a href="#audience-fields" class="MCXref xref" >Audience fields</a> under <a href="#create-a-record" class="MCXref xref" >Create a record</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
      <td>Enter or map the ID of the record you want to update.</td>
    </tr>
  </tbody>
</table>

### Searches

* [[!UICONTROL Get records]](#get-records)

* [[!UICONTROL Search]](#search)


#### [!UICONTROL Get records]

This search module retrieves a list of records of the selected type.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Target], see <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Create a connection to [!DNL Adobe Target]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>Select the type of record that you want to update.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sort by]</td>
      <td>For each field that you want to sort by, click <b>[!UICONTROL Add item]</b> and select the field and whether the returned results should be ascending or descending.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts At]</td>
      <td>
        <p>Enter the earliest date that you want to retrieve records for. </p>
        <p>For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends At]</td>
      <td>
        <p>Enter the latest date that you want to retrieve records for. </p>
        <p>For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Search]

This search module searches for Activities, Offers, or Audiences based on criteria you specify.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>For instructions on creating a connection to [!DNL Adobe Target], see <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Create a connection to [!DNL Adobe Target]</a> in this article.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Select the type of record that you want to update.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Sort by]</td>
    <td>For each field that you want to sort by, click <b>[!UICONTROL Add item]</b> and select the field and whether the returned results should be ascending or descending.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Search criteria]</td>
    <td>For each rule you want to set up, select the field, the operator, and the value. Click <b>[!UICONTROL Add AND rule]</b> to create additional rules.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>Enter the number of the first response that you want the module to return. The first returned response has an offset of <code>0</code>. Use this field in combination with the [!UICONTROL Maximum number of returned results] field to paginate the responses.</p>
      <p>For example, to see the third page of responses, when each page has ten responses, set [!UICONTROL Offset] to 20 and [!UICONTROL Maximum number of returned] results to 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Maximum number of returned results]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle. Use this field in combination with the [!UICONTROL Offset] field to paginate the responses.</p>
      <p>For example, to see the third page of responses, when each page has ten responses, set [!UICONTROL Offset] to 20 and [!UICONTROL Maximum number of returned] results to 10.</p>
    </td>
  </tr>
</tbody>
</table>
