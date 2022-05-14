---
filename: google-slides-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Slides modules
description: The Adobe Workfront Fusion Google Slides modules allow you to create, update, list, and/or delete presentations and upload images to presentations in your Google Slides account.
---

# Google Slides modules

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

The Adobe Workfront Fusion Google Slides modules allow you to create, update, list, and/or delete presentations and upload images to presentations in your Google Slides account.

In order to use Google Slides with Workfront Fusion, it is necessary to have a Google account. If you don't have a Google account yet, you can create one at the Google Account help page.

You also need Google Slides in your Google Drive.

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
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
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Google Slides modules, you must have a Google account.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Connect Google Slides to Workfront Fusion</h2>
-->

   <!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to Workfront Fusion and open the Google Slides module's Create a connection dialog.</li>
   -->

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Continue</strong>, then click <strong>Allow</strong>.</li>
   -->

## Google Slides modules and their fields

When you configure Google Slides modules, Workfront Fusion displays the fields listed below. Along with these, additional Google Slides fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Presentation](#presentation) 
* [Other](#other)

### Presentation {#presentation}

* [Watch Presentations](#watch-presentations) 
* [List Presentations](#list-presentations) 
* [Get a Presentation](#get-a-presentation) 
* [Get a Page/Thumbnail](#get-a-page-thumbnail) 
* [Create a Presentation From a Template](#create-a-presentation-from-a-template) 
* [Upload an Image To a Presentation](#upload-an-image-to-a-presentation) 
* [Refresh a Chart](#refresh-a-chart) 
* [Add/Delete a Slide](#add-delete-a-slide)

#### Watch Presentations {#watch-presentations}

Triggers when a new presentation is created or updated.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch </td> 
   <td> <p>Select the option to watch the presentations:</p> 
    <ul> 
     <li> <p>Created Date</p> </li> 
     <li> <p>Modified Date</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>The maximum number of presentations Workfront Fusion should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Presentations {#list-presentations}

Retrieves a list of all presentations.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a drive location</td> 
   <td> <p>Select the Google Drive where the presentations you want to list are located:</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared With Me</li> 
     <li>Google Shared Drive</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder ID</td> 
   <td> <p>Choose the folder location of the presentations you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>The maximum number of presentations Workfront Fusion should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Presentation {#get-a-presentation}

Gets the latest version of a specified presentation.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a drive</td> 
   <td> <p>Select the Google Drive where the presentations you want to list are located:</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared With Me</li> 
     <li>Google Shared Drive</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Presentation ID</td> 
   <td> <p> Select the presentation that you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Page/Thumbnail {#get-a-page-thumbnail}

Gets the latest version of the specified page or of the thumbnail of a page in the presentation.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Presentation ID</td> 
   <td> <p> Select the Presentation ID that you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Page Object ID</td> 
   <td> <p> Select the slide for which you want to view the page object details.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Show Page Thumbnail</td> 
   <td> <p> Select the checkbox if you want to view the page thumbnail information.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Presentation From a Template {#create-a-presentation-from-a-template}

Creates a new presentation by replacing all tags like {{Name}}, {{Email}} in a template with provided data.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Title </td> 
   <td> <p>Enter a name for the new presentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Copy a Presentation</td> 
   <td> <p> Select the option if you are copying an existing presentation:</p> 
    <ul> 
     <li>By Mapping</li> 
     <li>By Dropdown</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Copy of Existing Presentation ID</td> 
   <td> <p> Enter the Path or Presentation ID of an existing presentation which you want to copy. This field appears if you are creating the presentation By Mapping.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a drive</td> 
   <td> <p>Select the Google Drive where the presentations you want to list are located:</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared With Me</li> 
     <li>Google Shared Drive</li> 
    </ul> <p>This field appears if you are creating the presentation By Dropdown.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Presentation ID</td> 
   <td> <p> Select the Presentation ID whose of the presentation you want to use as a template.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Values </td> 
   <td> <p>Add the values:</p> 
    <ul> 
     <li><strong>Tag</strong>: Enter the tag you want to replace in the presentation. For example, {{Name}}</li> 
     <li><strong>Replaced Value</strong>: Enter the value with which the existing tag is to be replaced. For example, if a string <code>{{Name}}</code> in the presentation and the replaced value is Sample, then the <code>{{Name}}</code> will be replaced by <code>Sample</code>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">New Drive Location</td> 
   <td> <p>Select the Google Drive where you want to store or add the new presentation:</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared With Me</li> 
     <li>Google Shared Drive</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>New Document's Location</p> </td> 
   <td> <p>Select the folder where you want to store or add the presentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Shared </td> 
   <td> <p>Select if you want to share the presentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sharing with Other's Email Address</td> 
   <td> <p> Enter the email address with whom you want to share the presentation. If you are not entering an email address and selecting only shared field, the presentation is shareable to anyone.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Upload an Image To a Presentation {#upload-an-image-to-a-presentation}

Uploads an image with provided data.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Presentation</td> 
   <td> <p>Choose how you want to select the presentation that you are uploading an image to.</p> 
    <ul> 
     <li>By Mapping</li> 
     <li>By Dropdown</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a drive</td> 
   <td> <p>Select the Google Drive where the presentations you want to list are located:</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared With Me</li> 
     <li>Google Shared Drive</li> 
    </ul> <p>This field appears if you are creating the presentation By Dropdown.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Presentation ID</td> 
   <td> <p> Select the Presentation ID of the presentation that you are uploading an image to.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Values</td> 
   <td> <p>Values Add the values:</p> 
    <ul> 
     <li><strong>Tag</strong>: Enter the tag to which you want to add the URL.</li> 
     <li><strong>Image URL</strong>: Enter the path or URL to the image you want to upload.</li> 
    </ul> <p>Note: The images must be less than 50MB in size, cannot exceed 25 megapixels, and must be in PNG, JPEG, or GIF format.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Refresh a Chart {#refresh-a-chart}

Refreshes the chart data stored in a presentation specified by ID.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a drive</td> 
   <td> <p>Select the Google Drive where the presentations you want to list are located:</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared With Me</li> 
     <li>Google Shared Drive</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Presentation ID</td> 
   <td> <p>Select the Presentation ID of the presentation that includes chart you want to refresh.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Chart Object ID</td> 
   <td> <p> Select the Chart you want to refresh.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Add/Delete a Slide  {#add-delete-a-slide}

Creates an empty slide or deletes an existing slide on the specified presentation.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Select the method</td> 
   <td> <p>Choose whether you want to add a new slide or delete a slide.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Presentation ID</td> 
   <td> <p>Select the Presentation ID of the presentation for which you want to add or delete a slide.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Predefined layout type</td> 
   <td> <p> Select the predefined slide layout that you want your added slide to use. Specify values for any additional fields (such as Title).</p> 
    <ul> 
     <li>Blank layout, with no placeholders</li> 
     <li>Layout with a caption at the bottom</li> 
     <li>Layout with a title and subtitle</li> 
     <li>Layout with a title and body</li> 
     <li>Layout with a title and two columns</li> 
     <li>Layout with only a title</li> 
     <li>Layout with a section title</li> 
     <li>Layout with a title and subtitle on one side and description on the other</li> 
     <li>Layout with one title and one body, arranged in a single column</li> 
     <li>Layout with a main point</li> 
     <li>Layout with a big number heading</li> 
    </ul> <p>This field is available if you selected to add a slide.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Other {#other}

* [Make an API Call](#make-an-api-call) 
* [Insert Links in a Presentation](#insert-links-in-a-presentation)

#### Make an API Call {#make-an-api-call}

Performs an arbitrary authorized API call.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Enter a path relative to https://developers.google.com/slides/. E.g. Presentation.</p> <p>For the list of available endpoints, refer to the <a href="https://developers.google.com/slides/reference/rest">Google Slides API Documentation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Enter the desired request headers. You don't need to add authorization headers.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p> Enter the request query string.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Example:** Using an API call you can get the presentation details for the presentation ID you have entered. You can find the presentation ID in the URL when you the open the presentation in Google Slides.

![](assets/api-call-350x13.png)

The following API call returns the presentation details:

![](assets/presentation-details.png)

Matches of the search can be found in the module's Output under Bundle > Body > presentationId.

In our example, the requested presentation details were returned:

![](assets/presentation-details-2.png)

#### Insert Links in a Presentation {#insert-links-in-a-presentation}

This module makes all links in a presentation clickable, or inserts a link into all matched input texts.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google Slides account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Presentation</td> 
   <td> <p>Choose how you want to select the presentation that you are uploading an image to.</p> 
    <ul> 
     <li>By Mapping</li> 
     <li>By Dropdown</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a drive</td> 
   <td> <p>Select the Google Drive where the presentations you want to list are located:</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared With Me</li> 
     <li>Google Shared Drive</li> 
    </ul> <p>This field appears if you are creating the presentation By Dropdown.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Presentation ID</td> 
   <td> <p>Choose the folder location of the presentations you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Select</td> 
   <td> <p>Select whether you want to make all links in a presentation clickable, or whether you want to insert a link into all match input texts.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Text Inputs</td> 
   <td>For each text item that you want to add a link for, add the item as well as its associated link to the list. Every time the item appears in the presentation, it will automatically be linked to the specified site.</td> 
  </tr> 
 </tbody> 
</table>

