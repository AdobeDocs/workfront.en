---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Overview of calculated data expressions
description: You can use data expressions to define calculated custom data fields in Adobe Workfront. Calculated expressions connect existing Workfront fields in statements that generate a new field.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
---
# Overview of calculated data expressions

<!--Audited: 12/2023-->

You can use data expressions to define calculated custom fields in Adobe Workfront. Calculated expressions connect existing Workfront fields in statements that generate a new field.

You can use calculated data expressions in:

* A calculated custom field on a custom form

  For more information about creating calculated custom fields on custom forms in Workfront, see [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* A calculated custom column in a report or list, when you use text mode

  For more information about using text mode in reports and views, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntax of calculated custom fields vs. calculated custom columns

Although the functions that you use are the same, the syntax for building an expression in a calculated custom field can be different from it is for  building a calculated custom column.

The differences between the two syntaxes are:  

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Calculated custom field</strong></td> 
   <td><strong>Calculated custom reporting element</strong></td> 
  </tr> 
   <td>Enclose field names in curly brackets</td> 
   <td>Do not enclose field names in brackets or parentheses when using them in a <p><code>valuefield </code></p>line. <p>Enclose field names in curly brackets when using them in a <p><code>valueexpression</code></p> line.</p> </td> 
  </tr> 
  <tr> 
   <td>Separate the fields by periods</td> 
   <td> <p>Separate the fields by colons when using them in a <p><code>valuefield </code></p>line</p> <p>Separate the fields by periods when using them in a <p><code>valueexpression </code></p>line. </p> </td> 
  </tr> 
 </tbody> 
</table>

For example:

* In a custom field, on a custom form for tasks, you would use the following to generate the name of the parent project of the task where the custom form is attached:


   ` {project}.{name}`


* In a custom column in a report, you would use the following to add a Project Name custom column on a task report:

  
    `valuefield=project:name`
  

  Or

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >The same syntax applies to all text-mode reporting elements where calculated expressions are used: views, filters, groupings, prompts.

For more information about the syntax you must use in a calculated custom column, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Data expressions you can use

The lists below define the available expressions you can use when you are building one of the 3 different types of calculated custom fields in Workfront:

* [Date and time calculated custom fields](#date-time-calculated-custom-fields) 
* [Mathematical calculated custom fields](#mathematical-calculated-custom-fields) 
* [Text calculated custom fields](#text-calculated-custom-fields)

You can use the expressions listed below to build calculated custom columns. However, you must use the correct syntax for a calculated custom column, as described in the section  [Syntax of calculated custom fields vs. calculated custom columns](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in this article. 

### Date and time calculated custom fields {#date-time-calculated-custom-fields}

>[!NOTE]
>
>If you create a date and time calculation that doesn't include a time portion, or that uses the date wildcards $$TODAY or $$NOW, the system uses the date according to the Coordinated Universal Time (UTC) zone, not according your local timezone. This can cause an unexpected date result.

You can create a date or time calculated custom field using the following expressions: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expression</th> 
   <th>Explanation and example</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>Adds the number of days to the date. The number value can include partial days. For example, 1.5 adds one and a half days to the date.</p> <p>The expression is formatted as follows:</p>
   
   <p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Adds the number of weekdays to the date. This expression only adds whole integer values to the date, rounding down. </p> <p>The expression is formatted as follows:</p>
   
   <p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Adds the number of months to the date and is formatted as follows:
   
   </p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Adds the number of years to the date and is formatted as follows:</p>
   
   <p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Clears the time portion of a date and is formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Converts a string to a date and is formatted as follows:</p>
   
   <p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Returns the number of days between the two dates, taking into account the start and the end days of the period selected as well as the time stamps on those days. For example, if the start time of the start date is 3 PM, the start day is not counted as a full day.</p> <p>The expression is formatted as follows:</p>
   
   <p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Returns the day of month for the date as a number, between 1 and 31.</p> <p>The expression is formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Returns the day of week for the date as a number, between 1 (Sunday) and 7 (Saturday).</p> <p>The expression is formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Returns the total days in the month of the date as a number and is formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Returns the total weekdays between the date and the end of the week, or the end of the month, whichever comes first. In this example, the date is the Entry Date for a work object.</p> <p>The expression is formatted as follows:</p>
   
   <p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Returns the total days in the year of the date as a number and is formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Returns the latest date in the list and is formatted as follows:</p>
   
   <p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Returns the earliest date in the list and is formatted as follows:</p>
   
   <p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>Returns the hour of the date as a number between 0 and 23.</p> <p>The expression is formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Returns the minute of the date as a number between 0 and 60, formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>Returns the month of the date as a number between 1 and 12, formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Returns the second of the date as a number between 0 and 60, formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Returns the number of weekdays between two dates, taking into account the start and the end days of the period selected as well as the time stamps on those days. For example, if the start time of the start date is 3 PM, the start day will not be counted as a full day.</p> <p>The expression is formatted as follows:</p>
   
   <p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Returns the number of scheduled minutes between the dates according to the default schedule.</p> <p>The expression is formatted as follows:</p>
   
   <p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>YEAR</strong> </td> 
   <td> <p>Returns the year of the date as a 4-digit number, formatted as follows. In this example, the date is the Entry Date for a work object.</p>
   
   <p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Mathematical calculated custom fields {#mathematical-calculated-custom-fields}

You can create a calculated custom field that that uses some of the following mathematical expressions: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expression</th> 
   <th>Explanation</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>Returns the absolute value of the number and is formatted as follows. This example uses the  number of objects below the object where the custom form is attached.
   
   <p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Returns the average of numbers and is formatted as follows:
   
   <p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Rounds a number up to the nearest integer and is formatted as follows. This example uses the  number of  objects below the object where the custom form is attached.
   
   <p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Divides all the numbers in the order provided and is formatted as follows:
   
   <p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Rounds a number down to the nearest integer and is formatted as follows. This example uses the  number of objects below the object where the custom form is attached.
   
   <p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Returns the natural logarithm value of the number and is formatted as follows:
   
   <p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Returns the logarithm value of number2 to the base number1 and is formatted as follows:
   
   <p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Returns the largest item in the list and is formatted as follows:
   
   <p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Returns the smallest item in the list and is formatted as follows:
   
   <p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>Converts a string to a number and is formatted as follows:<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Returns a number raised to a power and is formatted as follows:
   
   <p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Multiplies all the numbers and is formatted as follows:
   
   <p><code>PROD(number1, number2, ....)</code></p>
   <p><b>NOTE</b></p>

   <p>When multiplying fields that contain hours, ensure that you understand whether the database saves the hours in selected fields in minutes, hours, or seconds. If the hours are saved in minutes or seconds but display in hours in the Workfront interface, you might need to account for the conversion from minutes or seconds to hours when writing an expression using this calculation. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Rounds the number up to specified decimals of precision and is formatted as follows:
   
   <p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Orders the numbers in ascending order and is formatted as follows:</p>
   
   <p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Orders the numbers in descending order and is formatted as follows:
   
   <p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Returns a square root of a number and is formatted as follows. This example uses the  number of objects below the object where the custom form is attached.</p>
   
   <p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Subtracts all numbers in the order provided and is formatted as follows:
   
   <p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Adds all the numbers and is formatted as follows:
   
   <p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Text calculated custom fields {#text-calculated-custom-fields}

You can create a calculated custom field that displays a text-formatted value using the following expressions:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expression</th> 
   <th>Explanation</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>CASE</strong> </td> 
   <td> <p>Is used with other expressions to choose a value from a list, based on an index number. </p>
   <p>An index number is a field or function that returns a numerical value (usually in a known range).</p> 
   <p>The expression is formatted as follows:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p> 
   
   <p>For example, the following expression returns the name of the day of the week, where 1=Sunday, 2=Monday, and so on, in a calculated column:</p>
   
   <p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p> 
   
   <p>Works best with other expressions that return a number, such as DAYOFWEEK, DAYOFMONTH, and MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Concatenates the string and is formatted as follows:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>The following are examples of separators that you can include:</p> 
    <ul> 
     <li>a space: " "</li> 
     <li>a dash: "-"</li> 
     <li>a slash: "/"</li> 
     <li>a comma: ","</li> 
     <li>a word: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>Returns true if the findText string is found within the withinText string and is formatted as follows:
   
   <p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Escapes any special characters in the string so they can be included in a URL argument.<p>The expression is formatted as follows:</p>
   
   <p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Evaluates a condition that you specify and returns the value of the trueExpression if it is true, or the value of the falseExpression if it is false.</p> 
   
   <p>The expression is formatted as follows:</p>
   
   <p><code>IF(condition, trueExpression, falseExpression)</code></p> 
   
   <p>For example, you can compare two different date fields followed by a True/False result as a data string:</p>
   
   <p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p> 
   
   <p>In everyday speech, this statement means: "IF the Projected Completion Date of my object is 'Greater Than' the Planned Completion Date of my same object, then display the words 'Off Track' in this field; otherwise, display the words 'On Track.'"</p> 
   
   <p>If you do not want to label the true or false expressions, you must insert a blank label in your statement, such as:</p>
   
   <p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>Or</p>
   
   <p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p> 
   
   <p>For more information about building "IF" statements, see <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">"IF" statements overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Allows you to look for a specific value in a string of possible values. If the value you are looking for equals one of the provided values, then the expression returns the trueExpression; otherwise, it returns the falseExpression.</p> 
   <p>The expression is formatted as follows:</p>
   
   <p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p> 
   
   <p>For example, you can find a specific Project Owner and mark those projects with a specified tag in a project view: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> In everyday speech, this statement means: "If the Project Owner is Jennifer Campbell or Rick Kuvec, mark this project with 'Marketing Team'; otherwise, mark it with 'Other Teams'."</p> 
    <p> If you do not want to label the true or false expressions, you must insert a blank label in your statement, such as: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>Or </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Returns true if the value equals one of the provided values; otherwise, the expression returns false.</p> <p>The expression is formatted as follows:
   
   </p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Returns true if the value is null or empty; otherwise, the expression returns false.</p> <p>The expression is formatted as follows:
   
   </p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>Returns a specified number of characters from the left side of a string and is formatted as follows:</p>
   
   <p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Returns the length of a string and is formatted as follows:</p>
   
   <p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Returns the string in lower case and is formatted as follows:
   
   <p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>REPLACE</strong> </td> 
   <td> <p>Replaces all occurences of string2 with string3 in string1.</p> <p>The expression is formatted as follows:</p>
   
   <p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>Returns a specified number of characters from the right side of a string and is formatted as follows:</p>
   
   <p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Returns the index of the first occurrence of findText in the string withinText, starting at the given start position, or -1 if the text is not found.</p> <p>The expression is formatted as follows:</p>
   
   <p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>Converts a number to a string and is formatted as follows:</p>
   
   <p><code>STRING(number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Sorts a list of strings in ascending order and is formatted as follows:</p>
   
   <p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Sorts a list of strings in descending order and is formatted as follows:</p>
   
   <p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Returns characters of a string based on the start and end index specified and is formatted as follows:</p>
   
   <p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Removes whitespace from the beginning and end of a string and is formatted as follows:</p>
   
   <p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Returns a string in upper case and is formatted as follows:</p>
   
   <p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
