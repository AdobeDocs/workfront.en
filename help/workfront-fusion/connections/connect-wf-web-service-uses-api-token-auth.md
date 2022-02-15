---
filename: connect-wf-web-service-uses-api-token-auth
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
---



# Connect *`Adobe Workfront Fusion`* to a web service that uses API token authorization {#connect-adobe-workfront-fusion-to-a-web-service-that-uses-api-token-authorization}

Some services do not allow *`Adobe Workfront Fusion`* (and other integration platforms) to create an app that you can easily use in your scenario.


There is a workaround to this situation. You can connect the desired service (app) to *`Workfront Fusion`* using *`Workfront Fusion`*'s HTTP module.


This article explains how to connect almost any web service to *`Workfront Fusion`* using an API Key/API token.


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


## Connect to a web service that uses an API token {#connect-to-a-web-service-that-uses-an-api-token}

The procedure of connecting the service via an API token is similar for most web services.



1. Create an application on the web service's website, as explained in the section [Create a new application and obtain the API token](#create) in this article.
1. Obtain the API Key or API token.
1. Add *`Workfront Fusion`*'s HTTP > Make a Request module to your scenario.
1. Set up the module according to the web service's API documentation and running the scenario, as explained in the section [Set up the HTTP module](#set) in this article.




>[!NOTE]
>
>We will use the Pushover notification service as an example throughout this article.




## Create a new application and obtain the API token {#create-a-new-application-and-obtain-the-api-token}



>[!NOTE]
>
>There are many different ways that web services create and distribute API keys or API tokens. For instructions on obtaining an API key and token for your desired web service, go to the service's website and search for "API&nbsp;key" or "API token."
>
>
>We are including instructions for obtaining a Pushover API key only as an example of what you might find.






1. Log in to your Pushover account.
1.  Click `Create an Application/API Token` at the bottom of the page.
1.  Fill in the Application Information and click `Create an Application`.
1.  Store the provided API token in a safe place. You will need it for the *`Workfront Fusion`* HTTP > Make a Request module to connect to the desired web service (Pushover, in this case).




## Set up the HTTP module {#set-up-the-http-module}

To connect a web service to your *`Workfront Fusion`* scenario, you need to use the HTTP > Make a request module in the scenario and set up the module according to the web service's API&nbsp;documentation.



1.  Add the HTTP > Make a Request module to your scenario.
1.  To push a message using *`Workfront Fusion`*, set up the HTTP module as follows.


   >[!NOTE]
   >
   >These module settings correspond to the Pushover web service API documentation. Settings may be different for other web services. For example, the API token may be inserted to the Header and not to the Body field.



<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 149px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">URL</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>The URL field contains the endpoint that you can find in the web service's API documentation.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Method</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><code>POST</code> </p> <p>The used method depends on the corresponding endpoint. The Pushover endpoint for pushing messages uses the POST method.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Headers</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Some web services may use Headers to specify the API token authentication or other parameters. This is not the case in our example as the Pushover's endpoint for pushing messages uses Body (see below) for all request types.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Query String</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Some web services may use a Query String to specify other parameters. This is not the case in our example as the Pushover web service uses Body (see below) for all request types.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Body Type</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><code>Raw</code> </p> <p>This setting allows you to select the JSON content type in the Content Type field below.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Content Type</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><code>JSON (application/json)</code> </p> <p>JSON is the required content type by the Pushover app. This may differ from other web services.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"> <p>Request Content</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Enter the Body request content in the JSON format. You can use the JSON &gt; Create JSON module as explained in <a href="#json" class="MCXref xref">JSON Body Mapped Using the JSON &gt; Create JSON module</a> in this article. Or you can enter the JSON content manually, as explained in <a href="#json2" class="MCXref xref">JSON Body Entered Manually</a> in this article.</p> <p>See the web service's API documentation for the required parameters for that web service.</p> </td> 
  </tr> 
 </tbody> 
</table>






## JSON Body Entered Manually {#json-body-entered-manually}

Specify parameters and values in the JSON format.

` `**Example: **`` {"user":"12345c2ecu1hq42ypqzhswbyam34",


"token":"123459evz8aepwtxydndydgyumbfx",


"message":"Hello World!",


"title":"The Push Notification"}

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>user</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Your USER_KEY. This can be found in your Pushover dashboard.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">token </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Your API token/API Key that was generated you created your Pushover app.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">message </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The text content of the push notification that is sent to the device(s).</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">title </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>(Optional) Your message's title. If no value is entered, your app's name is used. </p> </td> 
  </tr> 
 </tbody> 
</table>



## JSON Body Mapped Using the JSON > Create JSON module {#json-body-mapped-using-the-json-create-json-module}

The Create JSON module makes the specifying JSON easier. It also gives you the possibility to define values dynamically.


For more information about the JSON modules, see [JSON modules](json-modules.md).



1.  Enter or map the values you want to create JSON from.


   ![](assets/json-values-350x288.png)



1.  Connect the JSON > Create JSON module to the HTTP > Make a Request module.
1.  Map the JSON string from the Create JSON module to the Request content field in the HTTP > Make a Request module.


   Now when you run the scenario, the push notification is sent to the device that has been registered in your Pushover account.



