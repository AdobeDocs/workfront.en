---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Calculated data expressions
description: You can use data expressions to define calculated custom data fields in Adobe Workfront. They connect existing Workfront fields in statements that generate a new field.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
---
# Calculated data expressions

You can use data expressions to define calculated custom data fields in Adobe Workfront. They connect existing Workfront fields in statements that generate a new field.

You can use calculated data expressions in:

* A custom form

  For more information about creating calculated custom data fields on custom forms in Workfront, see [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* A calculated custom column in a report or list, when you use text mode

  For more information about using text mode in reports and views, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntax of calculated custom fields vs. calculated custom columns

Although the functions that you use are the same, the syntax for building an expression in a calculated custom field can be different than it is for  building a calculated custom column.

For example:

* In a custom field, on a custom form for tasks, you would use the following to generate the name of the parent project of the task where the custom form is attached:

  ```
  {project}.{name}
  ```

* In a custom column in a report, you would use the following to add a Project Name custom column on a task report:

  ```
  valuefield=project:name
  ```

  Or

  ```
  valueexpression={project}.{name}
  ```

  >[!TIP]
  >
  >The same syntax applies to all text-mode reporting elements where calculated expressions are used: views, filters, groupings, prompts.

The differences between the two syntaxes are:  

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Calculated custom field</strong></td> 
   <td><strong>Calculated custom reporting element</strong></td> 
  </tr> 
   <td>Enclose field names in curly brackets.</td> 
   <td>Do not enclose field names in brackets or parentheses when using them in a <code>valuefield </code>line. <p>Enclose field names in curly brackets when using them in a <code>valueexpression</code> line.</p> </td> 
  </tr> 
  <tr> 
   <td>Separate the fields by periods.</td> 
   <td> <p>Separate the fields by colons when using them in a <code>valuefield </code>line</p> <p>Separate the fields by periods when using them in a <code>valueexpression </code>line. </p> </td> 
  </tr> 
 </tbody> 
</table>

For more information about the syntax you must use in a calculated custom column, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Data expressions you can use

The lists below define the available expressions you can use when you are building one of the 3 different types of calculated custom fields in Workfront:

* [Date & time calculated custom fields](#date-time-calculated-custom-fields) 
* [Mathematical calculated custom fields](#mathematical-calculated-custom-fields) 
* [Text calculated custom fields](#text-calculated-custom-fields)

### Date & time calculated custom fields {#date-time-calculated-custom-fields}

>[!NOTE]
>
>If you create a date and time calculation that doesn't include a time portion, or that uses the date wildcards $$TODAY or $$NOW, the system uses the date according to the Coordinated Universal Time (UTC) zone, not according your local timezone. This can cause an unexpected date result.

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
   <td> <p>This expression adds the number of days to the date. The number value can include partial days (e.g., 1.5 will add one and a half days to the date).</p> <p>The expression is formatted as follows:</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>This expression adds the number of weekdays to the date. This expression only adds whole integer values to the date, rounding down. </p> <p>The expression is formatted as follows:</p><pre>ADDWEEKDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>This expression adds the number of months to the date and is formatted as follows:</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>This expression adds the number of years to the date and is formatted as follows:</p><pre>ADDYEARS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>This expression clears the time portion of a date and is formatted as follows. In this example, the date is the entry date for a work object.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>This expression converts a string to a date and is formatted as follows:</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>This expression returns the number of days between the two dates, taking into account the start and the end days of the period selected as well as the time stamps on those days. For example, if the start time of the start date is 3 PM, the start day will not be counted as a full day.</p> <p>The expression is formatted as follows:</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>This expression returns the day of month for the date as a number, between 1 and 31.</p> <p>The expression is formatted as follows. In this example, the date is the entry date for a work object.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>This expression returns the day of week for the date as a number, between 1 (Sunday) and 7 (Saturday).</p> <p>The expression is formatted as follows. In this example, the date is the entry date for a work object.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>This expression returns the total days in the month of the date as a number and is formatted as follows. In this example, the date is the entry date for a work object.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>This expression returns the total weekdays between the date and the end of the week, or the end of the month, whichever comes first. In this example, the date is the entry date for a work object.</p> <p>The expression is formatted as follows:</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>This expression returns the total days in the year of the date as a number and is formatted as follows. In this example, the date is the entry date for a work object.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>This expression returns the latest date in the list and is formatted as follows:</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>This expression returns the earliest date in the list and is formatted as follows:</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>This expression returns the hour of the date as a number between 0 and 23.</p> <p>The expression is formatted as follows. In this example, the date is the entry date for a work object.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>This expression returns the minute of the date as a number between 0 and 60, formatted as follows. In this example, the date is the entry date for a work object.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>This expression returns the month of the date as a number between 1 and 12, formatted as follows. In this example, the date is the entry date for a work object.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>This expression returns the second of the date as a number between 0 and 60, formatted as follows. In this example, the date is the entry date for a work object.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>This expression returns the number of weekdays between two dates, taking into account the start and the end days of the period selected as well as the time stamps on those days. For example, if the start time of the start date is 3 PM, the start day will not be counted as a full day.</p> <p>The expression is formatted as follows:</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>This expression returns the number of scheduled minutes between the dates according to the default schedule.</p> <p>The expression is formatted as follows:</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>YEAR</strong> </td> 
   <td> <p>This expression returns the year of the date as a 4-digit number, formatted as follows. In this example, the date is the entry date for a work object.</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### Mathematical calculated custom fields {#mathematical-calculated-custom-fields}

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
   <td>This expression returns the absolute value of the number and is formatted as follows. This example uses the  number of objects below the object where the custom form is attached.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>This expression returns the average of numbers and is formatted as follows:<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>This expression rounds a number up to the nearest integer and is formatted as follows. This example uses the  number of  objects below the object where the custom form is attached.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>This expression divides all the numbers in the order provided and is formatted as follows:<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>This expression rounds a number down to the nearest integer and is formatted as follows. This example uses the  number of objects below the object where the custom form is attached.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>This expression returns the natural logarithm value of the number and is formatted as follows:<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>This expression returns the logarithm value of number2 to the base number1 and is formatted as follows:<pre>LOG(number1, number2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>This expression returns the largest item in the list and is formatted as follows:<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>This expression returns the smallest item in the list and is formatted as follows:<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>This expression converts a string to a number and is formatted as follows:<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>This expression returns a number raised to a power and is formatted as follows:<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>This expression multiplies all the numbers and is formatted as follows:<pre>PROD(number1, number2, ....)</pre>
   <b>NOTE</b>

   When multiplying fields that contain hours, ensure that you understand whether the hours in the selected fields are saved in minutes, hours, or seconds in the database. If the hours are saved in minutes or seconds but display in hours in the Workfront interface, you might need to account for the conversion from minutes or seconds to hours when writing an expression using this calculation. 
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>This expression rounds the number up to specified decimals of precision and is formatted as follows:<p>ROUND(number, precision)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> This expression orders the numbers in ascending order and is formatted as follows:</p><pre>SORTASCNUM(number1,number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>This expression orders the numbers in descending order and is formatted as follows:<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>This expression returns a square root of a number and is formatted as follows. This example uses the  number of objects below the object where the custom form is attached.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>This expression subtracts all numbers in the order provided and is formatted as follows:<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>This expression adds all the numbers and is formatted as follows:<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### Text calculated custom fields {#text-calculated-custom-fields}

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
   <td> <p>This expression is used with other expressions to choose a value from a list, based on a index number. An index number is a field or function that returns a numerical value (usually in a known range).</p> <p>The expression is formatted as follows:</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>For example, the following expression returns the name of the day of the week, where 1=Sunday, 2=Monday, and so on, in a calculated column:</p><pre>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</pre> <p>This expression works best with other expressions that return a number, such as DAYOFWEEK, DAYOFMONTH, and MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>This expression concatenates the string and is formatted as follows:</p><pre>CONCAT(string1,"separator", string2)</pre> <p>The following are examples of separators that you can include:</p> 
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
   <td>This expression returns true if the findText string is found within the withinText string and is formatted as follows:<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>This expression escapes any special characters in the string so they an be included in a URL argument.<p>The expression is formatted as follows:</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>This expression evaluates a condition that you specify and returns the value of the trueExpression if it is true, or the value of the falseExpression if it is false.</p> <p>The expression is formatted as follows:</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>For example, you can compare two different date fields followed by a True/False result as a data string:</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</pre> <p>In everyday speech, this statement means: "IF the Projected Completion Date of my object is 'Greater Than' the Planned Completion Date of my same object, then display the words 'Off Track' in this field; otherwise, display the words 'On Track.'"</p> <p>If you do not want to label the true or false expressions, you must insert a blank label in your statement, such as:</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</pre> <p>Or</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</pre> <p>For more information about building "IF" statements, see <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">"IF" statements overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>This expression allows you to look for a specific value in a string of possible values. If the value you are looking for equals one of the provided values, then the expression returns the trueExpression; otherwise, it returns the falseExpression.</p> <p>The expression is formatted as follows:</p><pre>IFIN(value, value1, value2,..., trueExpression, falseExpression)</pre> <p>For example, you can find a specific Project Owner and mark those projects with a specified tag in a project view: <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> In everyday speech, this statement means: "If the Project Owner is Jennifer Campbell or Rick Kuvec, mark this project with 'Marketing Team'; otherwise, mark it with 'Other Teams'."</p> <p> If you do not want to label the true or false expressions, you must insert a blank label in your statement, such as: </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>Or </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>This expression returns true if the value equals one of the provided values; otherwise, the expression returns false.</p> <p>The expression is formatted as follows:</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>This expression returns true if the value is null or empty; otherwise, the expression returns false.</p> <p>The expression is formatted as follows:</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>This expression returns a specified number of characters from the left side of a string and is formatted as follows:</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>This expression returns the length of a string and is formatted as follows:</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>This expression returns the string in lower case and is formatted as follows:<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>REPLACE</strong> </td> 
   <td> <p>This expression replaces all occurences of string2 with string3 in string1.</p> <p>The expression is formatted as follows:</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>This expression returns a specified number of characters from the right side of a string and is formatted as follows:</p><pre>RIGHT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>This expression returns the index of the first occurrence of findText in the string withinText, starting at the given start position, or -1 if the text is not found.</p> <p>The expression is formatted as follows:</p><pre>SEARCH(findText, withinText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>This expression converts a number to a string and is formatted as follows:</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>This expression sorts a list of strings in ascending order and is formatted as follows:</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> This expression sorts a list of strings in descending order and is formatted as follows:</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>This expression return characters of a string based upon the start and end index specified and is formatted as follows:</p><pre>SUBSTR({string}, number of start position, number of end position)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>This expression removes whitespace from the beginning and end of a string and is formatted as follows:</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>This expression returns a string in upper case and is formatted as follows:</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
