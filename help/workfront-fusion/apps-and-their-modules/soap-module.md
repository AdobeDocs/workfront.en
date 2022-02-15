---
filename: soap-module
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
---



# SOAP module {#soap-module}

You can use the SOAP module to connect to SOAP APIs.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Using the SOAP module {#using-the-soap-module}

The SOAP module is currently in beta and does not support:



* Redefine elements
* Fraction digits restrictions
* Total digits restrictions
* White space restrictions
* Multiple parts in input and output messages. Only single part messages are supported
*  Custom XML Schema elements defined with the help of SOAP Encoding (http://schemas.xmlsoap.org) schemas and elements.

  ` `**Example: **`` The following would not be recognized correctly by *`Workfront Fusion`*:
  `<pre><complexType name="ArrayOfFloat"></pre>` `<blockquote> <pre><complexContent></pre> </blockquote>` `<blockquote>  <blockquote>  <pre><restriction base="soapenc:Array"></pre>  </blockquote> </blockquote>` `<blockquote>  <blockquote>   <blockquote>   <pre><attribute ref="soapenc:arrayType"</pre>   </blockquote>  </blockquote> </blockquote>` `<blockquote>  <blockquote>   <blockquote>    <blockquote>     <blockquote>     <pre>wsdl:arrayType="xsd:integer[]"/></pre>     </blockquote>    </blockquote>   </blockquote>  </blockquote> </blockquote>` `<blockquote>  <blockquote>  <pre></restriction></pre>  </blockquote> </blockquote>` `<blockquote> <pre></complexContent></pre> </blockquote>``<pre></complexType></pre>` It includes the 

  ```
  soapenc:Array
  ```

  , 

  ```
  soapenc:arrayType
  ```

  and 

  ```
  wsdl:arrayType
  ```

  references, which are not yet supported in *`Workfront Fusion`*.





## Workaround {#workaround}

If the SOAP module refuses to process the WSDL file or throws various errors in the module's configuration, you may try using the universal `HTTP > Make a request` module instead:



1. In *`Workfront Fusion`*, create a new scenario.
1. Insert the `HTTP > Make a request` module in the scenario.
1.  Open the module's configuration and configure it like shown below:


   ![](assets/workaround-350x443.png)



1. Open a new web browser window or tab.
1.  Paste the WSDL URL into the web browser's address bar and fetch the XML file. 


   The WSDL URL usually ends with 

   ```
   ?wsdl
   ```

   , but not necessarily, for example http://voip.ms/api/v1/server.wsdl.

1. If the WSDL file does not display directly in the web browser, open the downloaded file in a text editor.
1.  Search for the 

   ```
   <service>
   ```

   or 

   ```
   <wsdl:service>
   ```

   tag:


   ![](assets/service-350x65.png)



1. Once located, copy the URL from the 

   ```
   location
   ```

   attribute.
1. In *`Workfront Fusion`*, paste the URL into the HTTP module's URL field.
1. Open the [Online SOAP Client](https://wsdlbrowser.com/) in a new web browser window/tab.
1. Paste the WSDL URL into the WSDL URL field.
1. Click `Browse`.
1. Pick from the list of functions to the left, for example 

   ```
   getLanguages
   ```

   .
1. Copy the content of the Request XML text area.
1. In *`Workfront Fusion`*, paste the copied content to the module's URL field.
1.  Provide values for selected parameters by replacing the question marks with actual values:


   ![](assets/request-xml-350x172.png)



1. Close the module's configuration by clicking `OK`.
1. Execute the scenario or module.


