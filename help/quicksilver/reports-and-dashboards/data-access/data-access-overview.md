---
title: Data Access overview
description: Data Access overview
draft: Probably
---
# Data Access overview

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Work is paused on this product.</p>
<p>Resources: https://docs.google.com/presentation/d/1mbF1SUdfGGT57i-fh3IbtadsO1r2X5dN_2PpSf05_rM/edit#slide=id.p</p>
<p>https://docs.google.com/document/d/1zsvcpuNoYiXmudNoiA0Q1K3nh_REpyjLY9Nzjmjbdw8/edit) </p>
</div>
-->

Data Access gives you direct access to an analytics-optimized view of your Adobe Workfront data through Snowflake. Using the Snowflake connection, you can then put this data into the business intelligence (BI) tool of your choice to perform advanced reporting and visualizations without having to host, maintain, or transform the data.

For information on tools that connect to Snowflake, see Snowflake's [Connecting to Snowflake](https://docs.snowflake.com/en/user-guide-connecting.html) documentation. 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: Synapse)
</MadCap:conditionalText>
-->

With the curated Data Access view, you can:

* See time series or historical change data to make predictions into the future and learn from the past through retrospective analysis
* Perform cross-object reporting and view work data in the context of other related objects
* Integrate Workfront data with other data sources to connect strategy and execution metrics to performance

Star schemas (facts, dimensions, etc.)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: These dimensions are available for the following objects:</p>
<p>Portfolios</p>
<p>Programs</p>
<p>Projects</p>
<p>Tasks</p>
<p>Custom values in tasks</p>
<p>Facts:</p>
<p>Custom_Values_Curr</p>
<p>Custom_Values_Hist</p>
<p>Task Activity Curr</p>
<p>Task Activity Time Travel Daily)</p>
<p>(NOTE: Google this and determine how much detail is needed here.</p>
<p>https://docs.microsoft.com/en-us/power-bi/guidance/star-schema)</p>
</div>
-->

## Types of data

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: File for data catalog article (similar to API documentation with tables): https://adobe-my.sharepoint.com/:x:/p/kurtp/EULMCTvcoUBJtIKTPBUPrikB0TzvtWiXHeEDYmrUGCPHmg?e=4%3A9e2n3O&at=9)</p>
-->

You can currently access the following data types:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Current data</strong> </td> 
   <td> <p>Data that represents the view of the data at the time the data warehouse is loaded. Data will change over time to represent the current view. If a record was written to Workfront on Jan 7, 2020, but the values of the related dimension table have changed over time, the facts in the fact table will be for Jan 7, 2020, but the dimension values will be what they are currently. Example: If on Jan 7, 2020 project name = ‘Wonder’, but on July 7, 2020 the name changed to ‘Super’ the current dimension will reflect ‘Super’ as the name for the Jan 7, 2020 fact. Useful for trending dimensions over time. When joining to fact tables, the curr_dim_key will always represent the most current relationship</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Historical data</strong> </td> 
   <td> <p>Represents the value of the data at the time the record was written to Workfront. If a record in the _curr fact was written to Workfront on Jan 7, 2020, the historic dim will give you the dimension values of the data as they were on Jan 7, 2020. Historic data does not change over time.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Time Travel dimension</strong> </td> 
   <td> <p>Dimensions are similar to historic dimensions in that the data is represented at historic data. While a historic dimension represents data at the time the fact record was created, Time Travel dimensions represent what the data looked like on any calendar date. Note that when using time travel ALWAYS use the SLICE_CALENDAR_DATE from either the fact you are joining to or the time travel dimension itself. Currently all dimensions are sliced by calendar date and represent 00:00:00 or midnight of that day.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dimension types

Within the data types, there are 4 different dimensions:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">%_curr&nbsp;dimensions ​</p> <p role="rowheader">​</p> <p role="rowheader"></p> </td> 
   <td> <p>represent the current data as of&nbsp;the&nbsp;last load date. Will change over time to stay current.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>%_hist dimensions</strong> </td> 
   <td> <p>represent the actual data at the&nbsp;time&nbsp;the fact record loaded.&nbsp;Does not change over time.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>%_time_travel dimension</strong> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>%_date dim</strong> </td> 
   <td> <p>can be joined to any dimension key or date&nbsp;with a date data type.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Types of facts

There are 2 types of facts:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader"><strong>%_curr</strong>​</p> </td> 
   <td> <p role="rowheader">represent data is it is currently stored in the Workfront application.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>%_time_travel</strong> </td> 
   <td> <p role="rowheader">allow you to view the value of the data in the Workfront application from any point in time.</p> <p>Important: Must ALWAYS use calendar_date in your queries.</p> </td> 
  </tr> 
 </tbody> 
</table>

