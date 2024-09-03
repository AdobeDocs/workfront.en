---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Power BI modules
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
author: Becky
feature: Workfront Fusion
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
---
# [!DNL Power BI] Modules

[!DNL Power BI] is an application that allows you to visualize and present data to your stakeholders. It can take data from a variety of sources.

>[!NOTE]
>
>[!DNL Workfront Fusion] is not a data source. While [!DNL Workfront Fusion] can create and use data sources, it does not store your data.


## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
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

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

&#42;&#42;For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] modules and their fields

When you configure [!DNL Power BI], [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional fields might display, depending on factors such as your access level in the app or service. A bold title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Dashboards](#dashboards)
* [Reports](#reports)
* [Dataset](#dataset)
* [Apps](#apps)
* [Other](#other)

### Dashboards

* [Create a Dashboard](#create-a-dashboard)
* [Get a Dashboard](#get-a-dashboard)
* [Get a Dashboard Tile](#get-a-dashboard-tile)
* [List Dashboard Tiles](#list-dashboard-tiles)
* [List Dashboards](#list-dashboards)

#### [!UICONTROL Create a Dashboard]

This action module creates a new dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for the Dashboard.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that will own the new Dashboard.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Dashboard]

This action module retrieves metadata of a specified dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>Select or map the option to choose the dashboard that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Enter or map the ID of the dashboard that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that owns the dashboardsthat you want to retrieve metadata for.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Dashboard Tile]

This action module retrieves metadata of a specified dashboard tile.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>Select or map the option to choose the dashboard details you want to retrieve.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Enter or map the ID of the dashboard that you want to retrieve details for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tile ID]</td>
      <td>Enter or map the ID of the [!DNL Power BI] tile you want to retrieve details for.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that owns the tile you want to retrieve.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Dashboard Tiles]

This search module retrieves a list of dashboard tiles.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
    <td>
      <p>Select or map the option to choose the dashboard whose tiles you want to list.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Dashboard ID]</td>
    <td>
      <p>Enter or map the ID of the dashboard that contains the tiles you want to list.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Group ID]  </td>
    <td>Select or map the ID of the Group that owns the dashboards that contains the tiles you want to list.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]  </td>
    <td>
      <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL List Dashboards]

This search module retrieves a list of dashboards.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Select or map the ID of the Group that owns the dashboards you want to list.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

### Reports

* [Copy a Report](#copy-a-report)
* [Delete a Report](#delete-a-report)
* [Get a Report](#get-a-report)
* [List Reports](#list-reports)

#### [!UICONTROL Copy a Report]

This action module copies an existing report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Select or map the option to choose the report that you want to copy.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Enter or map the ID of the report that you want to copy.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that owns the report that you want to copy.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL New Copied Report Name]</td>
      <td>Enter or map a name for the new report.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a Report]

This action module deletes a report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Select or map the option to choose the report that you want to delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Enter or map the ID of the report that you want to delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that owns the report that you want to delete.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Report]

This action module retrieves metadata of a specified report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Select or map the option to choose the report that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Enter or map the ID of the report that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that owns the report that you want to retrieve metadata for.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Reports]

This search module retrieves a list of reports.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Select or map the ID of the Group that owns the reports you want to list.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>


### Dataset

* [Add/Delete Rows in a Dataset Table](#add-or-delete-rows-in-a-dataset-table)
* [Create a Dataset](#create-a-dataset)
* [Delete a Dataset](#delete-a-dataset)
* [Get a Dataset](#get-a-dataset)
* [List Datasets](#list-datasets)
* [Refresh a Dataset](#refresh-a-dataset)

#### [!UICONTROL Add or Delete Rows in a Dataset Table]

This action module adds or deletes rows of a specified push dataset table.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a table]</td>
      <td>Select or map the option to select the dataset that contains the table you want to adjust..</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>Enter or map the ID of the dataset that contains the rows you want to add or delete.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Enter or map the name of the table that contains the rows you want to add or delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Enter or map the ID of the group that owns the dataset.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Select the Action]</td>
      <td>
        <p>Select or map the action that you want to perform.</p>
        <ul>
          <li>
            <p>[!UICONTROL Add rows]</p>
          </li>
          <li>
            <p>[!UICONTROL Delete All Rows]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>
        <p>Add the row fields.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Key]</b>
            </p>
            <p>Enter or map the key name.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Field Type]</b>
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
            <p>[!UICONTROL Value]</p>
            <p>Enter or map the key value.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Create a Dataset]

This action module creates a new dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for the dataset.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that will own the new dataset.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default Mode]</td>
      <td>
        <p>Select or map the default mode for the dataset:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>: A dataset with a live connection to [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b>: A dataset with a live connection to [!DNL On-premise Analysis] Service</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>:  A dataset that allows programmatic access for pushing data into [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: A dataset that supports data streaming and allows programmatic access for pushing data into [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: A dataset that supports data streaming</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tables]</td>
      <td>Add tables to the dataset. For fields, see <a href="#Table" class="MCXref_0">Table fields</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Add the data sources. For fields, see <a href="#Data" class="MCXref_0">Data sources fields</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>Select or map the intentional policy for the dataset:</p>
        <ul>
          <li>
            <p>[!UICONTROL None]</p>
          </li>
          <li>
            <p>[!UICONTROL Basic FIFO]</p>
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
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>  Enter or map a name for the table.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Columns]</td>
      <td>
        <p>Add the columns:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter (map) a column name.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Data Type]</b>
            </p>
            <p>Select or map the data type:</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Format String]</b>
            </p>
            <p>Enter (map) the format string.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>Enter or map row details.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Measures]</td>
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
      <td role="rowheader">[!UICONTROL Database]  </td>
      <td>
        <p>Enter or map the database that you want to use.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>Enter or map the name of the server you want to use.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>Enter or map the URL that you want to use.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source ID]</td>
      <td>
        <p>  Enter or map the ID of the data source.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source Type]  </td>
      <td>
        <p>Select or map the data source type. Example: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gateway ID]  </td>
      <td>Enter or map the ID of the gateway you want to use.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a Dataset]

