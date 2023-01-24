---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Tools
description: The [!DNL Adobe Workfront Fusion Tools] section includes several useful modules that can enhance your scenario.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
---
# [!UICONTROL Tools]

The [!DNL Adobe Workfront Fusion Tools] section includes several useful modules that can enhance your scenario.

[!UICONTROL Tools] modules are available from the list of apps, or from the [!UICONTROL Tools] icon ![](assets/tools-icon-small.png) at the bottom of the screen.

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

## [!UICONTROL Tools] and their fields

* [Triggers](#triggers)
* [Actions](#actions)
* [Aggregators](#aggregators)
* [Transformers](#transformers)

### Triggers

#### [!UICONTROL Basic trigger]

This module allows you to create a custom trigger and define its input bundles.

You can use this module, for example, for contacts or any other list that is scheduled to be sent to a specified email address (such as [!UICONTROL Email] >[!UICONTROL Send an Email], or [!DNL Gmail] >[!UICONTROL Send an Email] modules), or as a simple reminder to be triggered whenever you want.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>Create custom bundles by adding array items. The array consists of the name - value pairs.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Get Multiple Variables]](#get-multiple-variables)
* [[!UICONTROL Get Variable]](#get-variable)
* [[!UICONTROL Increment function]](#increment-function)
* [[!UICONTROL Set Multiple Variables]](#set-multiple-variables)
* [[!UICONTROL Set Variable]](#set-variable)
* [[!UICONTROL Sleep]](#sleep)

#### [!UICONTROL Get Multiple Variables]

This module retrieves values that were previously created by the [!UICONTROL Set Variable] or [!UICONTROL Set Multiple Variables] module.

This module can read variables that were set anywhere in the scenario, even if the variable was set in a different route than where the [!UICONTROL Get Multiple Variables] module is located. The only requirement is that the [!UICONTROL Tools] > [!UICONTROL Set Variable] or [!UICONTROL Tools] > [!UICONTROL Set Multiple Variable] module is executed before the [!UICONTROL Tools] > [!UICONTROL Get Multiple Variables] module. For more information on the order in which modules are executed, see [Router module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variables]</td>
        <td>Add the variables that you want the module to get.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Variable name]</td>
        <td>For each variable you add, map the name of the variable you want to get.</td>
    </tr>
</table>

>[!INFO]
>
>**Examples:**  The following are possible uses of the [!UICONTROL Set]/[!UICONTROL Get (multiple) variable(s)] modules:
>
>* To store a calculated value for later use, even in a different route. This is useful in cases when the value is used in multiple modules and the formula to calculate the value is overly complex.
>* To debug a formula. If a formula used in a module does not seemingly provide a correct result, copy the formula and paste it into a [!UICONTROL Set Variable] module that you insert before the relevant module. Disconnect the module(s) after the [!UICONTROL Set Variable] module and execute the scenario. Verify the [!UICONTROL Set Variable] module's output, adjust or simplify the formula, execute the scenario again, and continue to do so until the issue has been resolved.


#### [!UICONTROL Get Variable]

This module retrieves a value that was previously created by the [!UICONTROL Set Variable] or [!UICONTROL Set Multiple Variables] module.

This module can read variables that were set anywhere in the scenario, even if the variable was set in a different route than where the [!UICONTROL Get Variable] module is located. The only requirement is that the [!UICONTROL Tools] > [!UICONTROL Set Variable] or [!UICONTROL Tools] > [!UICONTROL Set Multiple Variables] module is executed before the [!UICONTROL Tools] > [!UICONTROL Get Variable] module. For more information on the order in which modules are executed, see [Router module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable name]</td> 
   <td> <p>Map the name of the variable that you want the module to get.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Increment function]

This module returns a value incremented by 1 after each module's operation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reset a value]</td> 
   <td> <p>Select when you want the module to increment the value. </p> 
    <ul> 
     <li>[!UICONTROL After one cycle]</li> 
     <li>[!UICONTROL After one scenario run]</li> 
     <li>[!UICONTROL Never]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Example:**
>
>One of the module's uses is to implement a "round robin" assignment of tasks, leads, emails, and so on, to users in a group. The algorithm chooses the assignees from a group in some rational order, usually going from the top to the bottom of a list. When the algorithm reaches the end of the list, it would then give the next assignment to the user at the top of the list and continue to make assignments down the list.
>
>The following scenario sends an email to the first recipient after every odd-numbered scenario run, and to the second recipient after every even-numbered scenario run.
>
>![](assets/example-email-350x246.gif)
>
>1. To create this scenario:
>1. Set the module's **[!UICONTROL Reset a value]** field to Never.
>1. Set the route for odd values. Set the filter for this route using the modulus math function that equals `1`:
>
>   ![](assets/odd-350x459.png)
>
>  **Note**: Do not forget to change the [!UICONTROL Equal to] operator from the default [!UICONTROL Text] operator to the [!UICONTROL Numeric] operator.
>
>1. Set the route for even values using the modulus math function that equals `0`:
>
>The increment function adds one every time the scenario runs. The filters check the increment and act on its value, ensuring that the emails are evenly distributed.

#### [!UICONTROL Set Multiple Variables]

This module creates variables that can be mapped by other modules in the route. The variable can also be mapped to the [!UICONTROL Get Variable] or [!UICONTROL Get Multiple Variables] modules for any route in the scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variables]</td> 
   <td>Add the variables that you want the module to set.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>For each variable, enter the variable name. This name will be displayed when mapping the variable in other modules. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>For each variable, enter the value for the variable. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable lifetime] </td> 
   <td> <p>Select how long you want the variables to remain valid (keep the same value).</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>: The variable is valid for one cycle. Useful when multiple webhooks in one scenario run are received (more webhooks = more cycles). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: The variable is valid for one scenario execution. One execution can contain one or more cycles.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Set Variable]

This module creates a variable that can be mapped by other modules in the route. The variable can also be mapped to the [!UICONTROL Get Variable] or [!UICONTROL Get Multiple Variables] modules for any route in the scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>Enter the variable name. This name will be displayed when mapping the variable in other modules. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable lifetime] </td> 
   <td> <p>Select how long you want the variables to remain valid (keep the same value).</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>: The variable is valid for one cycle. Useful when multiple webhooks in one scenario run are received (more webhooks = more cycles). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: The variable is valid for one scenario execution. One execution can contain one or more cycles.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>Enter or map the value for the variable. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sleep]

This module allows you to delay the scenario flow for up to 300 seconds (5 minutes).

This function can be useful, for example, if you want to lower the [!DNL target] service server load or to imitate human behavior when sending bulk SMS or emails.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Delay]</p> </td> 
   <td> <p>Enter the number of seconds the scenario will be paused for.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>If you want to pause the flow for longer periods of time, we suggest to split your scenario into two scenarios:
