---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Sheets modules
description: In order to use [!DNL Google Sheets] with [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] extension (optional, but required for instant triggers).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
---
# [!DNL Google Sheets] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Google Sheets], as well as connect it to multiple third-party applications and services.

For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see [Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

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
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisites

To use [!UICONTROL Google Sheets] modules, you must have a [!UICONTROL Google] account.

## Google Sheets API information

The Google Sheets connector uses the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Base URL</td> 
   <td> https://sheets.googleapis.com/v4</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API version</td> 
   <td> v4 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API tag</td> 
   <td>v2.5.7</td> 
  </tr>
 </tbody> 
 </table>

## Triggers

### [!UICONTROL Watch Rows]

Retrieves values from every newly added row in the spreadsheet.

The module retrieves only new rows that have not been filled in before. The trigger will not process an overwritten row.

>[!IMPORTANT]
>
>If the worksheet contains a blank row, no rows after the blank row will be processed.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the spreadsheet that contains the sheet you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet] </td> 
   <td> <p>Select the sheet you want to watch for a new row.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table contains headers]</td> 
   <td> <p> Select whether the spreadsheet contains the header row.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>The module doesn't retrieve the header row as output data. </p> <p>Variable names in the output are called by the headers.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>The module also retrieves the first table row</p> <p>Variable names in the output are called A, B, C, D, and so on.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row with headers] </td> 
   <td> <p>Enter the range of the header row. For example, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL First table row]</td> 
   <td> <p>Enter the range of the first row of the table. For example, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Value render option]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>The values will be calculated and formatted in the reply according to the cell's formatting. Formatting is based on the spreadsheet's locale, not the requesting user's locale. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Unformatted value]</p> <p>The values will be calculated, but not formatted in the reply. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return the number <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>The values will not be calculated. The reply will include the formulas. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Date and time render option]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Serial number]</p> <p>Instructs date, time, datetime, and duration fields to be outputted as doubles in "serial number" format, as popularized by Lotus 1-2-3. The whole number portion of the value (left of the decimal) counts the days since December 30th 1899. The fractional portion (right of the decimal) counts the time as a fraction of the day. For example, January 1st 1900 at noon would be 2.5, 2 because it's 2 days after December 30th 1899, and .5 because noon is half a day. February 1st 1900 at 3pm would be 33.625. This correctly treats the year 1900 as not a leap year.</p> <p style="font-weight: bold;">[!UICONTROL Formatted string]</p> <p>Instructs date, time, datetime, and duration fields to be outputted as strings in their given number format (which is dependent on the spreadsheet's locale).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of results that [!DNL Workfront Fusion] will work with during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Actions

* [[!UICONTROL Add a Row]](#add-a-row)
* [[!UICONTROL Update a Row]](#update-a-row)
* [[!UICONTROL Clear a Row]](#clear-a-row)
* [[!UICONTROL Delete a Row]](#delete-a-row)
* [[!UICONTROL Get a Cell]](#get-a-cell)
* [[!UICONTROL Update a Cell]](#update-a-cell)
* [[!UICONTROL Clear a Cell]](#clear-a-cell)
* [[!UICONTROL Add a Sheet]](#add-a-sheet)
* [[!UICONTROL Create a Spreadsheet]](#create-a-spreadsheet)
* [[!UICONTROL Delete a Sheet]](#delete-a-sheet)
* [[!UICONTROL Make an API Call]](#make-an-api-call)

### [!UICONTROL Add a Row] 

This module appends adds a row to a sheet.

When you configure [!DNL Google Sheets] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Google Sheets] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Select whether you want to select the spreadsheet and sheet manually or by mapping.</p> <p>Note: Manual mapping is useful, for example, when a new spreadsheet is created in an [!DNL Workfront Fusion] scenario and you want to add data in the newly created spreadsheet directly in the scenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Select the sheet you want to add a row to.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Column Range]</td> 
   <td>Select the column range you want to work with.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p> Select whether the spreadsheet contains the header row.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>The module doesn't retrieve the header row as output data. </p> <p>Variable names in the output are called by the headers.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>The module also retrieves the first table row</p> <p>Variable names in the output are called A, B, C, D, and so on.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Enter or map the desired cells of the row you want to add.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>The values are parsed as if the user typed them into the UI. Numbers remain numbers, but strings may be converted to numbers, dates, or other formats following the same rules that are applied when entering text into a cell via the [!DNL Google Sheets] UI.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> The values that the user enters are not parsed and are stored as-is. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insert data option]</td> 
   <td> <p>Specify how existing data is changed when new data is input. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Insert rows]</strong></p> <p>Rows are inserted for the new data.</p> </li> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>The new data overwrites existing data in the areas where it is written. Adding data to the end of the sheet inserts new rows or columns so the data can be written.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a Row]

This module allows you to change the cell content in a selected row.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Select whether you want to select the spreadsheet and sheet manually or by mapping.</p> <p>Note: Manual mapping is useful, for example, when a new spreadsheet is created in the [!UICONTROL Workfront Fusion] scenario and you want to add data to the newly created spreadsheet directly in the scenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Select the sheet you want to update a row in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Row number]</td> 
   <td> <p> Enter the number of the row you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p> Select whether the spreadsheet contains the header row.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>The module doesn't retrieve the header row as output data. </p> <p>Variable names in the output are called by the headers.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>The module also retrieves the first table row</p> <p>Variable names in the output are called A, B, C, D, and so on.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Enter or map the values to the desired cells of the row you want to change (update).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>The values are parsed as if the user typed them into the UI. Numbers remain numbers, but strings may be converted to numbers, dates, or other formats following the same rules that are applied when entering text into a cell via the [!DNL Google Sheets] UI.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> The values that the user enters are not parsed and are stored as-is. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Clear a Row]

Deletes values from a specified row.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the [!DNL Google] spreadsheet that contains the sheet you want to clear a row from.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p> Select the sheet you want to clear data from.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Row number]</td> 
   <td> <p>Enter the number of the row you want to clear data from. For example, <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a Row]

Deletes a specified row.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the Google spreadsheet that contains the sheet you want to delete a row from.</p> </td> 
  </tr> 
  <tr> 
   <td>Sheet </td> 
   <td> <p>Select the sheet you want to delete a row from.</p> </td> 
  </tr> 
  <tr> 
   <td>Row number</td> 
   <td> <p>Enter the number of the row you want to delete. Example: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Get a Cell]

Retrieves a value from a selected cell.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Select the sheet that contains the cell you want to retrieve data from.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Enter the ID of the cell you want to retrieve data from. Example: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>The values will be calculated and formatted in the reply according to the cell's formatting. Formatting is based on the spreadsheet's locale, not the requesting user's locale. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>The values will be calculated, but not formatted in the reply. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return the number <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>The values will not be calculated. The reply will include the formulas. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>Instructs date, time, datetime, and duration fields to be outputted as doubles in "serial number" format, as popularized by Lotus 1-2-3. The whole number portion of the value (left of the decimal) counts the days since December 30th 1899. The fractional portion (right of the decimal) counts the time as a fraction of the day. For example, January 1st 1900 at noon would be 2.5, 2 because it's 2 days after December 30th 1899, and .5 because noon is half a day. February 1st 1900 at 3pm would be 33.625. This correctly treats the year 1900 as not a leap year.</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>Instructs date, time, datetime, and duration fields to be outputted as strings in their given number format (which is dependent on the spreadsheet's locale).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a Cell]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Enter the ID of the cell you want to update. Example: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td> <p>Enter the new value for the cell.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>The values are parsed as if the user typed them into the UI. Numbers remain numbers, but strings may be converted to numbers, dates, or other formats following the same rules that are applied when entering text into a cell via the [!DNL Google Sheets] UI.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> The values that the user enters are not parsed and are stored as-is. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Clear a Cell]

Deletes a value from a specified cell.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the Google spreadsheet that contains the sheet that you want to clear a cell from.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Select the sheet you want to clear a cell from.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Enter the ID of the cell you want to clear. Example: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Add a Sheet]

Creates a new sheet in a selected spreadsheet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the Google spreadsheet where you want to add a sheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Properties]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL Title]</p> <p>Enter the name of the new sheet.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Index]</p> <p>Enter the sheet position. The default is 0 (places the sheet in the first place)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create a Spreadsheet]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Enter the name of a new spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Locale]</td> 
   <td> <p>Enter the locale of the spreadsheet in one of the following formats:</p> 
    <ul> 
     <li>an ISO 639-1 language code such as <code>en</code></li> 
     <li>an ISO 639-2 language code such as <code>haw</code>, if no 639-1 code exists</li> 
     <li>a combination of the ISO language code and country code, such as <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recalculation interval]</td> 
   <td> <p>The amount of time to wait before volatile functions are recalculated:</p> <p style="font-weight: bold;">[!UICONTROL On change]</p> <p>Volatile functions are updated upon every change.</p> <p style="font-weight: bold;">[!UICONTROL On change and every minute]</p> <p>Volatile functions are updated upon every change and every minute.</p> <p style="font-weight: bold;">[!UICONTROL On change and hourly]</p> <p>Volatile functions are updated upon every change and hourly.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time zone]</td> 
   <td> <p> Select the time zone of the spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Number format]</td> 
   <td> <p>Select the default format of all cells in the spreadsheet.</p> <p><strong>[!UICONTROL Text]</strong>: Text formatting. Example: <code>1000. 12</code></p> <p><strong>[!UICONTROL Number]</strong>: Number formatting. Example: <code>1,000.12</code></p> <p><strong>[!UICONTROL Percent]</strong>: Percent formatting. Example: <code>10. 12%</code></p> <p><strong>[!UICONTROL Currency]</strong>: Currency formatting. Example: <code>$1,000.12</code></p> <p><strong>[!UICONTROL Date]</strong>: Date formatting. Example: <code>9/26/2008</code></p> <p><strong>[!UICONTROL Time]</strong>: Time formatting. Example: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL Date time]</strong>: Date and Time formatting. Example: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Scientific]</strong>Scientific number formatting. Example: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheets] </td> 
   <td> <p>Click <strong>[!UICONTROL Add]</strong> to add a sheet to the spreadsheet. For each sheet, enter or map a title for the sheet and the sheet's index. An index of 0 represents the first sheet.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a Sheet]

