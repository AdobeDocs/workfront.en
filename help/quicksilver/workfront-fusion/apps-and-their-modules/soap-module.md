---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: SOAP module
description: You can use the SOAP module to connect to SOAP APIs in Adobe Workfront Fusion.
feature: Workfront Fusion
---

# SOAP module

You can use the SOAP module to connect to SOAP APIs in Adobe Workfront Fusion.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
    </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Using the SOAP module

The SOAP module is currently in beta and does not support:

* Redefine elements
* Fraction digits restrictions
* Total digits restrictions
* White space restrictions
* Multiple parts in input and output messages. Only single part messages are supported
* Custom XML Schema elements defined with the help of SOAP Encoding (http://schemas.xmlsoap.org) schemas and elements.

**Example:** 
  
The following would not be recognized correctly by Workfront Fusion:

```
<complexType name="ArrayOfFloat">

   <complexContent>

      <restriction base="soapenc:Array">

         <attribute ref="soapenc:arrayType"

            wsdl:arrayType="xsd:integer[]"/>

      </restriction>

   </complexContent>

</complexType>
```

It includes the `soapenc:Array`, `soapenc:arrayType` and `wsdl:arrayType` references, which are not yet supported in Workfront Fusion.

## Workaround

If the SOAP module refuses to process the WSDL file or throws various errors in the module's configuration, you may try using the universal **HTTP > Make a request** module instead:

1. In Workfront Fusion, create a new scenario.
1. Insert the **HTTP > Make a request** module in the scenario.
1. Open the module's configuration and configure it like shown below:

   ![](assets/workaround-350x443.png)

1. Open a new web browser window or tab.
1. Paste the WSDL URL into the web browser's address bar and fetch the XML file.

   The WSDL URL usually ends with `?wsdl`, but not necessarily, for example `http://voip.ms/api/v1/server.wsdl`.

1. If the WSDL file does not display directly in the web browser, open the downloaded file in a text editor.
1. Search for the `<service>` or `<wsdl:service>` tag:

   ![](assets/service-350x65.png)

1. Once located, copy the URL from the `location` attribute.
1. In Workfront Fusion, paste the URL into the HTTP module's URL field.
1. Open the [Online SOAP Client](https://wsdlbrowser.com/) in a new web browser window/tab.
1. Paste the WSDL URL into the WSDL URL field.
1. Click **Browse**.
1. Pick from the list of functions to the left, for example `getLanguages`.
1. Copy the content of the Request XML text area.
1. In Workfront Fusion, paste the copied content to the module's URL field.
1. Provide values for selected parameters by replacing the question marks with actual values:

   ![](assets/request-xml-350x172.png)

1. Close the module's configuration by clicking **OK**.
1. Execute the scenario or module.
