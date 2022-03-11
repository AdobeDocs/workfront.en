---
filename: airtable-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Airtable modules
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
---

# Airtable modules

`Adobe Workfront Fusion` requires an `Adobe Workfront Fusion` license in addition to an `Adobe Workfront` license.
In a `Adobe Workfront Fusion` scenario, you can connect your `Airtable` account to multiple third-party applications and services.

<!--
For more information, see the tutorial Sync Airtable and Google contacts.
-->

## Connect Airtable to `Workfront Fusion`

<ol> 
 <li value="1">Log in to your Airtable account.</li> 
 <li value="2"> <p>Open your account overview and generate the API key.</p> </li> 
 <li value="3">Open <span>Workfront Fusion</span> and the <span class="bold">Create a connection</span> dialog of the desired module.</li> 
 <li value="4"> <p>Enter the generated API key in the <span class="bold">API</span> token field.</p> <p> <img src="assets/airtable-create-a-connection-350x263.png" style="width: 350;height: 263;"> </p> </li> 
 <li value="5">Click the <span class="bold">Continue</span> button. The connection is now established.</li> 
</ol>

## Airtable modules and their fields

### Records

* [Create a Record](#create) 
* [Delete a Record](#delete) 
* [Get a record](#get) 
* [Search Records](#search) 
* [Update a Record](#update) 
* [Watch Records](#watch2)

#### Create a Record

This action module `creates a new record`.

You specify the data you want in the record and where you want it to be stored.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Airtable</span> account to <span>Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref" data-mc-variable-override="">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Record</p> </td> 
   <td> <p>Enter the values for the new record.</p> <p>For more information on field types, search for "Field types reference" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><span class="bold">Text</span>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><span class="bold">Long text</span>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><span class="bold">Attachment</span> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><span class="bold">Checkbox</span>: Select one of the options.</li> 
     <li><span class="bold">Multiple select</span>: Select multiple options in the checklist.</li> 
     <li><span class="bold">Single select</span>: Select one option from the drop-down menu.</li> 
     <li><span class="bold">Collaborator</span>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><span class="bold">Date</span>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><span class="bold">Emails</span>: A valid email address.</li> 
     <li><span class="bold">URL</span>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><span class="bold">Number</span>: Enter a number.</li> 
     <li><span class="bold">Currency</span>: Currency value.</li> 
     <li><span class="bold">Percent</span>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><span class="bold">Duration</span>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><span class="bold">Rating</span>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><span class="bold">Link</span>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><span class="bold">Rollup</span>: Computed value: COUNT(values)</li> 
     <li><span class="bold">Lookup</span>: Array of long text fields</li> 
     <li><span class="bold">Autonumber</span>: Automatically incremented unique counter for each record.</li> 
     <li> <p><span class="bold">Barcode</span>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Smart links</td> 
   <td> <p><![CDATA[	]]>Enter names instead of record IDs to fields that link to another table. The record is automatically created in the linked table if there is no match.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Record

This action module `deletes a particular record`.

You specify the ID and locates of the record.

The module returns the ID of the  `record` and any associated fields, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Airtable</span> account to <span>Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref" data-mc-variable-override="">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Table </td> 
   <td> <p>Select the table you want to delete the record from.</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID</td> 
   <td> <p><![CDATA[	]]>Enter or map the unique <span>Airtable</span> ID of the <span>record</span> that you want the module to <span>delete</span>. You can retrieve the ID, for example, using the Search Records module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a record

This action module retrieves record details.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Airtable</span> account to <span>Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref" data-mc-variable-override="">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Select the base that contains the table with the record you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td>Table</td> 
   <td> <p> Select the table that contains the record you want to retrieve details for.</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID</td> 
   <td> <p> Enter or map the ID of the record you want to retrieve details for.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Records

This search module looks for `records in an object` in `Airtable` that match the search query you specify.

You can map `this information` in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Airtable</span> account to <span>Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref" data-mc-variable-override="">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Table </td> 
   <td> <p>Select the table you want to search for records.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Formula</p> </td> 
   <td> <p>A formula used to filter records. The formula is evaluated for each record, and if the result is not <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>, or <code>#Error!</code> the record is included in the response.</p> <p>If combined with the <code>view</code>, only records in that view which satisfy the formula are returned.</p> <p>For example, to only include records where Name isn't empty, pass in:<code> NOT({Name} = '')</code></p> <p>To learn more, see the information about formula field references in the Airtable support documentation.</p> </td> 
  </tr> 
  <tr> 
   <td>Sort </td> 
   <td> <p>Select the sorting direction and the field you want to sort the results by.</p> </td> 
  </tr> 
  <tr> 
   <td>View </td> 
   <td> <p>Select the view you want to search for records.</p> </td> 
  </tr> 
  <tr> 
   <td>Max Records</td> 
   <td> <p><![CDATA[	]]>Enter or map the maximum number of <span>record</span>s you want the module to <span>return</span> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a Record

This action module `updates a particular record`.

You specify the ID of the record and the new data you want it to contain.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p style="font-weight: normal;">Establish a connection to your Airtable account. (See <a href="#connecti" class="MCXref xref">Connect Airtable to Workfront Fusion</a>.)</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID </td> 
   <td> <p>Enter or map the unique <span>Airtable</span> ID of the <span>record</span> that you want the module to <span>update</span>. You can retrieve the ID, for example, using the Search Records module.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Record</p> </td> 
   <td> <p>Enter the values for the new record.</p> <p>In order to delete the content of the field, use the erase function. </p> <!--
     screenshot
    --> <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><span class="bold">Text</span>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><span class="bold">Long text</span>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><span class="bold">Attachment</span>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><span class="bold">Checkbox</span>: Select one of the options.</li> 
     <li><span class="bold">Multiple select</span>: Select multiple options in the checklist.</li> 
     <li><span class="bold">Single select</span>: Select one option from the drop-down menu.</li> 
     <li><span class="bold">Collaborator</span>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><span class="bold">Date</span>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><span class="bold">Phone number</span>: A telephone number, for example, (415) 555-9876.</li> 
     <li><span class="bold">Email</span>: A valid email address.</li> 
     <li><span class="bold">URL</span>: A valid URL such as airtable.com or https://airtable.com/universe.</li> 
     <li><span class="bold">Number</span>: Enter a number.</li> 
     <li><span class="bold">Currency</span>: Currency value.</li> 
     <li><span class="bold">Percent</span>: A percentage value; must be equal to or more than 0.</li> 
     <li><span class="bold">Duration</span>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><span class="bold">Rating</span>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><span class="bold">Link</span>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><span class="bold">Rollup</span>: Computed value: COUNT(values)</li> 
     <li><span class="bold">Lookup</span>: Array of long text fields</li> 
     <li><span class="bold">Autonumber</span>: Automatically incremented unique counter for each record.</li> 
     <li> <p><span class="bold">Barcode</span>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Smart links</td> 
   <td> <p><![CDATA[	]]>Enter names instead of record IDs to fields that link to another table. The record is automatically created in the linked table if there is no match.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Records

This trigger module executes a scenario when `a new record is added or updated in the table`. The module `returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses`. You can map `this information` in subsequent modules in the scenario.

>[!NOTE]
>
>In order to use this module, the Created Time field must be created in your table.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Airtable</span> account to <span>Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref" data-mc-variable-override="">Connect Airtable to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Table </td> 
   <td> <p>Select the table you want to watch for new records.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Trigger configuration</p> </td> 
   <td> <p style="font-weight: bold;">Trigger field</p> <p>A <code>Created Time</code> field that is used to sort records. If you do not have a <code>Created Time</code> field in your schema, you need to create one. </p> <p style="font-weight: bold;">Label field</p> <p>A field that is used as a label for a record, for example, in the Choose where to start dialog.</p> </td> 
  </tr> 
  <tr> 
   <td> <p style="font-weight: bold;">Formula</p> </td> 
   <td> <p>A formula used to filter records. The formula is evaluated for each record, and if the result is not <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>, or <code>#Error!</code> the record is included in the response.</p> <p>If combined with the <code>view</code>, only records in that view which satisfy the formula are returned.</p> <p>For example, to only include records where Name isn't empty, pass in:<code> NOT({Name} = '')</code></p> <p>To learn more, see the information about formula field references in the Airtable support documentation.</p> </td> 
  </tr> 
  <tr> 
   <td>Max Records</td> 
   <td> <p>Enter or map the maximum number of <span>record</span>s you want the module to <span>watch</span> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Responses

This trigger module starts a scenario when a form is submitted.

>[!NOTE]
>
>This functionality is available only for paid Airtable Pro Plan only.

The webhook URL needs to be generated in Workfront Fusion and then added to form configuration in Airtable.

1. Add the Watch New Responses module to your Workfront Fusion scenario.
1. Generate and copy the webhook URL.

   For instructions, see [Instant triggers (webhooks)](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. Log in to your Airtable account.
1. Open the Base and the table you want to use for the form and create a Form view.
1. Set the form as needed, scroll down the form, and enable the Redirect to URL after the form is submitted option.
1. Enter the Webhook URL generated in step 2 to the displayed dialog box and add the ?record_id={record_id} just after the webhook URL to include the Record ID in the module's output, then click Save. The resulting URL will, for example, look like this:
1. Go back to your Workfront Fusion scenario and run the Watch Responses module only to load fields from Airtable and to be able to map those fields into the other modules.
1. Submit the form in Airtable where the Redirect to URL after the form is submitted option is enabled and Webhook URL added (step 6 above).

   The Watch Responses module is triggered and the desired data are loaded.

1. Add the Airtable > Get a Record module just after the Airtable > Watch Responses module and map the record_id to the Record ID field.

Now, every time the form is submitted, the Watch Responses module in your Workfront Fusion scenario is triggered, and the Get a Record module returns the submitted form details.
