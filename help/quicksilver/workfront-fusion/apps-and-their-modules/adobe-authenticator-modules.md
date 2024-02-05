---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Authenticator module
description: With the Adobe Authenticator module, you can connect to any Adobe product with an API, using a single connection.
author: Becky
feature: Workfront Fusion
---
# Adobe Authenticator modules

The Adobe Authenticator module allows you to connect to any Adobe API, using a single connection. This allows you to more easily connect to Adobe products that do not yet have a dedicated Fusion connector.

The advantage over the HTTP modules is that you can create a connection, as in a dedicated app.

To see a list of available Adobe APIs, see X. You may be able to use only the APIs to which you are assigned.

## Access requirements

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan</td>
      <td>
        <p>New: Any</p><p>Or</p><p>Current: [!UICONTROL Pro] or higher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license</td>
      <td>
        <p>New: Standard</p><p>Or</p><p>Current: [!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] license</td>
      <td>
   <p>Current Fusion license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy Fusion license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>
   <p>New Workfront plan: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Current Workfront plan: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td>
    </tr>
  </tbody>
</table>

## Prerequisites

* You must have access to the Adobe product that you want the module to connect to.
* You must have access to the Adobe Developer Console.
* You must have a project on the Adobe Developer Console that includes the API that you want the module to connect to. You can:

   * Create a new project with the API.

       Or
   * Add the API to an existing project.

  For information on creating or adding an API to a project on the Adobe Developer Console, see [Create a project](https://developer.adobe.com/dep/guides/dev-console/create-project/) in the Adobe documentation.

## Create a connection

An Adobe Authenticator connection connects to a single project on the Adobe Developer Console. To use the same connection for more than one Adobe API, add the APIs to the same project, and create a connection to that project.

You can create separate connections to separate projects, but you cannot use a connection to access an API that is not on the project specified in that connection.

>[!IMPORTANT]
>
>With the Adobe Authenticator connector, you have the choice between making an OAuth Server-to-server connection, or a Service Account (JWT) connection. Adobe has deprecated JWT credentials, which will stop working after January 1, 2025. **Therefore, we highly recommend creating OAuth connections.**
>
>For more information on these types of connections, see [Server to Server authentication](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) in the Adobe documentation

To create a connection:

1. In any Adobe Authenticator module, click **Add** next to the Connection field.
1. Fill in the following fields:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>Select whether you want to create an OAuth Server-to-Server connection, or a service account (JWT) connection.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Enter a name for this connection.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Enter your [!DNL Adobe] Client ID. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Enter your [!DNL Adobe] Client Secret. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Scopes]</td>
        <td>If you have selected an OAuth connection, enter the scopes needed for this connection.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Enter your [!DNL Adobe] Technical account ID. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>If you have selected a JWT connection, enter your [!DNL Adobe] Organization ID. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>If you have selected a JWT connection, enter the meta scopes needed for this connection. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>If you have selected a JWT connection, enter the private key that was generated when your credentials were created in the [!DNL Adobe Developer Console]. </p>
          <p>To extract your private key or certificate:</p>
          <ol>
            <li value="1">
              <p>Click <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Select the type of file you are extracting.</p>
            </li>
            <li value="3">
              <p>Select the file that contains the private key or certificate.</p>
            </li>
            <li value="4">
              <p>Enter the password for the file.</p>
            </li>
            <li value="5">
              <p>Click <b>[!UICONTROL Save]</b> to extract the file and return to the connection setup.</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Select whether you are connecting to a production or non-production environment.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Select whether you are connecting to a service account or a personal account.</td>
      </tr>
    </tbody>
    </table>

1. Click **[!UICONTROL Continue]** to save the connection and return to the module.

## Module

### Make a custom API call

This action module allows you to make a call to any Adobe API.

>[!TIP]
>
>You must enter the entire URL for the API you want to connect to. This module does not accept relative URLs.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>For instructions on creating a connection to the Adobe Authenticator module, see <a href="#create-a-connection" class="MCXref xref" >Create a connection</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Enter the entire URL of the API point you want to connect to.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion adds authorization headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Enter the request query string.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Enter the maximum number of results that you want the module to return in one execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

