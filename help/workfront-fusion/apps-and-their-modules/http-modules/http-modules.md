---
filename: http-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
---



# HTTP > Other modules {#http-other-modules}


*`Adobe Workfront Fusion`* requires an *`Adobe Workfront Fusion`* license in addition to an *`Adobe Workfront`* license.
The HTTP app provides various modules for communication based on Hypertext Transfer Protocol (HTTP) protocol. HTTP is the foundation of data communication for the World Wide Web. You can use the modules to download web pages and files, call webhooks and API endpoints, and so on.


The right choice of the module depends on the authentication/ authorization mechanism the resource you want to access employs.&nbsp;The following are examples of modules



* Make a request:universal module primarily intended for resources not employing any type of authentication/ authorization
* Make a Basic Auth request:for resources employing HTTP Basic authentication (BA)
* Make a OAuth 2.0 request: for resources employing OAuth 2.0 authorization protocol
*  Make a Client Certificate Auth request: for resources employing authorization protocol that requires a client-side certificate.
*  Make an API Key authorization request: for resources employing API Keys for authorization.




## Request modules {#request-modules}

See the following articles for specific request module instructions:



*  [HTTP > Make a request module](http-module-make-a-request.md) 
*  [HTTP > Make a Basic Authorization request module](http-module-make-a-basic-auth-request.md) 
*  [HTTP > Make an OAuth 2.0 request module](http-module-make-an-oauth-2-request.md) 
*  [HTTP > Make a Client Certificate Authorization request module](http-module-make-a-client-cert-auth-request.md) 
*  [HTTP > Make an API Key Authorization request](http-module-make-an-api-key-auth-request.md) 




## Other action modules {#other-action-modules}




*  [Get a File](#get) 
*  [Resolve a target URL](#resolve) 




### Get a File {#get-a-file}

This action module downloads a file from the specified URL. After the file is downloaded, you can further process the file (map the file data) using other modules in the scenario.

<table style="width: 717px;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">URL </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Enter or map the URL of the file you want to download. </p> </td> 
  </tr> 
 </tbody> 
</table>



### Resolve a target URL {#resolve-a-target-url}

This action module resolves a chain of HTTP redirects and returns a target URL.

<table style="width: 717px;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">URL </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Enter or map the URL you want to resolve, such as a bit.ly URL.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray">Method </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select whether you want to use the HEAD method or the GET method.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Iterator modules {#iterator-modules}



### Retrieve headers {#retrieve-headers}

This module returns each header (name and value) from the specified HTTP module in a separate bundle.

<table style="width: 717px;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">Source Module</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p> Select the module you want to retrieve headers from.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Generating JSON Web Tokens (JWT) {#generating-json-web-tokens-jwt}

It is possible to generate a JWT token with the help of built-in functions:


Header:


Code for copy&paste:
`<pre>{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}</pre>` Payload:


![](assets/jwt-payload-350x17.png)




Code for copy&paste:
`<pre>{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}</pre>` Token:


![](assets/jwt-token-350x15.png)




Code for copy&paste:
`<pre>{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}</pre>`  