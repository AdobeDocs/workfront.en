---
filename: map-using-functions
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Map items using functions
description: When you map items, you can use functions to create simple or complex formulas.
---

# Map items using functions

When you map items, you can use functions to create simple or complex formulas.

The functions available in `Adobe Workfront Fusion` are similar to functions in Excel and in some programming languages. They evaluate general logic, math, text, dates, and arrays. They let you perform conditional logic and transformations of item values, such as converting a text to uppercase, trimming text, converting a date into a different format, and more. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Insert functions into fields

If you click a field, the mapping panel displays. The mapping panel contains several tabs:

![](assets/functions-toolbar-350x189.png)

The first tab ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (shown upon opening the panel) displays the items that you can map from other modules.

The other tabs contain the following types of functions:

<ul> 
 <li><span class="bold">General functions</span> <img src="assets/toolbar-icon-general-function.png"> - See <a href="../../workfront-fusion/functions/general-functions.md" class="MCXref xref">General functions</a> for more information.</li> 
 <li><span class="bold">Math functions</span> <img src="assets/toolbar-icon-math-functions.png"> - See <a href="../../workfront-fusion/functions/math-functions.md" class="MCXref xref">Math functions</a> for more information.</li> 
 <li><span class="bold">Text and binary functions</span> <img src="assets/toolbar-icon-text&binary-functions.png"> - See <a href="../../workfront-fusion/functions/string-functions.md" class="MCXref xref">String functions</a> for more information.</li> 
 <li><span class="bold">Date and time</span> <img src="assets/toolbar-icon-date&time-functions.png"> - See <a href="../../workfront-fusion/functions/date-and-time-functions.md" class="MCXref xref">Date and time functions</a> and the articles below for more information.
  <ul>
   <li><a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Tokens for date and time formatting</a></li>
   <li><a href="../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md" class="MCXref xref">Tokens for date and time parsing</a></li>
  </ul></li> 
 <li><span class="bold">Functions for working with arrays</span> <img src="assets/toolbar-icon-functions-for-arrays.png"> - See <a href="../../workfront-fusion/functions/array-functions.md" class="MCXref xref">Array functions</a> for more information.</li> 
</ul>

To insert a function into a field:

1. Click the function name.

   Or

   Drag the function into the field.

` `**Example: **`` Some data types prevent users from entering more than a certain number of characters. You can use the substring function to limit a value to a certain number of characters.

In this example, the substring function limits project name to 50 characters.

![](assets/example-meet-length-restriction-350x184.png)

## Nesting functions

You can nest functions within each other to create limitless possibilities.

## Use Google Sheets functions

If Workfront Fusion does not feature a function you want to use, but it is featured by Google Sheets, you can use it by following these steps:

<ol> 
 <li value="1">In Google Sheets, create a new empty spreadsheet.</li> 
 <li value="2">In <span>Workfront Fusion</span>, open your scenario.</li> 
 <li value="3"> <p>Add the <span class="bold">Google Sheets </span>><span class="bold"> Update a cell</span> module to the scenario.</p> <p>For instructions on adding a module, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#add" class="MCXref xref">Add a module in a scenario</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario</a>.</p> </li> 
 <li value="4"> <p>Configure the module:<br></p> 
  <ol> 
   <li value="1">Choose the newly created spreadsheet in the <span class="bold">Spreadsheet</span> field.</li> 
   <li value="2"> <p>Insert your formula containing the Google Sheets function(s) into the <span class="bold">Value</span> field. </p> <p>You can use the output of preceding modules as usual.</p> <p> <img src="assets/exploit-google-sheet-functions-350x218.png" style="width: 350;height: 218;"> </p> </li> 
  </ol> </li> 
 <li value="5">Insert the <span class="bold">Google Sheets > Get a cell</span> module to obtain the calculated result.</li> 
 <li value="6"> <p>Configure the module, using the same Cell ID that you used in step 4.</p> <p> <img src="assets/exploit-google-sheet-functions-2-350x187.png" style="width: 350;height: 187;"> </p> </li> 
</ol>

