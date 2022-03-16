---
filename: google-forms-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Forms modules
description: The Google Forms modules allow you to monitor, select, add, update or delete responses on your Google Forms.
---

# Google Forms modules

The Google Forms modules allow you to monitor, select, add, update or delete responses on your Google Forms.

In order to use Google Docs with Adobe Workfront Fusion, it is necessary to have a Google account. If you don't have a Google account yet, you can create one at the Google Account help page.

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

To use Google Forms modules, you must have a Google account.

## Creating a Spreadsheet from the Form

In order to work with your form responses, the spreadsheet from your responses must be created.

1. Open your form.
1. Go to the `Responses`tab.
1. Click the `Create Spreadsheet` icon ![](assets/spreadsheet-icon.png). 

1. Select whether you want to create a new spreadsheet or an existing spreadsheet
1. Click `Create`.

## Google Forms modules and their fields

When you configure Google Forms modules, Workfront Fusion displays the fields listed below. Along with these, additional Google Forms fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers

#### Watch Responses

Watches the form for new responses.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario</a>.</p> </td> 
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
     <li> <p><span class="bold">Formatted value</span><![CDATA[	]]></p> <p>Values are calculated and formatted in the reply according to the cell's formatting. Formatting is based on the spreadsheet's locale, not the requesting user's locale. For example, if <code>A1</code> is <code>1. 23</code> and <code>A2 </code>is <code>=A1</code> and formatted as currency, then <code>A2</code> returns <code>$1. 23</code> .</p> </li> 
     <li> <p><span class="bold">Unformatted value </span> </p> <p>Values are calculated, but not formatted in the reply. For example, if <code>A1</code> is <code>1. 23</code> and <code>A2 </code>is <code>=A1</code> and formatted as currency, then <code>A2</code> returns the number <code>1. 23</code> .</p> </li> 
     <li> <p><span class="bold">Formula </span> </p> <p>Values are not calculated. The reply includes the formulas. For example, if <code>A1</code> is <code>1. 23</code> and <code>A2 </code>is <code>=A1</code> and formatted as currency, then <code>A2</code> returns <code>=A1</code>.</p> </li> 
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

### Actions

* [Add a Response](#add) 
* [Update a Response](#update)

  <!--
  Select Responses
  -->

* [Delete a Response](#delete)

#### Add a Response

This module appends a new response to the bottom of the form's spreadsheet.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Spreadsheet</td> 
   <td> <p>Select the spreadsheet that contains the sheet where you want to add a response.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sheet</td> 
   <td> <p> Select the sheet that contains the form responses.</p> </td> 
  </tr> Values Enter the desired values to the sheet columns. For the Timestamp column in the correct format, use the following value: formatDate(now;DD/MM/YYYY HH:mm;UTC) Value input option Raw The values that the user enters are not parsed and are stored as-is. User entered The values are parsed as if the user typed them into the UI. Numbers remain numbers, but strings may be converted to numbers, dates, or other formats following the same rules that are applied when entering text into a cell via the Google Sheets UI. Insert data option Specify how existing data is changed when new data is input. Overwrite The new data overwrites existing data in the areas where it is written. Adding data to the end of the sheet inserts new rows or columns so the data can be written. Insert rows Rows are inserted for the new data. 
 </tbody> 
</table>

#### Update a Response

This module updates the selected response.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario</a>.</p> </td> 
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
  </tr> Value input option Raw The values that the user enters are not parsed and are stored as-is. User entered The values are parsed as if the user typed them into the UI. Numbers remain numbers, but strings may be converted to numbers, dates, or other formats following the same rules that are applied when entering text into a cell via the Google Sheets UI. 
 </tbody> 
</table>

<!--
Select Responses This module returns response rows that match the criteria specified on a selected worksheet. Connection For instructions about connecting your Google account to Workfront Fusion, see Connect the module's app or web service to Workfront Fusion in the article Create a scenario. File Select the spreadsheet that contains the sheet where you want to update a response. Worksheet Select the sheet that contains the form responses. Row ID Enter or map the ID of the row you want to update. Values Enter the new values to the desired columns. Continue the execution of the route even if the module returns no results Enable this option to ensure that the scenario is not stopped by this module. Filtering Enter or map the filter by which you want to select responses. Maximum number of returned rows Set the maximum number of responses that Workfront Fusion returns during one cycle.
-->

#### Delete a Response

This module deletes a selected response.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario</a>.</p> </td> 
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

### Searches

* [Search Responses](#search) 
* [Search Responses (Advanced)](#search2)

#### Search Responses

This module returns responses matching the given criteria.

<table cellspacing="0">   
 <tbody> Connection For instructions about connecting your Google account to Workfront Fusion, see Connect the module's app or web service to Workfront Fusion in the article Create a scenario. Spreadsheet Select the form you want to search in. Sheet Select the sheet that contains the form responses. Column range Select the column range you want to search. Filter Define the filter you want to search responses responses by. Sort Order Select whether to sort returned responses in ascending or descending order. Order By Select the column you want to order returned responses by. Value Render Option Specify how you want the values to be rendered in the output. Formatted value Values are calculated and formatted in the reply according to the cell's formatting. Formatting is based on the spreadsheet's locale, not the requesting user's locale. For example, if A1 is 1. 23 and A2 is =A1 and formatted as currency, then A2 returns $1. 23 . Unformatted value Values are calculated, but not formatted in the reply. For example, if A1 is 1. 23 and A2 is =A1 and formatted as currency, then A2 returns the number 1. 23 . Formula Values are not calculated. The reply includes the formulas. For example, if A1 is 1. 23 and A2 is =A1 and formatted as currency, then A2 returns =A1. Date and time render option Select how you want dates, times, and duration to be represented in the output. This field is ignored if Value Render Option is set to Formatted Value. 
  <tr> <!--
    Maximum number of returned responses
   --> 
   <td> <p> Set the maximum number of responses that Workfront Fusion returns during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Responses (Advanced)

This module performs a search using the [Google Charts Query Language](https://developers.google.com/chart/interactive/docs/querylanguage). This module does not return a row number.

<table cellspacing="0">   
 <tbody> 
  <tr> <!--
    Connection
   --> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario</a>.</p> </td> 
  </tr> 
  <tr> <!--
    Spreadsheet
   --> 
   <td> <p>Select the spreadsheet that contains the sheet you want to search.</p> </td> 
  </tr> 
  <tr> <!--
    Sheet
   --> 
   <td> <p> Select the sheet that contains the form responses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <p>Define the search query using the <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Google Charts Query Language</a>.</p> <p>Example: <code>select * where C = "John"</code> retrieves all values for the row where the C column is "John".</p> </td> 
  </tr> 
  <tr> <!--
    Maximum number of returned rows
   --> 
   <td> <p> Set the maximum number of responses that Workfront Fusion returns during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