This action module deletes a dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Select or map the option to choose the dataset that you want to delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Enter or map the ID of the dataset that you want to delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that owns the dataset that you want to delete.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Dataset]

This action module retrieves metadata of a specified dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Select or map the option to choose the report that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Enter or map the ID of the dataset that you want to retrieve metadata for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that owns the dataset that you want to retrieve metadata for.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Datasets]

This search module retrieves a list of datasets.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Select or map the ID of the Group that owns the report that you want to retrieve metadata for.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>
        <p>Enter or map the maximum number of records you want the module to [action] during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Refresh a Dataset]

This action module refreshes a specified dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a dataset]</td>
      <td>Select or map the option to select the dataset that you want to refresh.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>Enter or map the ID of the dataset that you want to refresh.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Enter or map the name of the table that contains the rows you want to add or delete.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Enter or map the ID of the group that owns the dataset.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Notify Option]  </td>
      <td>
        <p>Select or map the option to notify:</p>
        <ul>
          <li>
            <p>[!UICONTROL Mail on Completion]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL No Notification]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

<!-- BECKY START HERE AND CHECK POUND SIGNS-->

### Apps

* [Get an App](#get-an-app)
* [Get an App's Dashboard](#get-an-apps-dashboard)
* [Get an App's Report](#get-an-apps-report)
* [List App's Dashboards](#list-apps-dashboards)
* [List App's Reports](#list-apps-reports)
* [List Apps](#list-apps)
* [Watch Apps](#watch-apps)

#### [!UICONTROL Get an App]

This action module retrieves metadata of a specified app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Select or map the ID of the app you want to retrieve.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get an App's Dashboard]

This action module retrieves metadata of a specified app's dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Select or map the ID of the app that contains the dashboard you want to retrieve.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Select or map the ID of the dashboard you want to retreive.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get an App's Report]

This action module retrieves metadata of a specified app's report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Select or map the ID of the app that contains the report you want to retrieve.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Select or map the ID of the report you want to retreive.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Apps]

This search module retrieves a list of all apps installed.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List App's Dashboards]

This search module retrieves a list of dashboards from a specified app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Select or map the ID of the app that you want to list dashboards from.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List App's Reports]

This search module retrieves a list of all reports from the specified app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Select or map the ID of the app that you want to list reports from.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Watch Apps]

This trigger module starts a scenario when an app is updated.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

### Other

#### [!UICONTROL Make an API Call]

This action module performs an API call to the [!DNL Power BI] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>For instructions about connecting your [!DNL Power BI] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe [!DNL Workfront Fusion] - Basic instructions</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Enter a path relative to <code>https://api.powerbi.com</code>. Example: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
        <p>Select the [!UICONTROL HTTP] request method you need to configure the API call. For more information, see [!UICONTROL HTTP] request methods.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adds authorization headers and x-api-key headers automatically.</p>
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
  </tbody>
</table>
