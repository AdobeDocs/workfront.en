---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Use cURL to add an HTTP module
description: The Adobe Workfront Fusion documentation has moved to a new location. This article has been deprecated, but contains a link to the new article that covers this functionality.
author: Becky
feature: Workfront Fusion
exl-id: 5eac3e87-0dd3-4bad-ae3e-77264329b717
---
# Use cURL to add an HTTP module

>[!IMPORTANT]
>
>The Adobe Workfront Fusion documentation has moved to a new location. 
>
>The information in this article can now be found in the article:
>
>* [Use cURL to add an HTTP module](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/use-curl-create-http.html)
>
>Please update any bookmarks.
>
>This article is no longer being updated, and will be removed in the near future.

You can paste a cURL request into your scenario, and Fusion creates an HTTP module configured from the cURL request.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to use the functionality in this article: 

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront plan</td>  
      <td>Any</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront license</td>  
      <td>
        New: Standard<br>
        Or<br>
        Current: Work or higher
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion license</td>  
      <td> 
        Current: No Workfront Fusion license requirement.<br>
        Or<br>
        Legacy: Any
      </td>  
    </tr>  
    <tr>  
      <td>Product</td>  
      <td> 
        New: Select or Prime Workfront Plan: Your organization must purchase Adobe Workfront Fusion.<br>
        Ultimate Workfront Plan: Workfront Fusion is included.<br>
        Or<br>
        Current: Your organization must purchase Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table> 

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md). 

+++

## Create an HTTP module from a cURL request


To create an HTTP module using cURL:

1. Create the text of the cURL request outside of Fusion, such as in a text editor.

   >[!IMPORTANT]
   >
   >If you are using Fusion on a Windows machine, your cURL request must not include line breaks. 
1. Copy the cURL request to your clipboard.
1. Click the **[!UICONTROL Scenario]** tab in the left panel.
1. Select the scenario where you want to create the module.
1. Click anywhere on the scenario to enter the Scenario editor.
1. Right click on any white space in the scenario editor and select **Paste**.

   Or

   Press Ctrl + V (Windows) or Cmd + V (Mac).
   

   An HTML module is created.
1. Drag the module to connect it to your scenario.

## Troubleshooting

If your cURL is not pasting into your scenario, check the following:

* Check your browser settings to ensure that pasting from the clipboard is enabled.
* If you are running Windows, check the cURL request to ensure that it does not include line breaks.
