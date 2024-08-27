---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Figma modules
description: With the [!DNL Adobe Workfront Fusion] Figma modules, you can retrieve lists of comments, files, file versions, or projects. You can also post a comment or make a call to the Figma API.
author: Becky
feature: Workfront Fusion
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
---
# [!DNL Figma] Modules

With the [!DNL Adobe Workfront Fusion] [!DNL Figma] modules, you can retrieve lists of comments, files, file versions, or projects. You can also post a comment or make a call to the [!DNL Figma] API.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] or higher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>
      <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td>
    </tr>
  </tbody>
</table>


To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisites

To use [!DNL Figma] modules, you must have a [!DNL Figma] account.

## [!DNL Figma] modules and their fields

When you configure [!DNL Figma] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Figma] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Comments](#comments)

* [Projects and files](#projects-and-files)

* [Components and styles](#components-and-styles)

* [Other](#other)


### Comments

* [Delete a comment](#delete-a-comment)

* [List comments](#list-comments)

* [Post a comment](#post-a-comment)


#### [!UICONTROL Delete a comment]

This action module deletes a single comment from a file.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>For instructions about connecting your [!DNL Figma] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>Enter or map the File ID of the file that you want to add a delete a comment from. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>Enter the text of the comment you want to delete.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List comments]

This search module lists all of the comments attached to a single file in [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>For instructions about connecting your [!DNL Figma] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Enter or map the File ID of the file that you want to retrieve comments for. </p>
        <ul>
          <li>
            <p>If you do not know the ID, click <b>[!UICONTROL Find Files]</b> and enter or map the ID of the project that the file is associated with, then select the file.</p>
          </li>
          <li>
            <p>If you do not know the project's ID, click <b>[!UICONTROL Find Projects]</b> and enter or map the ID of the team that owns the project the file is associated with, then select the project, then select the file.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Enter or map the maximum number of comments you want the module to return during each scenario execution cycle.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Post a comment]

This action module posts a comment to a Figma file.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>For instructions about connecting your [!DNL Figma] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Enter or map the File ID of the file that you want to post a comment to. </p>
        <ul>
          <li>
            <p>If you do not know the file's ID, click <b>[!UICONTROL Find Files]</b> and enter or map the ID of the project that the file is associated with, then select the file.</p>
          </li>
          <li>
            <p>If you are attempting to find the file's ID and do not know the project's ID, click <b>[!UICONTROL Find Projects]</b> and enter or map the ID of the team that owns the project the file is associated with. Select the project, then select the file.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>Enter the text of the comment.</td>
    </tr>
  </tbody>
</table>


### Projects and files

* [Get a file or image](#get-a-file-or-image)

* [List file version history](#list-file-version-history)

* [List project files](#list-project-files)

* [List projects](#list-projects)


#### [!UICONTROL Get a file or image]

This action module retrieves a single file or image from a Figma library

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>For instructions about connecting your [!DNL Figma] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>
        <p>Select the type of object you want to retrieve.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL File]</b>
            </p>
            <p>The module returns the document referred to by [!UICONTROL Key] as a JSON object. The file key can be parsed from any Figma file URL.</p>
            <p>For fields, see <a href="#Get2" class="MCXref xref" >[!UICONTROL Get a file or image: File]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL File nodes]</b>
            </p>
            <p>Returns the nodes referenced to by IDs as a JSON object. The nodes are retrieved from the [!DNL Figma] file referenced to by [!UICONTROL Key].</p>
            <p>For fields, see <a href="#Get3" class="MCXref xref" >[!UICONTROL Get a file or image: File nodes]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image]</b>
            </p>
            <p>The module renders images from a file.</p>
            <p>For fields, see <a href="#Get4" class="MCXref xref" >[!UICONTROL Get a file or image: Image]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image fills]</b>
            </p>
            <p>The module returns download links for all images present in image fills in a document. Image fills are how [!DNL Figma] represents any user-supplied images. When you drag an image into [!DNL Figma], [!DNL Figma] creates a rectangle with a single fill that represents the image, and the user is able to transform the rectangle (and properties on the fill).</p>
            <p>For fields, see <a href="#Get5" class="MCXref xref" >[!UICONTROL Get a file or image: Image fills]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Get a file or image: File]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Select the file that you want to return JSON from.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Enter or map the version of the file you want the module to return. For the current module, leave this field blank.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>To return only a subset of the document, enter the nodes that you want the module to return. The module returns the listed nodes, their children, and anything between the root node and the listed nodes.</p>
        <p>For each node that you want to return, click <b>[!UICONTROL Add]</b> and enter the text of the node.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Enter or map an integer that represents how deep into the document tree you want to return results for. </p>
        <div class="example"><span class="autonumber"><span><b>Example: </b></span></span>
          <ul>
            <li>
              <p>To return pages only, enter <code>1</code>.</p>
            </li>
            <li>
              <p>To return pages and top level objects, enter <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>To return all nodes, leave this field blank.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>To return vector data, enter <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>A comma separated list of plugin IDs and/or the string "[!UICONTROL shared]". Any data present in the document written by those plugins will be included in the result in the <code>pluginData</code> and <code>sharedPluginData</code> properties.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Branch data]</td>
      <td>Enable this option to return branch metadata for the requested file. If the file is a branch, the main file's key is included in the returned response. If the file has branches, their metadata is included in the returned response. Default: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Get a file or image: File nodes]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Select the file that you want to return JSON from.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Enter the nodes that you want the module to return and convert</p>
        <p>For each node that you want to return, click <b>[!UICONTROL Add]</b> and enter the text of the node.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Enter or map the version of the file you want the module to return. For the current module, leave this field blank.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Enter or map an integer that represents how deep into the document tree you want to return results for. </p>
        <div class="example"><span class="autonumber"><span><b>Example: </b></span></span>
          <ul>
            <li>
              <p>To return pages only, enter <code>1</code>.</p>
            </li>
            <li>
              <p>To return pages and top level objects, enter <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>To return all nodes, leave this field blank.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>To return vector data, enter <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>A comma separated list of plugin IDs and/or the string "shared". Any data present in the document written by those plugins will be included in the result in the pluginData and sharedPluginData properties.</td>
    </tr>
  </tbody>
</table>


##### Get a file or image: Image

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Select the file that you want to return JSON from.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Enter the nodes that you want the module to render.</p>
        <p>For each node that you want to render, click <b>[!UICONTROL Add]</b> and enter the text of the node.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Scale]</td>
      <td>To scale the image, enter or map the scaling factor. This number must be between 0.01 and 4.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Format]</td>
      <td>
        <p>Select the format for the image output.</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Include ID]</td>
      <td>Enable this option to include ID attributes for all SVG elements. Default: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Simplify Stroke]</td>
      <td>Enable this option to simplify inside/outside strokes and use stroke attribute if possible instead of &lt;mask>. Default: [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Use absolute bounds]</td>
      <td>Enable this option to use the full dimensions of the node regardless of whether or not it is cropped or the space around it is empty. Use this to export text nodes without cropping. Default: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Enter or map the version of the file you want the module to return. For the current module, leave this field blank.</td>
    </tr>
  </tbody>
</table>

##### Get a file or image: Image fills

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Select the file that you want to return JSON from.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL List file version history]

