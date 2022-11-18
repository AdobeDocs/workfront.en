---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Power BI Modules
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
author: Becky
hidefromtoc: true
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
---
# Power BI Modules

Power BI is an application that allows you to visualize and present data to your stakeholders. It can take data from a variety of sources.

>[!NOTE]
>
>Workfront Fusion is not a data source. While Workfront Fusion can create and use data sources, it does not store your data.


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
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## PowerBI modules and their fields

When you configure PowerBI, Workfront Fusion displays the fields listed below. Along with these, additional fields might display, depending on factors such as your access level in the app or service. A bold title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Dashboards

#### List Dashboards

This search module retrieves a list of dashboards.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>
        <p>Select or map the ID of the Group that owns the dashboards you want to list.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Limit  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### List Dashboard Tiles

This search module retrieves a list of dashboard tiles.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">Connection</td>
    <td>&#160;</td>
  </tr>
  <tr>
    <td role="rowheader">Enter a Dashboard ID</td>
    <td>
      <p>Select or map the option to choose the dashboard whose tiles you want to list.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">Dashboard ID</td>
    <td>
      <p>Enter or map the ID of the dashboard that contains the tiles you want to list.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">Group ID  </td>
    <td>Select or map the ID of the Group that owns the dashboards that contains the tiles you want to list.</td>
  </tr>
  <tr>
    <td role="rowheader">Limit  </td>
    <td>
      <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
    </td>
  </tr>
</tbody>
</table>

#### Get a Dashboard

This action module retrieves metadata of a specified dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Enter a Dashboard ID</td>
      <td>
        <p>Select or map the option to choose the dashboard that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Dashboard ID</td>
      <td>
        <p>Enter or map the ID of the dashboard that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that owns the dashboardsthat you want to retrieve metadata for.</td>
    </tr>
  </tbody>
</table>

#### Get a Dashboard Tile

This action module retrieves metadata of a specified dashboard tile.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Enter a Dashboard ID</td>
      <td>
        <p>Select or map the option to choose the dashboard details you want to retrieve.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Dashboard ID</td>
      <td>
        <p>Enter or map the ID of the dashboard that you want to retrieve details for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Tile ID</td>
      <td>Enter or map the ID of the Power BI tile you want to retrieve details for.</td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that owns the tile you want to retrieve.</td>
    </tr>
  </tbody>
</table>

#### Create a Dashboard

This action module creates a new dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Name</td>
      <td>Enter or map a name for the Dashboard.</td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that will own the new Dashboard.</td>
    </tr>
  </tbody>
</table>

### Reports

#### List Reports

This search module retrieves a list of reports.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>
        <p>Select or map the ID of the Group that owns the reports you want to list.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Limit  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Get a Report

This action module retrieves metadata of a specified report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Enter a Report ID</td>
      <td>
        <p>Select or map the option to choose the report that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Report ID</td>
      <td>
        <p>Enter or map the ID of the report that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that owns the report that you want to retrieve metadata for.</td>
    </tr>
  </tbody>
</table>

#### Copy a Report

This action module copies an existing report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Enter a Report ID</td>
      <td>
        <p>Select or map the option to choose the report that you want to copy.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Report ID</td>
      <td>
        <p>Enter or map the ID of the report that you want to copy.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that owns the report that you want to copy.</td>
    </tr>
    <tr>
      <td role="rowheader">New Copied Report Name</td>
      <td>Enter or map a name for the new report.</td>
    </tr>
  </tbody>
</table>

#### Delete a Report

This action module deletes a report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Enter a Report ID</td>
      <td>
        <p>Select or map the option to choose the report that you want to delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Report ID</td>
      <td>
        <p>Enter or map the ID of the report that you want to delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that owns the report that you want to delete.</td>
    </tr>
  </tbody>
</table>

### Dataset

#### List Datasets

This search module retrieves a list of datasets.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that owns the report that you want to retrieve metadata for.</td>
    </tr>
    <tr>
      <td role="rowheader">Limit</td>
      <td>
        <p>Enter or map the maximum number of records you want the module to [action] during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Get a Dataset