Deletes a specific sheet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Select the sheet you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Make an API Call] 

This action module allows you to perform a custom API call.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [Fusion App] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Enter a path relative to <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Add the query for the API call in the form of a standard JSON object.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:   <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Searches

* [[!UICONTROL Search Rows]](#search-rows)
* [[!UICONTROL Search Rows (Advanced)]](#search-rows-advanced)
* [[!UICONTROL Get Range Values]](#get-range-values)
* [[!UICONTROL List Sheets]](#list-sheets)

### [!UICONTROL Search Rows]

Searches rows using the filter options.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [Fusion App] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Select the sheet you want to search the rows in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p> Select whether the spreadsheet contains the header row. If the [!UICONTROL Yes] option is selected, the module doesn't retrieve the header row as output data and variable names in the output are then called by the headers. If the [!UICONTROL No] option is selected, then the module also retrieves the first table row and variable names in the output are then called just A, B, C, D, and so on.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Column range]</td> 
   <td>Select the column range to work with. Example: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Set the filter for the row to be searched by.</p> <p>For more information about filters, see <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Add a filter to a scenario in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort order]</td> 
   <td>Select whether you want to sort ascending or descending.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td>Choose the column that you want to sort by.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>The values will be calculated and formatted in the reply according to the cell's formatting. Formatting is based on the spreadsheet's locale, not the requesting user's locale. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Unformatted value]</p> <p>The values will be calculated, but not formatted in the reply. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return the number <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>The values will not be calculated. The reply will include the formulas. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Serial number]</p> <p>Instructs date, time, datetime, and duration fields to be output as doubles in "serial number" format, as popularized by Lotus 1-2-3. The whole number portion of the value (left of the decimal) counts the days since December 30th 1899. The fractional portion (right of the decimal) counts the time as a fraction of the day. For example, January 1st 1900 at noon would be 2.5, 2 because it's 2 days after December 30th 1899, and .5 because noon is half a day. February 1st 1900 at 3pm would be 33.625. This correctly treats the year 1900 as not a leap year.</p> <p style="font-weight: bold;">[!UICONTROL Formatted string]</p> <p>Instructs date, time, datetime, and duration fields to be outputted as strings in their given number format (which is dependent on the spreadsheet's locale).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned rows]</td> 
   <td>Set the maximum number of rows that [!DNL Workfront Fusion] will return during one execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Search Rows (Advanced)]

Returns results matching the given criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the Google spreadsheet that contains the sheet you want to search..</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Select the sheet that contains the rows you want to search.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Use the [!DNL Google Charts Query Language]. Example: <code>select * where B = "John"</code></p> <p>For more information on [!DNL Google Charts Query Language], see <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Query Language Reference</a> in the [!DNL Google] documentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Get Range Values]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Select the sheet you want to get the range content from.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Range] </td> 
   <td> <p>Enter the range you want to get. Example: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p>Check this box if the sheet has a header row</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Row with headers]</td> 
   <td>Enter the range of the table headers. Example <code>A1:F1</code>. If you leave the field empty, [!DNL Workfront Fusion] will suppose that the header is in the first row of the specified range.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>The values will be calculated and formatted in the reply according to the cell's formatting. Formatting is based on the spreadsheet's locale, not the requesting user's locale. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Unformatted value]</p> <p>The values will be calculated, but not formatted in the reply. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return the number <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>The values will not be calculated. The reply will include the formulas. For example, if <code>A1</code> is <code>1.23</code> and <code>A2</code> is <code>=A1</code> and formatted as currency, then <code>A2</code> would return <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Serial number]</p> <p>Instructs date, time, datetime, and duration fields to be output as doubles in "serial number" format, as popularized by Lotus 1-2-3. The whole number portion of the value (left of the decimal) counts the days since December 30th 1899. The fractional portion (right of the decimal) counts the time as a fraction of the day. For example, January 1st 1900 at noon would be 2.5, 2 because it's 2 days after December 30th 1899, and .5 because noon is half a day. February 1st 1900 at 3pm would be 33.625. This correctly treats the year 1900 as not a leap year.</p> <p style="font-weight: bold;">[!UICONTROL Formatted string]</p> <p>Instructs date, time, datetime, and duration fields to be outputted as strings in their given number format (which is dependent on the spreadsheet's locale).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL List Sheets] 

This module returns a list of all sheets in a spreadsheet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google Sheets] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Select the [!DNL Google] spreadsheet that contains the sheets you want to list.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Usage Limits

