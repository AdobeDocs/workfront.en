---
filename: use-mtls-in-http-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
---



# Use Mutual TLS in HTTP modules {#use-mutual-tls-in-http-modules}


*`Adobe Workfront Fusion`* requires an *`Adobe Workfront Fusion`* license in addition to an *`Adobe Workfront`* license.


## Mutual TLS overview {#mutual-tls-overview}

When you send data over the internet, it's important to ensure that it goes to or comes from the correct location and that only the intended recipient can read it. With TLS enabled, the client (computer requesting information) uses certificates to verify the identity of the server (computer providing information). This makes secure HTTP connections.


Mutual TLS allows this identity confirmation to go both ways. When the server sends its certificate to verify its identity to the client, it also requests the client's certificate. This ensures that the server does not send information to a site or user that would misuse it.

` `**Example: **`` 


*  `TLS`: When a person types "MyGreatBank.com" into a browser, they want to be sure that they are going to My Great Bank, not a website that might misuse or sell their banking information. They also want to be sure their bank account information is encrypted.


  When the browser (the client) connects to MyGreatBank.com (the server), TLS requires a certificate from MyGreatBank.com to verify its identity. The certificate is provided by a certificate authority such as DigiCert or Thawte. Because the browser trusts the certificate authority, it allows the connection.

*  `Mutual TLS`: MySoftware.com is a software client that needs information from the MyGreatBank.com API. MyGreatBank allows only trusted clients to connect to their servers. So, in addition to the regular TLS verifying the identity of MyGreatBank.com, the TLS/certificate authority process also verifies the request from MySoftware.com.




## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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


## Providing your *`Workfront Fusion`* public certificate {#providing-your-workfront-fusion-public-certificate}

When you connect to a web service with an HTTP request, the web service usually requires a *`Workfront Fusion`* public certificate for verification. This allows the web service to compare the certificate presented in the HTTP request to the one on file, as a way to ensure that the certificate is on the web service's allowlist.


For instructions on uploading the *`Adobe Workfront Fusion`* public certificate to a web service, see the web service's documentation.


You can use the following links to download the *`Workfront Fusion`* public certificates:



### Certificates for the year November 17, 2021 - November 17, 2022 {#certificates-for-the-year-november-november}




*  [Download *`Workfront Fusion`* Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com_certificate-chain-2022.crt) 
*  [Download *`Workfront Fusion`* EU Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app-eu_workfrontfusion_com_certificate-chain-2022.crt) 


  For use in the EU





### Certificates expiring November 16, 2021 {#certificates-expiring-november}




*  [Download *`Workfront Fusion`* Certificate](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com_certificate-chain.crt) 
*  [Download *`Workfront Fusion`* EU Certificate](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app-eu_workfrontfusion_com_certificate-chain.crt) 


  For use in the EU





>[!IMPORTANT] {type="important"}
>
>*`Workfront Fusion`* public certificates expire annually. After yours expires you will need to upload a new certificate to the web service. We recommend that you:
>
>
>
>*  Make note of the expiration date and set a reminder for yourself to upload the certificate to your web service.
>*  Bookmark this page to easily find the new certificates.
>
>





>[!NOTE]
>
>You may need to provide other information in addition to the certificate. For information on what a web service requires, see the web service's API documentation.




## Enabling Mutual TLS in *`Workfront Fusion`* HTTP modules {#enabling-mutual-tls-in-workfront-fusion-http-modules}

All *`Workfront Fusion`* HTTP request modules have the option to enable Mutual TLS. 


To enable Mutual TLS in an HTTP request module:



1.  Add an HTTP request module to your scenario.
1.  Begin configuring the module. 


   For instructions on configuring an HTTP request module, see the appropriate article under [HTTP modules](_http-modules.md).

1.  Enable `Show advanced settings` near the bottom of the module.
1.  Enable `Use Mutual TLS`.