This action module retrieves metadata of a specified dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Enter a Report ID</td>
      <td>
        <p>Select or map the option to choose the report that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Report ID</td>
      <td>
        <p>Enter or map the ID of the dataset that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that owns the dataset that you want to retrieve metadata for.</td>
    </tr>
  </tbody>
</table>

#### Create a Dataset

This action module creates a new dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Name</td>
      <td>Enter or map a name for the dataset.</td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that will own the new dataset.</td>
    </tr>
    <tr>
      <td role="rowheader">Default Mode</td>
      <td>
        <p>Select or map the default mode for the dataset:</p>
        <ul>
          <li>
            <p><b>As Azure</b>: A dataset with a live connection to Azure Analysis Service</p>
          </li>
          <li>
            <p><b>As on Prem</b>: A dataset with a live connection to On-premise Analysis Service</p>
          </li>
          <li>
            <p><b>Push</b>:  A dataset that allows programmatic access for pushing data into PowerBI</p>
          </li>
          <li>
            <p><b>Push Streaming</b>: A dataset that supports data streaming and allows programmatic access for pushing data into Power BI</p>
          </li>
          <li>
            <p><b>Streaming</b>: A dataset that supports data streaming</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Tables</td>
      <td>Add tables to the dataset. For fields, see <a href="#Table" class="MCXref_0">Table fields</a></td>
    </tr>
    <tr>
      <td role="rowheader">Data sources</td>
      <td>Add the data sources. For fields, see <a href="#Data" class="MCXref_0">Data sources fields</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">Default Retention Policy  </td>
      <td>
        <p>Select or map the intentional policy for the dataset:</p>
        <ul>
          <li>
            <p>None</p>
          </li>
          <li>
            <p>Basic FIFO</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Table fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Name</td>
      <td>
        <p>  Enter or map a name for the table.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Columns</td>
      <td>
        <p>Add the columns:</p>
        <ul>
          <li>
            <p><b>Name</b>
            </p>
            <p>Enter (map) a column name.</p>
          </li>
          <li>
            <p><b>Data Type</b>
            </p>
            <p>Select or map the data type:</p>
            <ul>
              <li>
                <p>String</p>
              </li>
              <li>
                <p>Integer</p>
              </li>
              <li>
                <p>Boolean</p>
              </li>
              <li>
                <p>Date Time</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>Format String</b>
            </p>
            <p>Enter (map) the format string.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Rows</td>
      <td>Enter or map row details.</td>
    </tr>
    <tr>
      <td role="rowheader">Measures</td>
      <td>Add the measure for the tables.</td>
    </tr>
  </tbody>
</table>

##### Data sources fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Database  </td>
      <td>
        <p>Enter or map the database that you want to use.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Server  </td>
      <td>
        <p>Enter or map the name of the server you want to use.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">URL  </td>
      <td>
        <p>Enter or map the URL that you want to use.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Data source ID</td>
      <td>
        <p>  Enter or map the ID of the data source.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Data source Type  </td>
      <td>
        <p>Select or map the data source type. Example: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Gateway ID  </td>
      <td>Enter or map the ID of the gateway you want to use.</td>
    </tr>
  </tbody>
</table>

#### Add or Delete Rows in a Dataset Table