>
>* The first scenario would contain the part before the pause.
>* The second scenario would contain the part after it.
>
>The first scenario would end up with storing all the necessary information in a data store together with the current timestamp. The second scenario would periodically check the data store for records with a timestamp older than the intended delay, retrieve the records, finalize the processing of the data and remove the records from the data store.
>
>For more information on data stores, see [Data Stores in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>For more information on specific data store modules, see [[!UICONTROL Data store] modules](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Aggregators 

* [[!UICONTROL Numeric aggregator]](#numeric-aggregator)
* [[!UICONTROL Table aggregator]](#table-aggregator)
* [[!UICONTROL Text aggregator]](#text-aggregator)

#### [!UICONTROL Numeric aggregator]

This module allows you to retrieve numerical values, then apply one of the selected functions (SUM, AVG, COUNT, MAX, MIN), and return the result in one bundle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Select the module you want to aggregate fields from.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Aggregate function]</p> </td> 
   <td> <p>Select the function that you want to use to aggregate the values.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Define an expression that you want to group the aggregated output by. This expression can contain one or more mapped items. The aggregated data is then separated into groups using this expression's value. Each group outputs as a separate bundle with a key (the evaluated expression) and a value (the aggregated value). You can use the key as a filter in subsequent modules.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Enable this option to stop the scenario when there are no results.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Value]</p> </td> 
   <td> <p>Enter or map the value that you want to aggregate.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Table aggregator]

This module merges values from the selected fields of received bundles into a single bundle using a specified column and row separator (which allows you to create a table).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Select the module you want to aggregate fields from.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td> <p> Select the fields from the module selected above that contain values you want to aggregate into the one bundle.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Column separator]</p> </td> 
   <td> <p>Select or enter the type of separator that will separate the field value columns in the resulting bundle. If you select [!UICONTROL Other], enter the character you want to use to separate values into the separator field.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Row separator]</p> </td> 
   <td> <p>Select or enter the type of separator that will separate the field value rows in the resulting bundle. If you select [!UICONTROL Other], enter the character you want to use to separate values into the separator field.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Define an expression that you want to group the aggregated output by. This expression can contain one or more mapped items. The aggregated data will be then separated into groups using this expression's value. Each group outputs as a separate bundle with a key (the evaluated expression) and a value (the aggregated value). You can use the key as a filter in subsequent modules.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Select this option to stop the scenario when there are no results.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Text aggregator]

This module merges values from the selected fields of received bundles into a single bundle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Select the module you want to aggregate fields from.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Row separator]</p> </td> 
   <td> <p>Select or enter the type of separator that will separate the field value rows in the resulting bundle. If you select [!UICONTROL Other], enter the character you want to use to separate values into the separator field.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Define an expression containing one or more mapped items. The aggregated data is separated under Groups with the same expression's value. Each Group outputs as a separate bundle containing a Key with the evaluated expression and the aggregated text. By doing this, you can use the Key as a filter in subsequent modules.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text]</td> 
   <td> <p> Enter or map the text that you want the module to aggregate.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Select this option to stop the scenario when there are no results.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Example:** You can use the text aggregator to insert more values (for example, customer names or notes)into a single bundle and send an email containing all the values in the email body or the email subject.

