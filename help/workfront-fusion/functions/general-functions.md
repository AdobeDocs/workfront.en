---
filename: general-functions
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
---



# General functions {#general-functions}



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


## get (object or array; path) {#get-object-or-array-path}

Returns the value path of an object or array. To access nested objects, use dot notation. The first item in an array is index 1.

` `**Examples: **`` 


* `get(` `array` `;`

  ```
  1
  ```

  `+`

  ```
  1
  ```

  `)` 

* `get(` `array` `;`

  ```
  5.raw_name
  ```

  `)` 

* `get(` `object` `;`

  ```
  raw_name
  ```

  `)` 

* `get(` `object` `;`

  ```
  raw_name.sub_raw_name
  ```

  `)` 





## if (expression; value1; value2) {#if-expression-value-value}

Returns the value 1 if the expression is evaluated to true; otherwise it returns the value 2.

` `**Examples: **`` 


*  `if(`

  ```
  1
  ```

  `=`

  ```
  1
  ```

  `;`

  ```
  A
  ```

  `;`

  ```
  B
  ```

  `)` 


  Returns A

*  `if(` `=`

  ```
  2
  ```

  `;`

  ```
  A
  ```

  `;`

  ```
  B
  ```

  `)` 


  Returns B





## ifempty (value1; value2) {#ifempty-value-value}

Returns the value 1 if this value is not empty; otherwise it returns the value 2.

` `**Examples: **`` 


*  `ifempty(`

  ```
  A
  ```

  `;`

  ```
  B
  ```

  )


  Returns A

*  `ifempty(`

  ```
  unknown
  ```

  `;`

  ```
  B
  ```

  )


  Returns B

*  `ifempty(`

  ```
  ""
  ```

  `;`

  ```
  B
  ```

  )


  Returns B





## switch (expression; value1; result1; [value2; result2; ...]; [else]) {#switch-expression-value-result-value-result-else}

Evaluates one value (called the expression) against a list of values; returns the result corresponding to the first matching value.

` `**Examples: **`` 


*  `switch(`

  ```
  B
  ```

  `;`

  ```
  A
  ```

  `;`

  ```
  1
  ```

  `;`

  ```
  B
  ```

  `;`

  ```
  2
  ```

  `;`

  ```
  C
  ```

  `;`

  ```
  3
  ```

  `)` 


  Returns 2

*  `switch(`

  ```
  C
  ```

  `;`

  ```
  A
  ```

  `;`

  ```
  1
  ```

  ;

  ```
  B
  ```

  `;`

  ```
  2
  ```

  `;`

  ```
  C
  ```

  `;`

  ```
  3
  ```

  `)`


  Returns 3

*  `switch(`

  ```
  X<span class="function">;</span>A<span class="function">;</span>1<span class="function">;</span>B<span class="function">;</span>2<span class="function">;</span>C<span class="function">;</span>3<span class="function">;</span>4
  ```

  `)` 


  Returns 4





## omit(object; key1; [key2; ...]) {#omit-object-key-key}

Omits the given keys of the object and returns the rest.

` `**Example: **`` `omit(` `User` `;`password `)`


Returns a collection of the user's information, excluding the password.


## pick(object; key1; [key2; ...]) {#pick-object-key-key}

Picks only the given keys from the object.

` `**Example: **`` `pick(` `User` `;`password `;`email `)`


Returns a collection of only the user's password and email address.
&nbsp;