This action module adds or deletes rows of a specified push dataset table.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Enter a table</td>
      <td>Select or map the option to select the dataset that contains the table you want to adjust..</td>
    </tr>
    <tr>
      <td role="rowheader">Dataset ID</td>
      <td>Enter or map the ID of the dataset that contains the rows you want to add or delete.</td>
    </tr>
    <tr>
      <td role="rowheader">Table Name  </td>
      <td>
        <p>Enter or map the name of the table that contains the rows you want to add or delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Enter or map the ID of the group that owns the dataset.</td>
    </tr>
    <tr>
      <td role="rowheader">Select the Action</td>
      <td>
        <p>Select or map the action that you want to perform.</p>
        <ul>
          <li>
            <p>Add rows</p>
          </li>
          <li>
            <p>Delete All Rows</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Rows</td>
      <td>
        <p>Add the row fields.</p>
        <ul>
          <li>
            <p><b>Key</b>
            </p>
            <p>Enter or map the key name.</p>
          </li>
          <li>
            <p><b>Field Type</b>
            </p>
            <p>Select or map the field type:</p>
            <ul>
              <li>
                <p>Boolean</p>
              </li>
              <li>
                <p>Date</p>
              </li>
              <li>
                <p>Text</p>
              </li>
              <li>
                <p>Number</p>
              </li>
            </ul>
          </li>
          <li>
            <p>Value</p>
            <p>Enter or map the key value.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### Refresh a Dataset

This action module refreshes a specified dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Enter a dataset</td>
      <td>Select or map the option to select the dataset that you want to refresh.</td>
    </tr>
    <tr>
      <td role="rowheader">Dataset ID</td>
      <td>Enter or map the ID of the dataset that you want to refresh.</td>
    </tr>
    <tr>
      <td role="rowheader">Table Name  </td>
      <td>
        <p>Enter or map the name of the table that contains the rows you want to add or delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Enter or map the ID of the group that owns the dataset.</td>
    </tr>
    <tr>
      <td role="rowheader">Notify Option  </td>
      <td>
        <p>Select or map the option to notify:</p>
        <ul>
          <li>
            <p>Mail on Completion</p>
          </li>
          <li>
            <p>Mail on Failure</p>
          </li>
          <li>
            <p>No Notification</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### Delete a Dataset

This action module deletes a dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Enter a Report ID</td>
      <td>
        <p>Select or map the option to choose the dataset that you want to delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Report ID</td>
      <td>
        <p>Enter or map the ID of the dataset that you want to delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Group ID  </td>
      <td>Select or map the ID of the Group that owns the dataset that you want to delete.</td>
    </tr>
  </tbody>
</table>

### Apps

#### Watch Apps

This trigger module starts a scenario when an app is updated.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Limit  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### List Apps

This search module retrieves a list of all apps installed.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">Limit  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### List App's Reports

This search module retrieves a list of all reports from the specified app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">App ID</td>
      <td>Select or map the ID of the app that you want to list reports from.</td>
    </tr>
    <tr>
      <td role="rowheader">Limit  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### List App's Dashboards

This search module retrieves a list of dashboards from a specified app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">App ID</td>
      <td>Select or map the ID of the app that you want to list dashboards from.</td>
    </tr>
    <tr>
      <td role="rowheader">Limit  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Get an App

This action module retrieves metadata of a specified app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">App ID  </td>
      <td>
        <p>Select or map the ID of the app you want to retrieve.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Get an App's Report

This action module retrieves metadata of a specified app's report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">App ID  </td>
      <td>
        <p>Select or map the ID of the app that contains the report you want to retrieve.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Report ID</td>
      <td>
        <p>  Select or map the ID of the report you want to retreive.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Get an App's Dashboard

This action module retrieves metadata of a specified app's dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>&#160;</td>
    </tr>
    <tr>
      <td role="rowheader">App ID  </td>
      <td>
        <p>Select or map the ID of the app that contains the dashboard you want to retrieve.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Report ID</td>
      <td>
        <p>  Select or map the ID of the dashboard you want to retreive.</p>
      </td>
    </tr>
  </tbody>
</table>

### Other

#### Make an API Call

This action module performs an API call to the Power BI API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td></td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Path</p>
      </td>
      <td>
        <p>Enter a path relative to <code>https://api.powerbi.com</code>. Example: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Method</p>
      </td>
      <td>
        <p>Select the HTTP request method you need to configure the API call. For more information, see HTTP request methods.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Headers</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion adds authorization headers and x-api-key headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Query String  </td>
      <td>
        <p>Enter the request query string.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Body</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
