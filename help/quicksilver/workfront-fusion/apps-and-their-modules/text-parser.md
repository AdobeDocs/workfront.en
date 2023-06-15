---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Text parser
description: You can use the Text parser tool to parse text for use in other [!DNL Adobe Workfront Fusion] scenario modules. The Text parser does not require a connection.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
---
# [!UICONTROL Text parser]

You can use the [!UICONTROL Text parser tool] to parse text for use in other [!DNL Adobe Workfront Fusion] scenario modules. The [!UICONTROL Text parser] does not require a connection.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Text parser] modules and their fields

When you configure [!UICONTROL Text parser] modules, [!DNL Adobe Workfront Fusion] displays the fields listed below. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformers

* [[!UICONTROL Get Elements from HTML]](#get-elements-from-html)
* [[!UICONTROL Get Elements from text]](#get-elements-from-text)
* [[!UICONTROL HTML to Text]](#html-to-text)
* [[!UICONTROL Match Pattern]](#match-pattern)
* [[!UICONTROL Replace]](#replace)

#### [!UICONTROL Get Elements from HTML]

Retrieves the desired elements from HTML code.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module finds no matches]</td> 
   <td> <p>Enable this option to ensure that the module does not stop the scenario if it returns no results.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Element type]</td> 
   <td> <p> Select the type of element you want to retrieve from the HTML code. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL iFrame element(s)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Enter or map the HTML code you want to retrieve the specified element types from.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Elements from text]

Parses elements from text based on the given pattern.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Input text]</td> 
   <td> <p>Enter or map the text you want to parse.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>Select the pattern that reflects the elements you want to parse from the text.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignore Duplicate Occurrences]</td> 
   <td> <p>Check this box to ignore duplicate occurrences of a text element.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML to Text]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Enter the HTML code you want to convert to plain text.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Line break] </td> 
   <td> <p>Select the type of newline (line break).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Uppercase headings]</p> </td> 
   <td> <p>Enable this option to convert text enclosed in the heading tags (such as &lt;h2> &lt;/h2>) into uppercase text.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Match Pattern]

The [!UICONTROL Match pattern] module enables you to find and extract string elements matching a search pattern from a given text. This module uses regular expressions (also known as regex or regexp).

A regular expression is a sequence of characters in which each character is either a metacharacter, having a special meaning, or a regular character that has a literal meaning. These character and metacharacters identify a pattern that can be used to search text. For example, if you wanted to search for names, you could set up a regular expression to search for a pattern that consists of two consecutive words that begin with capital letters. Regular expressions are a powerful tool for searching and manipulating text.

A discussion of regular expressions is beyond the scope of this article. We recommend the following resources:

* For the complete list of metacharacters, see [Regular expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) in MDN web docs.
* For a tutorial on how to create regular expressions, we recommend [RegexOne](https://regexone.com/).
* For experimenting with regular expressions, we recommend the [Regular Expressions 101](https://regex101.com/) website. Select the ECMAScript (JavaScript) FLAVOR in the left panel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Enter the regular expression pattern. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extracts all numerals in the provided text.</p> <p>Note:  <p>The pattern should contain at least one capture group in parenthesis <code>()</code>. If the pattern does not contain any capture groups, the output bundle is empty.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Enable this option to retrieve all matches in the text. Each match is output in a separate bundle. If this option is disabled, the module retrieves only the first entry.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Enable this option for this module to treat text as case-sensitive.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Enable this option to ensure that beginning and end metacharacters (<code>^</code> and <code>$</code>) matches the beginning or end of each line, not just the very beginning or end of the whole input string.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Enable this option to ensure that the period (.) matches newline characters (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p>Enable this option to ensure that the module does not stop the scenario if it returns no results.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Enter or map the text you want to match the pattern.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Replace]

Searches the entered text for a specified value or regular expression and replaces the result with the new value.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Enter the search term. You can also use a regular expression. For more details about the regular expression refer to the <a href="#match-pattern" class="MCXref xref">[!UICONTROL Match Pattern]</a> module.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New value]</td> 
   <td> <p> Enter a value that replaces the search term.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Enable this option to retrieve all matches in the text. Each match is output in a separate bundle. If this option is disabled, the module retrieves only the first entry.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Enable this option for this module to treat text as case-sensitive.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Enable this option to ensure that beginning and end metacharacters (<code>^</code> and <code>$</code>) matches the beginning or end of each line, not just the very beginning or end of the whole input string.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Enable this option to ensure that the period (.) matches newline characters (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Enter the text to be searched.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Data Scraping

Data scraping, sometimes called web scraping, data extraction, or web harvesting, is the process of collecting data from websites and storing it in your local database or spreadsheets. If you want to scrape data from a website and you are not familiar with regular expressions, you may use a data scraping tool.

If the data scraping tool provides a REST API, you can connect to it via our universal [[!UICONTROL HTTP] modules](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) and [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) modules.
