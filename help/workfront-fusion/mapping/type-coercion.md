---
filename: type-coercion
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
---



# Type coercion {#type-coercion}



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


### Type coercion {#type-coercion-1}

This document describes how *`Adobe Workfront Fusion`* behaves in situations when it receives values in expected and unexpected data formats.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Expected</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Received</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p>Description</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">array </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">array </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">array </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">other </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>If the received value is not of the array type, <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> will create an array and the first (and the only) element will be the received value.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">number </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The value is converted to logical Yes, even if the value is 0.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>If the value is equal to false or the value is empty, it is converted to logical No. If not, it is converted to logical Yes.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">other </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The value is converted to logical Yes whenever the received value exists (is not null).</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">buffer </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">buffer </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is handed over unchanged only if the codepage is as expected. If the codepage differs, <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> will try to convert the received value to the requested codepage. If this conversion is not supported, <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> will return a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">buffer </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The value is converted to text (true/false) and then to binary data following the steps mentioned above for converting to text.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">buffer </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">date </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is converted to ISO 8601 text and then to binary data following the steps mentioned for converting to text.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">buffer </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">number </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The value is converted to text and then to binary data following the steps mentioned above for converting to text.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">buffer </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is converted to binary data and encoded as expected. If the expected encoding is not specified, utf8 encoding will be used.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">buffer </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">other </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">collection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">collection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">collection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">other </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">date </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">date </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">date </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> will try to convert the text to a date. If the conversion fails, it will return a validation error. Date must contain day, month and year. Date may contain time and time zone. Default time zone is based on your settings. Examples:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">date </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">other </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">number </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">number </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">number </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> will try to convert the text to a number. If the conversion fails, it will return a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">number </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">other </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">array </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>If the given array supports conversion to text, the value will be converted. If not, <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> will return a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is converted to text (true/false).</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">buffer </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>If text encoding is specified for binary data, the value will be converted to text. If not, <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> will return a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">date </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value is converted to ISO 8601 text.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">number </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The value is converted to text.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">other </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">time </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">time </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">time </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">text </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> will try to convert time to the hours:minutes:seconds format. If the conversion fails, it will return a validation error.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">time </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">other </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
 </tbody> 
</table>

