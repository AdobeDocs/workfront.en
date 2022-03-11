

# `Data Access` overview

`Data Access` gives you direct access to an analytics-optimized view of your `Adobe Workfront` data through Snowflake. Using the Snowflake connection, you can then put this data into the business intelligence (BI) tool of your choice to perform advanced reporting and visualizations without having to host, maintain, or transform the data.

For information on tools that connect to Snowflake, see Snowflake's [Connecting to Snowflake](https://docs.snowflake.com/en/user-guide-connecting.html) documentation.

With the curated `Data Access` view, you can:

* See time series or historical change data to make predictions into the future and learn from the past through retrospective analysis
* Perform cross-object reporting and view work data in the context of other related objects
* Integrate `Workfront` data with other data sources to connect strategy and execution metrics to performance

Star schemas (facts, dimensions, etc.)

## Types of data

You can currently access the following data types:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span class="bold">Current data</span> </td> 
   <td> <p>Data that represents the view of the data at the time the data warehouse is loaded. Data will change over time to represent the current view. If a record was written to Workfront on Jan 7, 2020, but the values of the related dimension table have changed over time, the facts in the fact table will be for Jan 7, 2020, but the dimension values will be what they are currently. Example: If on Jan 7, 2020 project name = ‘Wonder’, but on July 7, 2020 the name changed to ‘Super’ the current dimension will reflect ‘Super’ as the name for the Jan 7, 2020 fact. Useful for trending dimensions over time. When joining to fact tables, the curr_dim_key will always represent the most current relationship</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">Historical data</span> </td> 
   <td> <p>Represents the value of the data at the time the record was written to Workfront. If a record in the _curr fact was written to Workfront on Jan 7, 2020, the historic dim will give you the dimension values of the data as they were on Jan 7, 2020. Historic data does not change over time.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">Time Travel dimension</span> </td> 
   <td> <p>Dimensions are similar to historic dimensions in that the data is represented at historic data. While a historic dimension represents data at the time the fact record was created, Time Travel dimensions represent what the data looked like on any calendar date. Note that when using time travel ALWAYS use the SLICE_CALENDAR_DATE from either the fact you are joining to or the time travel dimension itself. Currently all dimensions are sliced by calendar date and represent 00:00:00 or midnight of that day.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dimension types

Within the data types, there are 4 different dimensions:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">%_curr&nbsp;dimensions ​</p> <p role="rowheader">​</p> <p role="rowheader"><![CDATA[
 ]]></p> </td> 
   <td> <p>represent the current data as of&nbsp;the&nbsp;last load date. Will change over time to stay current.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">%_hist dimensions</span> </td> 
   <td> <p>represent the actual data at the&nbsp;time&nbsp;the fact record loaded.&nbsp;Does not change over time.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">%_time_travel dimension</span> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">%_date dim</span> </td> 
   <td> <p>can be joined to any dimension key or date&nbsp;with a date data type.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Types of facts

There are 2 types of facts:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader"><span class="bold">%_curr</span>​</p> </td> 
   <td> <p role="rowheader">represent data is it is currently stored in the Workfront application.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">%_time_travel</span> </td> 
   <td> <p role="rowheader">allow you to view the value of the data in the Workfront application from any point in time.</p> <p>Important: Must ALWAYS use calendar_date in your queries.</p> </td> 
  </tr> 
 </tbody> 
</table>

