---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: OpenAI(ChatGPT) modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use OpenAIT(ChatGPT), as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
---
# [!DNL OpenAI(ChatGPT)] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL OpenAI(ChatGPT)], as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] or higher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisites

To use [!DNL OpenAI(ChatGPT)] modules, you must have an [!DNL OpenAI(ChatGPT)] account, including an API key and Organization ID.

## Connecting [!DNL OpenAI(ChatGPT)] to [!DNL Workfront Fusion]

You can create a connection to your [!DNL OpenAI(ChatGPT)] account directly from inside an [!DNL OpenAI(ChatGPT)] module.

1. In any [!DNL OpenAI(ChatGPT)] module, click **[!UICONTROL Add]** next to the [!UICONTROL Connection] field.
1. Enter the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Enter a name for the new connection.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td>You can locate your API key in your OpenAI user settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Organization ID] </td> 
      <td>You can locate your Organization ID on your Organization Settings page in OpenAI.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.


## [!DNL OpenAI(ChatGPT)] modules and their fields

When you configure [!DNL OpenAI(ChatGPT)] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL OpenAI(ChatGPT)] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Create a Completion

This action module creates a completion for the provided prompt or chat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI(ChatGPT)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI(ChatGPT)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> ID of the model to use. You can use the Get models module to see all of your available models </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Temperature]</td> 
   <td> This value must be between 0 and 2, and determines the randomness of the output. Higher values produce output that is more random, while lower values produce more focused output. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the <a href="https://platform.openai.com/docs/api-reference/completions/create" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Create an Edit

This action module returns an edited version of a prompt you provide, following your instructions.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI(ChatGPT)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI(ChatGPT)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> ID of the model to use. You can use the Get models module to see all of your available models </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> Enter or map the text that you want to edit. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Instruction]</td> 
   <td> Enter or map the instructions for the edit. Example: "Fix the spelling mistakes." </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Enter or map the maximum number of edits you want the module to return during each scenario execution cycle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the <a href="https://platform.openai.com/docs/api-reference/edits/create" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


### Create Chat Completion

Given a list of messages describing a conversation, this action module returns a response.



### Create a Custom API Call

This action module a custom HTTP request to the OpenAI API.



### Generate Images

This action module generates or manipulates images with Dall-E models.



### Get Models

This module lists and describes the various models available in the OpenAI API.


