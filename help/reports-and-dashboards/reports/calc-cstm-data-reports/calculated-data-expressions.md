---
filename: calculated-data-expressions
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
---



# Calculated data expressions {#calculated-data-expressions}

You can use data expressions to define calculated custom data fields in *`Adobe Workfront`*. They connect existing *`Workfront`* fields in statements that generate a new field.


You can use calculated data expressions in:



*  A custom form  



  For more information about creating calculated custom data fields on custom forms in *`Workfront`*, see [Add calculated data to a custom form](add-calculated-data-to-custom-form.md).

*  A calculated custom column in a report or list, when you use text mode  



  For more information about using text mode in reports and views, see [Text Mode overview](understand-text-mode.md).





## The syntax of calculated custom fields vs the syntax of calculated custom columns  {#the-syntax-of-calculated-custom-fields-vs-the-syntax-of-calculated-custom-columns}

Although the data expressions used are the same, the syntax for building a calculated custom field is different than that of building a calculated custom column.


For example:



*  To add a calculated data expression to a custom field on a task form for the Project Name, you use the following text: 




  ```
  Project.Name
  ```



*  To add a calculated data expression to a custom column on a task report for the Project Name, you use the following text:


  *

  ```
  valuefield=project:name
  ```

* 


  Or  





  ```
  valueexpression={project}.{name}
  ```




  >[!TIP] {type="tip"}
  >
  >The same syntax applies to all text-mode reporting elements where calculated expressions are used: views, filters, groupings, prompts. 





The differences between the two syntaxes are: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStylesheets/Standard.css');" class="TableStyle-Standard" cellspacing="3"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Calculated custom field</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="font-weight: bold;">Calculated custom reporting element</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray"> <p>Use the name of the fields as they appear in&nbsp;the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> interface.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>Example of field name used in a calculated custom field:&nbsp;<code>Planned Completion Date</code>.</p> </td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray"> <p>Use the name of the objects or fields as they appear in the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> database. The names of objects and fields are spelled in lower case or camel case, if they are compound names. </p> <p>For an inventory of all&nbsp;<span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> objects and fields as they appear in the database, see <a href="api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>Example of field name used in a calculated custom reporting element:&nbsp;<code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Do not enclose field names in parentheses or curly brackets.</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray"> <p>Do not enclose field names in brackets or parentheses when using them in a <code>valuefield </code>line.</p> <p>Enclose field names in curly brackets when using them in a <code>valueexpression</code> line.</p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyB-Column1-MediumGray">Separate the fields by periods.</td> 
   <td class="TableStyle-Standard-BodyA-Column1-MediumGray"> <p>Separate the fields by colons when using them in a <code>valuefield </code>line</p> <p>Separate the fields by periods when using them in a <code>valueexpression </code>line. </p> </td> 
  </tr> 
 </tbody> 
</table>

For more information about the syntax you must use in a calculated custom column, see [Text Mode overview](understand-text-mode.md).


## Data expressions you can use {#data-expressions-you-can-use}

The lists below define the available expressions you can use when you are building one of the 3 different types of calculated custom fields in *`Workfront`*:



