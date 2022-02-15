---
filename: math-functions
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
---



# Math functions {#math-functions}



## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> <p data-mc-conditions="SnippetConditions.HIDE"><span class="mc-variable WFVariables.WFFusionAutomation variable varname">Workfront Fusion for Work Automation</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## average ([array of values]) average(value1; [value2], ...) {#average-array-of-values-average-value-value}

Returns the average value of the numeric values in a specific array, or the average value of numerical values entered individually.


## ceil (number) {#ceil-number}

Returns the smallest integer greater than or equal to a specified number.

` `**Examples: **`` 


*  `ceil(`

  ```
  1.2
  ```

  `)` 


  Returns 2

*  `ceil(`

  ```
  4
  ```

  `)` 


  Returns 4





## floor (number) {#floor-number}

Returns the largest integer less than or equal to a specified number.

` `**Examples: **`` 


*  `floor(`

  ```
  1.2
  ```

  `)` 


  Returns 1

*  `floor(`

  ```
  1.9
  ```

  `)` 


  Returns 1






*  `floor(`

  ```
  4
  ```

  `)` 


  Returns 4





## formatNumber (number; decimalPOINTS; [decimalSeparator]; [thousandsSeparator]) {#formatnumber-number-decimalpoints-decimalseparator-thousandsseparator}

Returns a number in requested format. By default, the decimal point is a comma (,) and the thousands separator is a period (.).

` `**Example: **`` `formatNumber(`

```
123456789<span class="function">;</span>3<span class="function">;</span>,<span class="function">;</span>.
```

`)` 


Returns 123.456.789,000


## max ([array of values]), max(value1;value2; ...) {#max-array-of-values-max-value-value}

Returns the largest number in a specified array or the largest number among numbers entered individually.


## min ([array of values]), min(value1; value2; ...) {#min-array-of-values-min-value-value}

Returns the smallest number in a specified array or the smallest number among numbers entered individually.


## parseNumber (number; decimal separator) {#parsenumber-number-decimal-separator}

Parses a string with a number and returns the number. For example, parseNumber(1 756,456;,)


## round (number) {#round-number}

Rounds a numeric value to the nearest integer.

` `**Examples: **`` 


*  `round(`

  ```
  1.2
  ```

  `)` 


  Returns 1

*  `round(`

  ```
  1.5
  ```

  `)` 


  Returns 2






*  `round(`

  ```
  1.7
  ```

  `)` 


  Returns 2






*  `round(`

  ```
  2
  ```

  `)` 


  Returns 2





## sum ([array of values]), sum(value1; value2; ...) {#sum-array-of-values-sum-value-value}

Returns the sum of the values in a specified array or the sum of numbers entered individually.