### Transformers

* [[!UICONTROL Compose a string]](#compose-a-string)
* [[!UICONTROL Convert the encoding of the text]](#convert-the-encoding-of-the-text)
* [[!UICONTROL Switch]](#switch)

#### [!UICONTROL Compose a string]

Converts any value to a string data type (text). It makes the mapping easier when mapping, for example, binary data.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p>Enter or map the data that you want to covert into text.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convert the encoding of the text]

Converts entered input text (or binary data) to the selected encoding.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input data]</p> </td> 
   <td> <p>Enter or map the content you want to convert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Input data codepage]</td> 
   <td> <p>Select the encoding type of the input data. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Output data codepage]</p> </td> 
   <td> <p>Select the encoding type of your target (output) data.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Switch]

Checks the input value for a match with the provided list of values. Returns output based on the result.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>Enter the expression you want to evaluate.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Use regular expressions to match]</td> 
   <td> <p>Enable this option to use regular expressions. The module determines the cases based on the regular expression, rather than an exact match.</p> 
    <div> 
     <p>A regular expression is a sequence of characters in which each character is either a metacharacter, having a special meaning, or a regular character that has a literal meaning. These character and metacharacters identify a pattern that can be used to search text. For example, if you wanted to search for names, you could set up a regular expression to search for a pattern that consists of two consecutive words that begin with capital letters. Regular expressions are a powerful tool for searching and manipulating text.</p> 
     <p>A discussion of regular expressions is beyond the scope of this article. We recommend the following resources:</p> 
     <ul> 
      <li>For the complete list of metacharacters, see <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Regular expressions</a> in MDN web docs.</li> 
      <li>For a tutorial on how to create regular expressions, we recommend <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>For experimenting with regular expressions, we recommend the <a href="https://regex101.com/">Regular Expressions 101</a> website. Select the ECMAScript (JavaScript) FLAVOR in the left panel.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cases] </td> 
   <td> <p>If the input contains a value entered to the [!UICONTROL Pattern] field, then the value entered to the [!UICONTROL Output] field is returned.</p> <p>If the input does not match any of the values that you have set in a [!UICONTROL Pattern] field, then one of the following occurs:</p> 
    <ul> 
     <li>The value from the [!UICONTROL Else] field is returned</li> 
     <li>If there is no value in the [!UICONTROL Else] field, no output is returned.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Enter the value that is returned when the criteria set in the Cases field are not met. </p> </td> 
  </tr> 
 </tbody> 
</table>