This search module returns the version history of a single file in [!UICONTROL Figma].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>For instructions about connecting your [!DNL Figma] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Enter or map the File ID of the file that you want retrieve version history for. </p>
        <ul>
          <li>
            <p>If you do not know the file's ID, click <b>[!UICONTROL Find Files]</b> and enter or map the ID of the project that the file is associated with, then select the file.</p>
          </li>
          <li>
            <p>If you are attempting to find the file's ID and do not know the project's ID, click <b>[!UICONTROL Find Projects]</b> and enter or map the ID of the team that owns the project the file is associated with. Select the project, then select the file.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List project files]

This search module returns a list of all files in the specified project.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>For instructions about connecting your [!DNL Figma] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Enter or map the Project ID the project that you want retrieve files for. </p>
        <ul>
          <li>
            <p>If you do not know the projects's ID, click <b>[!UICONTROL Find Projects]</b> and enter or map the ID of the team that the project is are associated with, then select the project.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List projects]

This search module returns a list of all projects within the specified team.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>For instructions about connecting your [!DNL Figma] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Enter or map the Project ID of the project that you want to retrieve files for. The team ID can be found in the URL of the team's page in Figma</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td>
    </tr>
  </tbody>
</table>


### Components and styles

#### [!UICONTROL Get a style or component]

This action module retrieves a single style or component, or a set of styles or components.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>For instructions about connecting your [!DNL Figma] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions.</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Object> key]</td>
      <td>Enter the key (unique identifier) of the object you want to retrieve.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Enter or map the ID of the team that the record or records are associated with.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Page Size]</td>
      <td>Enter or map the number or results to return per page. Default: 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL After]</td>
      <td>
        <p>Enter or map the number of the result after which to start retrieving results. This can be combined with the [!UICONTROL Page Size] field to paginate results.</p>
        <p>This value does not correspond to object IDs.</p>
        <p>This field cannot be used in combination with the [!UICONTROL Before] field.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Before]</td>
      <td>
        <p>Enter or map the number of the result before which to start retrieving results. This can be combined with the [!UICONTROL Page Size] field to paginate results.</p>
        <p>This value does not correspond to object IDs.</p>
        <p>This field cannot be used in combination with the [!UICONTROL After] field.</p>
      </td>
    </tr>
  </tbody>
</table>


### Other

* [Make an API call](#make-an-api-call)

* [Watch events](#watch-events)


#### [!UICONTROL Make an API call]

This action module lets you make a custom authenticated call to the Figma API without having to think through authentication. This way, you can create a data flow automation that can't be accomplished by the other Figma modules.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>For instructions about connecting your [!DNL Figma] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Enter a path relative to <code>https://api.figma.com/v1/</code>.</p>
        <p>For example: <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Method]</td>
      <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adds the authorization headers for you.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Add the query for the API call in the form of a standard JSON object.</p>
        <p>For example: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Watch events]

This trigger module starts a scenario when one of the following events occur for a specific team in your [!DNL Figma] team space

* File update

* File version update

* File delete

* Library publish

* File comment

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>Select the webhook that the module watches.</p>
        <p>To add a new webhook:</p>
        <ol>
          <li value="1">
            <p>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL Webhook] field.</p>
          </li>
          <li value="2">
            <p>Select the connection you want to use for this webhook. For instructions about connecting your [!DNL Figma] account to [!UICONTROL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!UICONTROL Adobe Workfront Fusion] - Basic instructions.</a></p>
          </li>
          <li value="3">
            <p>Select the event type that you want the module to watch.</p>
          </li>
          <li value="4">
            <p>Enter the ID of the team whose events you want the webhook to watch.</p>
          </li>
          <li value="5">
            <p>Enter the [!UICONTROL Status] or [!UICONTROL Description] of events that you want the webhook to watch.</p>
          </li>
          <li value="6">
            <p>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
