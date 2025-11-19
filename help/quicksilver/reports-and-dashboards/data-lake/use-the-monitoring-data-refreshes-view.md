---
product-area: reports and dashboards
navigation-topic: data-connect
title: Use the Monitoring Data Refreshes view in Data Connect 
description: With Data Connect, Workfront administrators can access detailed records of the recent updates that were made to the data lake date during the most recent refresh.
author: Jenny
feature: Reports and Dashboards
---
# Use the Monitoring Data Refreshes view in Data Connect 

The Monitoring Data Refreshes view displays the recent updates that were made to the data lake date during the most recent refresh. This view's data is updated after each successful completion of a data load. 

Due to the high volume of data and the complexity of the aggregations, the Monitoring Data Refreshes view only displays the object views that have been updated within the last 2 weeks. If a specific record type is absent in this view, it's likely due to a lack of activity within that timeframe.  

>[!NOTE]
>
>This view displays a detailed collection of the data provided by the application and refresh activities as opposed to a daily history or event view that displays refresh activity history. To obtain historical refresh activity details, you can utilize the <code>DL_LOAD_TIMESTAMP</code> date object. 

## Monitoring Data Refreshes view columns 

The Monitoring Data Refreshes view columns contain the following information: 

   <table>
    <tr>
        <td><b>Column Name</b></td>
        <td><b>Type</b></td>
        <td><b>Description</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>Varchar
        </td>
        <td> 
      The object type associated with the Workfront records sent to the data lake. 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>Date</td>
        <td>
   The date of the last successful data refresh for the object type displayed in the OBJ_TYPE column. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 The date and time of the most recent data refresh for the object type displayed in the OBJ_TYPE column.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       The date and time of the second most recent data refresh for the object type displayed in the OBJ_TYPE column. </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>Number</td>
        <td>
     The amount of time in minutes that has elapsed since the last data refresh for the object type. </td>
    </tr>
            <tr>
        <td>CREATED </td>
        <td>Number </td>
        <td>A count of the CREATE record events captured between the previous and latest data refreshes for the object type.  </td>
    </tr>
                <tr>
        <td>UPDATED</td>
        <td>Number </td>
        <td>A count of the UPDATE record events captured between the previous and latest data refreshes for the object type.</td>
    </tr>
                <tr>
        <td>DELETED</td>
        <td>Number </td>
        <td>A count of the DELETE record events captured between the previous and latest data refreshes for the object type. </td>
    </tr>
                <tr>
        <td>TOTAL</td>
        <td>Number </td>
        <td>A count of the total number of events between the previous and latest data refreshes for the object type. 
        <br> 
        <br><b>Note</b>: This is not the same as the total number of records impacted by CREATE, UPDATE, or DELETE events since the same record could be CREATED and UPDATED multiple times within the interval between refreshes.  </td>
    </tr>
   </table>