If the error `429: RESOURCE_EXHAUSTED` occurs, you have exceeded the API rate limit.

The [!DNL Google Sheets] API has a limit of 500 requests per 100 seconds per project, and 100 requests per 100 seconds per user. Limits for reads and writes are tracked separately. There is no daily usage limit.

See more details at [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## Tips & Tricks

* [How to get Empty Cells from a [!DNL Google] Sheet](#how-to-get-empty-cells-from-a-google-sheet)
* [Add a button in a sheet to run a scenario](#add-a-button-in-a-sheet-to-run-a-scenario)

### How to get Empty Cells from a [!DNL Google Sheet] 

Use the [!UICONTROL Search Rows (Advanced)] module & use this formula to get the columns which are empty.
<pre>select * where E is null</pre>Here "E" is the column &amp; "is null" is the condition. You can create a more advanced query using [Google Query Lang](https://developers.google.com/chart/interactive/docs/querylanguage).

### Add a button in a sheet to run a scenario

1. In [!DNL Workfront Fusion], insert the **[!UICONTROL Webhook]** > **[!UICONTROL Custom webhooks]** module/trigger in the scenario and configure it (see [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)).

1. Copy the webhook's URL.
1. Execute the scenario.
1. In Google Sheets, choose **[!UICONTROL Insert]** > **[!UICONTROL Drawing]**... from the main menu bar.

1. In the [!UICONTROL Drawing] window, Click the **[!UICONTROL Text box]** icon ![](assets/text-box.png) near the top of the window.
1. Design a button and click the **[!UICONTROL Save and Close]** button in the top-right corner:
1. The button will be placed in your worksheet. Click the three vertical dots in the button's top-right corner:
1. Choose **[!UICONTROL Assign script..].** from the menu.
1. Enter the name of your script (function), e.g. `runScenario` and click **[!UICONTROL OK]**:
1. Choose **[!UICONTROL Tools]** > **[!UICONTROL Script editor]** from the main menu bar.

1. Insert the following code:

   * The name of the function must correspond to the name you specified in step 9.
   * Replace the URL with the webhook's URL you copied in step 2.

      <pre>function runScenario() {</pre><pre>UrlFetchApp.fetch("&lt;webhook you copied>");</pre><pre>}</pre>

1. Press **[!UICONTROL Ctrl+S]** to save the script file, enter a project name and click **[!UICONTROL OK]**.

1. Switch back to [!DNL Google Sheets] and click your new button.
1. Grant the required authorization to the script:
1. In [!DNL Workfront Fusion], verify that the scenario has successfully executed.

## Storing dates in a spreadsheet

If you store a Date value in a spreadsheet without any formatting, it will appear in the spreadsheet as text in ISO 8601 format. However, [!DNL Google Sheets] formulas or functions that work with dates that do not understand this text (Example: formula `=A1+10`) will display the following error:

![](assets/mceclip6-350x87.png)

To help allow [!DNL Google Sheets] to understand the date, format it with the [[!UICONTROL formatDate] (date; format; [timezone])](../../workfront-fusion/functions/date-and-time-functions.md#formatda) function. The correct format passed to the function as the second argument depends on the spreadsheet's locale settings.

To determine the correct format:

1. Choose **[!UICONTROL File]** > **[!UICONTROL Spreadsheet]** settings from the main menu to verify/set the locale.

1. Once you have verified/set the proper locale, determine the corresponding date and time format by choosing **[!UICONTROL Format]** > **[!UICONTROL Number]** from the main menu. The format is displayed next to the Date time menu item:

1. To compose the correct format that should be passed to the [!UICONTROL formatDate()] function, refer to the list of [Tokens for date and time formatting in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**Example:** The use of `MM/DD/YYYY HH:mm:ss` format for the United States locale:

![](assets/locale-time-350x83.png)

## Exploiting [!DNL Google Sheets] functions

If you miss a built-in function, but it is featured by [!DNL Google Sheets], you may exploit it. For more information, see [Use [!DNL Google Sheets] functions](../../workfront-fusion/functions/map-using-functions.md#exploiti) in [Map items using functions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## Keep [!DNL Google Sheets] from changing numbers into dates

You might find that a string of numbers that you are using as text is being interpreted as a date in a [!DNL Google] worksheet. For example, you type 1-2019, intending it as text, but Google interprets it as a date. You can pre-format the number as plain text to prevent this.

1. In [!DNL Google Sheets], highlight the column or cell containing the number or numbers.
1. Click **[!UICONTROL Format]** > **[!UICONTROL Number]** > **[!UICONTROL Plain text]**.

Another workaround in [!DNL Workfront Fusion] is to type an apostrophe (') before a number, for example, '1-2019 or '1/47. The apostrophe does not display in the cell after the data is sent from [!DNL Workfront Fusion].
