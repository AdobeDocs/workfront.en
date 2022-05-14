---
filename: google-forms-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Forms modules
description: The Adobe Workfront Fusion Google Forms modules allow you to monitor, select, add, update or delete responses on your Google Forms.
---

# Google Forms modules

The Adobe Workfront Fusion Google Forms modules allow you to monitor, select, add, update or delete responses on your Google Forms.

In order to use Google Docs with Adobe Workfront Fusion, it is necessary to have a Google account. If you don't have a Google account yet, you can create one at the Google Account help page.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
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
    <td>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Google Forms modules, you must have a Google account.

## Creating a Spreadsheet from the Form

In order to work with your form responses, the spreadsheet from your responses must be created.

1. Open your form.
1. Go to the **Responses** tab.
1. Click the **Create Spreadsheet** icon ![](assets/spreadsheet-icon.png). 

1. Select whether you want to create a new spreadsheet or an existing spreadsheet
1. Click **Create**.

## Google Forms modules and their fields

When you configure Google Forms modules, Workfront Fusion displays the fields listed below. Along with these, additional Google Forms fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers {#triggers}

#### Watch Responses

Watches the form for new responses.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Spreadsheet</td> 
   <td> <p>Select the spreadsheet that contains the responses from the form that you want to watch for new responses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sheet</td> 
   <td> <p> Select the sheet that contains the form responses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Row with headers</td> 
   <td>Specify the header row of the table. The default row is <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Value Render Option</td> 
   <td> <p>Specify how you want the values to be rendered in the output.</p> 
    <ul> 
     <li> <p><strong>Formatted value</strong> </p> <p>Values are calculated and formatted in the reply according to the cell's formatting. Formatting is based on the spreadsheet's locale, not the requesting user's locale. For example, if <code>A1</code> is <code>1. 23</code> and <code>A2 </code>is <code>=A1</code> and formatted as currency, then <code>A2</code> returns <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>Unformatted value</strong> </p> <p>Values are calculated, but not formatted in the reply. For example, if <code>A1</code> is <code>1. 23</code> and <code>A2 </code>is <code>=A1</code> and formatted as currency, then <code>A2</code> returns the number <code>1. 23</code> .</p> </li> 
     <li> <p><strong>Formula</strong> </p> <p>Values are not calculated. The reply includes the formulas. For example, if <code>A1</code> is <code>1. 23</code> and <code>A2 </code>is <code>=A1</code> and formatted as currency, then <code>A2</code> returns <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Date and time render option</td> 
   <td>Select how you want dates, times, and duration to be represented in the output. This field is ignored if Value Render Option is set to Formatted Value.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p> Set the maximum number of responses that Workfront Fusion works with during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Add a Response](#add-a-response) 
* [Update a Response](#update-a-response)

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#select-responses" class="MCXref xref">Select Responses</a> </li>
  -->

* [Delete a Response](#delete-a-response)

#### Add a Response {#add-a-response}

This module appends a new response to the bottom of the form's spreadsheet.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Spreadsheet</td> 
   <td> <p>Select the spreadsheet that contains the sheet where you want to add a response.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sheet</td> 
   <td> <p> Select the sheet that contains the form responses.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Values</p> </td> 
   <td> <p>Enter the desired values to the sheet columns.</p> <p>For the Timestamp column in the correct format, use the following value:</p><pre>formatDate(now;DD/MM/YYYY HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Value input option</td> 
   <td> 
    <ul> 
     <li> <p><strong>Raw</strong> </p> <p> The values that the user enters are not parsed and are stored as-is. </p> </li> 
     <li> <p><strong>User entered</strong></p> <p>The values are parsed as if the user typed them into the UI. Numbers remain numbers, but strings may be converted to numbers, dates, or other formats following the same rules that are applied when entering text into a cell via the Google Sheets UI.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Insert data option</td> 
   <td> <p>Specify how existing data is changed when new data is input. </p> 
    <ul> 
     <li> <p><strong>Overwrite</strong> </p> <p>The new data overwrites existing data in the areas where it is written. Adding data to the end of the sheet inserts new rows or columns so the data can be written.</p> </li> 
     <li> <p><strong>Insert rows</strong></p> <p>Rows are inserted for the new data.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a Response {#update-a-response}

This module updates the selected response.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Spreadsheet</td> 
   <td> <p>Select the spreadsheet that contains the sheet where you want to update a response.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sheet</td> 
   <td> <p> Select the sheet that contains the form responses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Row number</p> </td> 
   <td> <p>Enter or map the number of the row you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Values</p> </td> 
   <td> <p>Enter the new values to the desired columns.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Value input option</td> 
   <td> 
    <ul> 
     <li> <p><strong>Raw</strong> </p> <p> The values that the user enters are not parsed and are stored as-is. </p> </li> 
     <li> <p><strong>User entered</strong></p> <p>The values are parsed as if the user typed them into the UI. Numbers remain numbers, but strings may be converted to numbers, dates, or other formats following the same rules that are applied when entering text into a cell via the Google Sheets UI.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h4 id="select-responses"><a name="Select"></a>Select Responses</h4>
<p>This module returns response rows that match the criteria specified on a selected worksheet.</p>
<table>
<col data-mc-conditions="">
<col data-mc-conditions="">
<tbody>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td>
<td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">File</td>
<td> <p>Select the spreadsheet that contains the sheet where you want to update a response.</p> </td>
</tr>
<tr>
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Worksheet</td>
<td> <p> Select the sheet that contains the form responses.</p> </td>
</tr>
<tr>
<td role="rowheader"> <p>Row ID</p> </td>
<td> <p>Enter or map the ID of the row you want to update.</p> </td>
</tr>
<tr>
<td role="rowheader"> <p>Values</p> </td>
<td> <p>Enter the new values to the desired columns.</p> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue the execution of the route even if the module returns no results</td>
<td> <p>Enable this option to ensure that the scenario is not stopped by this module.</p> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Filtering</td>
<td data-mc-conditions="QuicksilverOrClassic.Draft mode">Enter or map the filter by which you want to select responses.</td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Maximum number of returned rows</td>
<td> <p> Set the maximum number of responses that Workfront Fusion returns during one cycle.</p> </td>
</tr>
</tbody>
</table>
</div>
-->

#### Delete a Response {#delete-a-response}

This module deletes a selected response.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Spreadsheet</td> 
   <td> <p>Select the spreadsheet that contains the sheet where you want to delete a response.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sheet</td> 
   <td> <p> Select the sheet that contains the form responses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Row number</p> </td> 
   <td> <p>Enter or map the number of the row you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Searches {#searches}

* [Search Responses](#search-responses) 
* [Search Responses (Advanced)](#search-responses-advanced)

#### Search Responses {#search-responses}

This module returns responses matching the given criteria.

<table> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td>
   --> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Spreadsheet</td>
   --> 
   <td> <p>Select the form you want to search in.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sheet </td>
   --> 
   <td> <p>Select the sheet that contains the form responses.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Column range</td>
   --> 
   <td> <p> Select the column range you want to search.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Filter</td> 
   <td> <p>Define the filter you want to search responses responses by.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sort Order </td>
   --> 
   <td> <p>Select whether to sort returned responses in ascending or descending order.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Order By</td>
   --> 
   <td> <p> Select the column you want to order returned responses by.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Value Render Option</td> 
   <td> <p>Specify how you want the values to be rendered in the output.</p> 
    <ul> 
     <li> <p><strong>Formatted value</strong></p> <p>Values are calculated and formatted in the reply according to the cell's formatting. Formatting is based on the spreadsheet's locale, not the requesting user's locale. For example, if <code>A1</code> is <code>1. 23</code> and <code>A2 </code>is <code>=A1</code> and formatted as currency, then <code>A2</code> returns <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>Unformatted value</strong> </p> <p>Values are calculated, but not formatted in the reply. For example, if <code>A1</code> is <code>1. 23</code> and <code>A2 </code>is <code>=A1</code> and formatted as currency, then <code>A2</code> returns the number <code>1. 23</code> .</p> </li> 
     <li> <p><strong>Formula</strong> </p> <p>Values are not calculated. The reply includes the formulas. For example, if <code>A1</code> is <code>1. 23</code> and <code>A2 </code>is <code>=A1</code> and formatted as currency, then <code>A2</code> returns <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Date and time render option</td>
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select how you want dates, times, and duration to be represented in the output. This field is ignored if Value Render Option is set to Formatted Value. </td>
  -->
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Maximum number of returned responses</td>
   <td> <p> Set the maximum number of responses that Workfront Fusion returns during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Responses (Advanced) {#search-responses-advanced}

This module performs a search using the [Google Charts Query Language](https://developers.google.com/chart/interactive/docs/querylanguage). This module does not return a row number.

<table> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection</td>
   --> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Spreadsheet</td>
   --> 
   <td> <p>Select the spreadsheet that contains the sheet you want to search.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sheet</td>
   --> 
   <td> <p> Select the sheet that contains the form responses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <p>Define the search query using the <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Google Charts Query Language</a>.</p> <p>Example: <code>select * where C = "John"</code> retrieves all values for the row where the C column is "John".</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Maximum number of returned rows</td>
   --> 
   <td> <p> Set the maximum number of responses that Workfront Fusion returns during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

