---
filename: tools-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Tools
description: The Adobe Workfront Fusion Tools section includes several useful modules that can enhance your scenario.
---

# Tools

The `Adobe Workfront Fusion` Tools section includes several useful modules that can enhance your scenario.

Tools modules are available from the list of apps, or from the Tools icon ![](assets/tools-icon-small.png) at the bottom of the screen.

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

## Tools and their fields

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Aggregators](#aggregat) 
* [Transformers](#transfor)

### Triggers

#### Basic trigger

This module allows you to create a custom trigger and define its input bundles.

You can use this module, for example, for contacts or any other list that is scheduled to be sent to a specified email address (such as Email > Send an Email, or Gmail > Send an Email modules), or as a simple reminder to be triggered whenever you want.

| Bundle |Create custom bundles by adding array items. The array consists of the name - value pairs. |
|---|---|

### Actions

* [Get Multiple Variables](#get) 
* [Get Variable](#get2) 
* [Increment function](#incremen) 
* [Set Multiple Variables](#set) [Set Variable](#set2) 
* [Set Variable](#set2) 
* [Sleep](#sleep)

#### Get Multiple Variables

This module retrieves values that were previously created by the Set Variable or Set Multiple Variables module.

This module can read variables that were set anywhere in the scenario, even if the variable was set in a different route than where the Get Multiple Variables module is located. The only requirement is that the Tools >Set Variable or Tools > Set Multiple Variable module is executed before the Tools > Get Variable module. For more information on the order in which modules are executed, see [Router module](../../workfront-fusion/modules/router-module.md).

| Variables |Add the variables that you want the module to get. |
|---|---|
| Variable name |For each variable you add, map the name of the variable you want to get. |

<!--

-->

` `**Examples: **`` The following are possible uses of the Set/Get (multiple) variable(s) modules:

* To store a calculated value for later use, even in a different route. This is useful in cases when the value is used in multiple modules and the formula to calculate the value is overly complex.
* To debug a formula. If a formula used in a module does not seemingly provide a correct result, copy the formula and paste it into a Set Variable module that you insert before the relevant module. Disconnect the module(s) after the Set Variable module and execute the scenario. Verify the Set Variable module's output, adjust or simplify the formula, execute the scenario again, and continue to do so until the issue has been resolved.

#### Get Variable

This module retrieves a value that was previously created by the Set Variable or Set Multiple Variables module.

This module can read variables that were set anywhere in the scenario, even if the variable was set in a different route than where the Get Multiple Variables module is located. The only requirement is that the Tools >Set Variable or Tools > Set Multiple Variable module is executed before the Tools > Get Variable module. For more information on the order in which modules are executed, see [Router module](../../workfront-fusion/modules/router-module.md).

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Variable name</td> 
   <td> <p>Map the name of the variable that you want the module to get.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Increment function

This module returns a value incremented by 1 after each module's operation.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Reset a value</td> 
   <td> <p>Select when you want the module to increment the value. </p> 
    <ul> 
     <li>After one cycle</li> 
     <li>After one scenario run</li> 
     <li>Never</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

` `**Example: **`` One of the module's uses is to implement a "round robin" assignment of tasks, leads, emails, and so on, to users in a group. The algorithm chooses the assignees from a group in some rational order, usually going from the top to the bottom of a list. When the algorithm reaches the end of the list, it would then give the next assignment to the user at the top of the list and continue to make assignments down the list.

The following scenario sends an email to the first recipient after every odd-numbered scenario run, and to the second recipient after every even-numbered scenario run.

![](assets/example-email-350x246.gif)

<ol> 
 <li value="1">To create this scenario: </li> 
 <li value="2">Set the module's <span class="bold">Reset a value</span> field to Never.</li> 
 <li value="3"> <p>Set the route for odd values. Set the filter for this route using the modulus math function that equals <code>1</code>:</p> <p> <img src="assets/odd-350x459.png" style="width: 350;height: 459;"> </p> <note type="note">
   Do not forget to change the Equal to operator from the default Text operator to the Numeric operator.
  </note> </li> 
 <li value="4">Set the route for even values using the modulus math function that equals <code>0</code>:</li> 
</ol>

The increment function adds one every time the scenario runs. The filters check the increment and act on its value, ensuring that the emails are evenly distributed.

#### Set Multiple Variables

This module creates variables that can be mapped by other modules in the route. The variable can also be mapped to the Get Variable or Get Multiple Variables modules for any route in the scenario.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Variables</td> 
   <td>Add the variables that you want the module to set.</td> 
  </tr> 
  <tr> 
   <td>Variable name </td> 
   <td>For each variable, enter the variable name. This name will be displayed when mapping the variable in other modules. </td> 
  </tr> 
  <tr> 
   <td>Variable value </td> 
   <td>For each variable, enter the value for the variable. </td> 
  </tr> 
  <tr> 
   <td>Variable lifetime </td> 
   <td> <p>Select how long you want the variables to remain valid (keep the same value).</p> 
    <ul> 
     <li><span class="bold">One cycle</span>: The variable is valid for one cycle. Useful when multiple webhooks in one scenario run are received (more webhooks = more cycles). </li> 
     <li><span class="bold">One execution</span>: The variable is valid for one scenario execution. One execution can contain one or more cycles.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Set Variable

This module creates a variable that can be mapped by other modules in the route. The variable can also be mapped to the Get Variable or Get Multiple Variables modules for any route in the scenario.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Variable name </td> 
   <td>Enter the variable name. This name will be displayed when mapping the variable in other modules. </td> 
  </tr> 
  <tr> 
   <td>Variable lifetime </td> 
   <td> <p>Select how long you want the variables to remain valid (keep the same value).</p> 
    <ul> 
     <li><span class="bold">One cycle</span>: The variable is valid for one cycle. Useful when multiple webhooks in one scenario run are received (more webhooks = more cycles). </li> 
     <li><span class="bold">One execution</span>: The variable is valid for one scenario execution. One execution can contain one or more cycles.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Variable value </td> 
   <td>Enter or map the value for the variable. </td> 
  </tr> 
 </tbody> 
</table>

#### Sleep

This module allows you to delay the scenario flow for up to 300 seconds (5 minutes).

This function can be useful, for example, if you want to lower the target service server load or to imitate human behavior when sending bulk SMS or emails.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Delay</p> </td> 
   <td> <p>Enter the number of seconds the scenario will be paused for.</p> </td> 
  </tr> 
 </tbody> 
</table>

` `**Tip: **`` If you want to pause the flow for longer periods of time, we suggest to split your scenario into two scenarios:

* The first scenario would contain the part before the pause
* The second scenario would contain the part after it.

The first scenario would end up with storing all the necessary information in a data store together with the current timestamp. The second scenario would periodically check the data store for records with a timestamp older than the intended delay, retrieve the records, finalize the processing of the data and remove the records from the data store.

For more information on data stores, see [Data Stores](../../workfront-fusion/modules/data-stores.md).

For more information on specific data store modules, see [Data store modules](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Aggregators

* [Numeric aggregator](#numeric) 
* [Table aggregator](#table) 
* [Text aggregator](#text)

#### Numeric aggregator

This module allows you to retrieve numerical values, then apply one of the selected functions (SUM, AVG, COUNT, MAX, MIN), and return the result in one bundle.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Source module</p> </td> 
   <td> <p>Select the module you want to aggregate fields from.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggregate function</p> </td> 
   <td> <p>Select the function that you want to use to aggregate the values.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Group by</p> </td> 
   <td> <p>Define an expression that you want to group the aggregated output by. This expression can contain one or more mapped items. The aggregated data is then separated into groups using this expression's value. Each group outputs as a separate bundle with a key (the evaluated expression) and a value (the aggregated value). You can use the key as a filter in subsequent modules.</p> </td> 
  </tr> 
  <tr> 
   <td>Stop processing after an empty aggregation</td> 
   <td>Enable this option to stop the scenario when there are no results.</td> 
  </tr> 
  <tr> 
   <td> <p>Value</p> </td> 
   <td> <p>Enter or map the value that you want to aggregate.</p> </td> 
  </tr> 
 </tbody> 
</table>

` `**Example: **`` The module sums up values under the number parameter.

![](assets/module-sums-up-values-350x186.gif)

#### Table aggregator

This module merges values from the selected fields of received bundles into a single bundle using a specified column and row separator (which allows you to create a table).

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Source module</p> </td> 
   <td> <p>Select the module you want to aggregate fields from.</p> </td> 
  </tr> 
  <tr> 
   <td>Aggregated fields</td> 
   <td> <p> Select the fields from the module selected above that contain values you want to aggregate into the one bundle.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Column separator</p> </td> 
   <td> <p>Select or enter the type of separator that will separate the field value columns in the resulting bundle. If you select Other, enter the character you want to use to separate values into the separator field.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Row separator</p> </td> 
   <td> <p>Select or enter the type of separator that will separate the field value rows in the resulting bundle. If you select Other, enter the character you want to use to separate values into the separator field.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Group by</p> </td> 
   <td> <p>Define an expression that you want to group the aggregated output by. This expression can contain one or more mapped items. The aggregated data will be then separated into groups using this expression's value. Each group outputs as a separate bundle with a key (the evaluated expression) and a value (the aggregated value). You can use the key as a filter in subsequent modules.</p> </td> 
  </tr> 
  <tr> 
   <td>Stop processing after an empty aggregation</td> 
   <td>Select this option to stop the scenario when there are no results.</td> 
  </tr> 
 </tbody> 
</table>

#### Text aggregator

This module merges values from the selected fields of received bundles into a single bundle.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Source module</p> </td> 
   <td> <p>Select the module you want to aggregate fields from.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Row separator</p> </td> 
   <td> <p>Select or enter the type of separator that will separate the field value rows in the resulting bundle. If you select Other, enter the character you want to use to separate values into the separator field.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Group by</p> </td> 
   <td> <p>Define an expression containing one or more mapped items. The aggregated data is separated under Groups with the same expression's value. Each Group outputs as a separate bundle containing a Key with the evaluated expression and the aggregated text. By doing this, you can use the Key as a filter in subsequent modules.</p> </td> 
  </tr> 
  <tr> 
   <td>Text</td> 
   <td> <p> Enter or map the text that you want the module to aggregate.</p> </td> 
  </tr> 
  <tr> 
   <td>Stop processing after an empty aggregation</td> 
   <td>Select this option to stop the scenario when there are no results.</td> 
  </tr> 
 </tbody> 
</table>

` `**Example: **``You can use the text aggregator to insert more values (for example, customer names or notes)into a single bundle and send an email containing all the values in the email body or the email subject.

### Transformers

* [Compose a string](#compose) 
* [Convert the encoding of the text](#convert) 
* [Switch](#switch)

#### Compose a string

Converts any value to a string data type (text). It makes the mapping easier when mapping, for example, binary data.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Text</td> 
   <td> <p>Enter or map the data that you want to covert into text.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Convert the encoding of the text

Converts entered input text (or binary data) to the selected encoding.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Input data</p> </td> 
   <td> <p>Enter or map the content you want to convert.</p> </td> 
  </tr> 
  <tr> 
   <td>Input data codepage</td> 
   <td> <p>Select the encoding type of the input data. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Output data codepage</p> </td> 
   <td> <p>Select the encoding type of your target (output) data.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Switch

Checks the input value for a match with the provided list of values. Returns output based on the result.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Input</p> </td> 
   <td> <p>Enter the expression you want to evaluate.</p> </td> 
  </tr> 
  <tr> 
   <td>Use regular expressions to match</td> 
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
   <td>Cases </td> 
   <td> <p>If the input contains a value entered to the Pattern field, then the value entered to the Output field is returned.</p> <p>If the input does not match any of the values that you have set in a Pattern field, then one of the following occurs:</p> 
    <ul> 
     <li>The value from the Else field is returned</li> 
     <li>If there is no value in the Else field, no output is returned.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Else</p> </td> 
   <td> <p>Enter the value that is returned when the criteria set in the Cases field are not met. </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
Execute a scenario
-->

<!--
Status: PLANNED - see the Workaround section below.
-->

<!--
Workaround
-->

<!--
Employ the HTTP modules > Make a request module in the main scenario to call the other scenario. Employ the Webhooks > Custom webhook module in the other scenario to receive the call. Employ the Webhooks > Webhook response module in the other scenario to return the response.
-->

<!--
Stop / Throw (an error)
-->

<!--
In some cases you may want to forcibly stop the scenario execution after the rollback or commit phase or stop the processing of a route and optionally store it in the queue of incomplete executions.
-->

<!--
Status: PLANNED - see the Throw module.
-->