*  [Date & time calculated custom field](#date) 
*  [Mathematical calculated custom field](#mathemat) 
*  [Text calculated custom field](#text) 




### Date & time calculated custom field {#date-time-calculated-custom-field}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');width: 100%;margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Expression</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Explanation</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">ADDDAYS</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression adds the number of days to date and is formatted as follows:</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">ADDWEEKDAYS</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression adds the number of weekdays to date and is formatted as follows:</p><pre>ADDWEEKDAYS(date, number)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">ADDMONTHS</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression adds the number of months to date and is formatted as follows:</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">ADDYEARS</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression adds the number of years to date and is formatted as follows:</p><pre>ADDYEARS(date, number)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">CLEARTIME</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression clears the time portion of a date and is formatted as follows:</p><pre>CLEARTIME(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">DATE</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression converts a string to a date and is formatted as follows:</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">DATEDIFF</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns the number of days between the two dates, taking into account the start and the end days of the period selected as well as the time stamps on those days. For example, if the start time of the start date is 3 PM, the start day will not be counted as a full day.</p> <p>The expression is formatted as follows:</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">DAYOFMONTH</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns the day of month for the given date as a number, between 1 and 31.</p> <p>The expression is formatted as follows:</p><pre>DAYOFMONTH(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">DAYOFWEEK</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns the day of week for the given date as a number, between 1 (Sunday) and 7 (Saturday).</p> <p>The expression is formatted as follows:</p><pre>DAYOFWEEK(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">DAYSINMONTH</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns the total days in the month of the given date as a number and is formatted as follows:</p><pre>DAYSINMONTH(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">DAYSINSPLITWEEK</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns the total weekdays between the date and the end of the week, or the end of the month, whichever comes first.</p> <p>The expression is formatted as follows:</p><pre>DAYSINSPLITWEEK(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">DAYSINYEAR</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns the total days in the year of the given date as a number and is formatted as follows:</p><pre>DAYSINYEAR(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">DMAX</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns the latest date in the list and is formatted as follows:</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">DMIN</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns the earliest date in the list and is formatted as follows:</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">HOUR</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns the hour of the given date as a number between 0 and 23</p> <p>The expression is formatted as follows:</p><pre>HOUR(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">MINUTE</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns the minute of the given date as a number and is formatted as follows:</p><pre>MINUTE(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">MONTH</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns the month of the given date as a number and is formatted as follows:</p><pre>MONTH(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">SECOND</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns the second of the given date as a number and is formatted as follows:</p><pre>SECOND(date)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">WEEKDAYDIFF</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns the number of weekdays between two dates, taking into account the start and the end days of the period selected as well as the time stamps on those days. For example, if the start time of the start date is 3 PM, the start day will not be counted as a full day.</p> <p>The expression is formatted as follows:</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">WORKMINUTESDIFF</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns the number of scheduled minutes between the dates according to the default schedule.</p> <p>The expression is formatted as follows:</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><span class="bold">YEAR</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>This expression returns the year of the given date as a number and is formatted as follows:</p><pre>YEAR(date)</pre> </td> 
  </tr> 
 </tbody> 
</table>



### Mathematical calculated custom field {#mathematical-calculated-custom-field}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');width: 100%;margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Expression</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Explanation</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">ABS</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression returns the absolute value of the number and is formatted as follows:<pre>ABS(number)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">AVERAGE</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This expression returns the average of numbers and is formatted as follows:<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">CEIL</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression rounds a number up to the nearest integer and is formatted as follows:<pre>CEIL(number)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">DIV</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This expression divides all the numbers in the order provided and is formatted as follows:<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">FLOOR</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression rounds a number down to the nearest integer and is formatted as follows:<pre>FLOOR(number)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">LN</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This expression returns the natural logarithm value of the number and is formatted as follows:<pre>LN(number)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">LOG</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression returns the logarithm value of number2 to the base number1 and is formatted as follows:<pre>LOG(number1, number2)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">MAX</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This expression returns the largest item in the list and is formatted as follows:<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">MIN</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression returns the smallest item in the list and is formatted as follows:<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">NUMBER</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This expression converts a string to a number and is formatted as follows:<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">POWER</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression returns a number raised to a power and is formatted as follows:<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">PROD</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This expression multiplies all the numbers and is formatted as follows:<pre>PROD(number1, number2, ....)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">ROUND</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression rounds the number up to specified decimals of precision and is formatted as follows:<p>ROUND(number, precision)</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">SORTASCNUM</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> This expression orders the numbers in ascending order and is formatted as follows:</p><pre>SORTASCNUM(number1,number2, ...)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">SORTDESCNUM</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression orders the numbers in descending order and is formatted as follows:<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">SQRT</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns a square root of a number and is formatted as follows:</p><pre>SQRT(number)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">SUB</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression subtracts all numbers in the order provided and is formatted as follows:<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><span class="bold">SUM</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">This expression adds all the numbers and is formatted as follows:<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>



### Text calculated custom field {#text-calculated-custom-field}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');width: 100%;margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Expression</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Explanation</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">CASE</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression is used with other expressions to choose a value from a list, based on a index number. An index number is a field or function that returns a numerical value (usually in a known range).</p> <p>The expression is formatted as follows:</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>For example, the following expression returns the name of the day of the week, where 1=Sunday, 2=Monday, and so on, in a calculated column:</p><pre>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</pre> <p>This expression works best with other expressions that return a number, such as DAYOFWEEK, DAYOFMONTH, and MONTH.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">CONCAT</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression concatenates the string and is formatted as follows:</p><pre>CONCAT(string1,"separator", string2)</pre> <p>The following are examples of separators that you can include:</p> 
    <ul> 
     <li>a space: " "</li> 
     <li>a dash: "-"</li> 
     <li>a slash: "/"</li> 
     <li>a comma: ","</li> 
     <li>a word: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">CONTAINS</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression returns true if the findText string is found within the withinText string and is formatted as follows:<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">ENCODEURL</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">This expression escapes any special characters in the string so they an be included in a URL argument.<p>The expression is formatted as follows:</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">IF</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression evaluates a condition that you specify and returns the value of the trueExpression if it is true, or the value of the falseExpression if it is false.</p> <p>The expression is formatted as follows:</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>For example, you can compare two different date fields followed by a True/False result as a data string:</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</pre> <p>In everyday speech, this statement means: “IF the Projected Completion Date of my object is ‘Greater Than’ the Planned Completion Date of my same object, then display the words ‘Off Track’ in this field; otherwise, display the words ‘On Track.’”</p> <p>If you do not want to label the true or false expressions, you must insert a blank label in your statement, such as:</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</pre> <p>Or</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</pre> <p>For more information about building "IF" statements, see <a href="if-statements-overview.md" class="MCXref xref">"IF" statements overview</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">IFIN</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression allows you to look for a specific value in a string of possible values. If the value you are looking for equals one of the provided values, then the expression returns the trueExpression; otherwise, it returns the falseExpression.</p> <p>The expression is formatted as follows:</p><pre>IFIN(value, value1, value2,..., trueExpression, falseExpression)</pre> <p>For example, you can find a specific Project Owner and mark those projects with a specified tag in a project view: <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> In everyday speech, this statement means: "If the Project Owner is Jennifer Campbell or Rick Kuvec, mark this project with 'Marketing Team'; otherwise, mark it with 'Other Teams'."</p> <p> If you do not want to label the true or false expressions, you must insert a blank label in your statement, such as: </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code><![CDATA[
						]]></p> <p>Or </p> <p><![CDATA[
						]]><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">IN</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns true if the value equals one of the provided values; otherwise, the expression returns false.</p> <p>The expression is formatted as follows:</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">ISBLANK</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns true if the value is null or empty; otherwise, the expression returns false.</p> <p>The expression is formatted as follows:</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">LEFT</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns a specified number of characters from the left side of a string and is formatted as follows:</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">LEN</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns the length of a string and is formatted as follows:</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">LOWER</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">This expression returns the string in lower case and is formatted as follows:<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">REPLACE</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression replaces all occurences of string2 with string3 in string1.</p> <p>The expression is formatted as follows:</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">RIGHT</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression returns a specified number of characters from the right side of a string and is formatted as follows:</p><pre>RIGHT(string, length)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">SEARCH</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression returns the index of the first occurrence of findText in the string withinText, starting at the given start position, or -1 if the text is not found.</p> <p>The expression is formatted as follows:</p><pre>SEARCH(findText, withinText, start)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">STRING</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression converts a number to a string and is formatted as follows:</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">SORTASCSTRING</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression sorts a list of strings in ascending order and is formatted as follows:</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">SORTDESCSTRING</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> This expression sorts a list of strings in descending order and is formatted as follows:</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">SUBSTR</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This expression return characters of a string based upon the start and end index specified and is formatted as follows:</p><pre>SUBSTR({string}, number of start position, length of string)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">TRIM</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This expression removes whitespace from the beginning and end of a string and is formatted as follows:</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><span class="bold">UPPER</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>This expression returns a string in upper case and is formatted as follows:</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>



##  

