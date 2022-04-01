---
filename: microsoft-365-calendar-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Calendar
description: In order to use Office 365 Calendar with Adobe Workfront Fusion, it is necessary to have an Office 365 Excel account. You can create one at www.office.com.
---

# Microsoft Office 365 Calendar

In order to use Office 365 Calendar with Adobe Workfront Fusion, it is necessary to have an Office 365 Excel account. You can create one at [www.office.com](http://www.office.com/).

For instructions about connecting your Office 365 account to Workfront Fusion, see [Create a connection to Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

After you grant consent, you are redirected back to the Workfront Fusion administration page where you can continue creating your scenario.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
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

To use Microsoft Office 365 Calendar modules, you must have a Microsoft Office 365 Calendar account.

## Microsoft Office 365 Calendar modules and their fields

When you configure Microsoft Office 365 Calendar modules, Workfront Fusion displays the fields listed below. Along with these, additional Microsoft Office 365 Calendar fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Event](#event) 
* [Calendar](#calendar) 
* [Other](#other)

### Event {#event}

* [Watch Events](#watch-events) 
* [Search Events](#search-events) 
* [Get an Event](#get-an-event) 
* [Create an Event](#create-an-event) 
* [Update an Event](#update-an-event) 
* [Delete an Event](#delete-an-event)

#### Watch Events {#watch-events}

This trigger module retrieves details of an event when the event is created, updated, deleted, started, or ended in the selected calendar.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch events</td> 
   <td> <p>Select how you want to watch events.</p> 
    <ul> 
     <li> <p><strong>By Created Time</strong> </p> <p>Watch for new events.</p> </li> 
     <li> <p><strong>By Updated Time</strong> </p> <p>Watch for updated events.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar Group ID</td> 
   <td>Select the calendar group that contains the calendar where you want to watch events.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar</td> 
   <td> <p>Select the specific calendar that you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td>Set the filter conditions to filter results by subject, event ID, or body.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter the maximum number of messages Workfront Fusion should return during one scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Events {#search-events}

This search module retreves details of an event when the event is created, updated, deleted, started, or ended in the selected calendar.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar Group ID</td> 
   <td>Select the calendar group that contains the calendar where you want to watch events.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar</td> 
   <td> <p>Select the specific calendar that you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <p>Set the filter conditions to filter results. You can filter by the following properties:</p> 
    <ul> 
     <li>Subject</li> 
     <li>Event ID</li> 
     <li>Created Date Time</li> 
     <li>Last Modified Date Time</li> 
     <li>Body Preview</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Order by</td> 
   <td> <p>Select how you want to order the results.</p> 
    <ul> 
     <li><strong>Subject</strong>, ascending or descending</li> 
     <li><strong>Created Date Time</strong>, ascending or descending</li> 
     <li><strong>Last Modified Date Time</strong>, ascending or descending</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>Enter the maximum number of events Workfront Fusion should return during one scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Get an Event {#get-an-event}

This action module retrieves details of the specified event.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event ID</td> 
   <td> <p>Enter or map the ID&nbsp;of the event you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create an Event {#create-an-event}

This action module creates a new event.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject</td> 
   <td> <p>Enter or map a title for the created event.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Start date</td> 
   <td> Enter a single point of time when the event starts in a combined date and time representation. Use the format <code>({date}T{time}</code>; for example, <code>2017-08-29T04:00:00.0000000</code>. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">End date</td> 
   <td> Enter a single point of time when the event ends in a combined date and time representation. Use the format <code>({date}T{time}</code>; for example, <code>2017-08-29T04:00:00.0000000</code>. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reminder on</td> 
   <td>Select whether you want to activate a reminder for this event.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reminder</td> 
   <td>Enter or map he number of minutes before the start of the event when the reminder should trigger.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importance</td> 
   <td> <p>Select the importance of this event.</p> 
    <ul> 
     <li>Low</li> 
     <li>Medium</li> 
     <li>High</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sensitivity </td> 
   <td> <p>Select the sensitivity of this event.</p> 
    <ul> 
     <li><strong>Normal</strong> </li> 
     <li> <p><strong>Personal</strong> </p> <p>The recipient sees a "Please treat this as Personal" message.</p> </li> 
     <li> <p><strong>Private</strong> </p> <p>The recipient sees a "Please treat this as Private" message. This event isn't forwarded or redirected by the recipient's inbox rules.</p> </li> 
     <li> <p><strong>Confidential</strong> </p> <p>The recipient sees a "Please treat this as Confidential" message. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body content type</td> 
   <td>Select whether the body content is plain text or HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body content</td> 
   <td>Enter or map the body of the message associated with the event. It can be in HTML or text format (as specified in the Body Content Type field above).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Location</td> 
   <td> <p>Enter the event location details.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Response requested</td> 
   <td>Select <strong>Yes</strong>to request the invitee to send a response to the event invitation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Show as</td> 
   <td> <p>Select how you want the event to appear to people who view your calendar.</p> 
    <ul> 
     <li>Free</li> 
     <li>Tentative</li> 
     <li>Busy</li> 
     <li>Out of office</li> 
     <li>Working elsewhere</li> 
     <li>Unknown</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attendees</p> </td> 
   <td> <p>Add attendees of the event.</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the attendee's name.</p> </li> 
     <li> <p><strong>Email</strong> </p> <p>Enter the attendee's email address.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Category</td> 
   <td>Enter or map the categories that you want the event to display as on the calendar.</td> 
  </tr> 
 </tbody> 
</table>

#### Update an Event {#update-an-event}

Updates an existing event.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event ID</td> 
   <td>Enter, map, or select the ID of the event you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subject</td> 
   <td> <p>Enter or map a title for the created event.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Start date</td> 
   <td> Enter a single point of time when the event starts in a combined date and time representation. Use the format <code>({date}T{time}</code>; for example, <code>2017-08-29T04:00:00.0000000</code>. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">End date</td> 
   <td> Enter a single point of time when the event ends in a combined date and time representation. Use the format <code>({date}T{time}</code>; for example, <code>2017-08-29T04:00:00.0000000</code>. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reminder on</td> 
   <td>Select whether you want to activate a reminder for this event.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reminder</td> 
   <td>Enter or map he number of minutes before the start of the event when the reminder should trigger.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importance</td> 
   <td> <p>Select the importance of this event.</p> 
    <ul> 
     <li>Low</li> 
     <li>Medium</li> 
     <li>High</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sensitivity </td> 
   <td> <p>Select the sensitivity of this event.</p> 
    <ul> 
     <li><strong>Normal</strong> </li> 
     <li> <p><strong>Personal</strong> </p> <p>The recipient sees a "Please treat this as Personal" message.</p> </li> 
     <li> <p><strong>Private</strong> </p> <p>The recipient sees a "Please treat this as Private" message. This event isn't forwarded or redirected by the recipient's inbox rules.</p> </li> 
     <li> <p><strong>Confidential</strong> </p> <p>The recipient sees a "Please treat this as Confidential" message. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body content type</td> 
   <td>Select whether the body content of the message associated with the event is plain text or HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body content</td> 
   <td>Enter or map the body of the message associated with the event. It can be in HTML or text format (as specified in the Body Content Type field above).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Location</td> 
   <td> <p>Enter the event location details.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Response requested</td> 
   <td>Select <strong>Yes</strong>to request the invitee to send a response to the event invitation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Show as</td> 
   <td> <p>Select how you want the event to appear to people who view your calendar.</p> 
    <ul> 
     <li>Free</li> 
     <li>Tentative</li> 
     <li>Busy</li> 
     <li>Out of office</li> 
     <li>Working elsewhere</li> 
     <li>Unknown</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attendees</p> </td> 
   <td> <p>Add attendees of the event.</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Enter the attendee's name.</p> </li> 
     <li> <p><strong>Email</strong> </p> <p>Enter the attendee's email address.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Category</td> 
   <td>Enter or map the categories that you want the event to display as on the calendar.</td> 
  </tr> 
 </tbody> 
</table>

#### Delete an Event {#delete-an-event}

Deletes an existing event.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event ID</td> 
   <td> <p>Enter or map the ID&nbsp;of the event you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calendar {#calendar}

* [List Calendars](#list-calendars) 
* [Get a Calendar](#get-a-calendar) 
* [Create a Calendar](#create-a-calendar) 
* [Update a Calendar](#update-a-calendar) 
* [Delete a Calendar](#delete-a-calendar)

#### List Calendars {#list-calendars}

Retrieves a list of all of the authenticated user's calendars.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar Group ID</td> 
   <td>Select the calendar group that contains the calendars you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>Enter the maximum number of calendars Workfront Fusion should return during one scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Get a Calendar {#get-a-calendar}

Deletes an existing event.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar ID</td> 
   <td> <p>Enter or map the ID&nbsp;of the calendar you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Calendar {#create-a-calendar}

Creates a new calendar in your Google account.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar name</td> 
   <td> <p>Enter a name for the new calendar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a Calendar {#update-a-calendar}

Edits an existing calendar.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar ID</td> 
   <td>Enter the Calendar ID for the calendar you want to update. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">New Calendar name</td> 
   <td> <p>Enter a name for the new calendar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Calendar {#delete-a-calendar}

Deletes an existing calendar.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar ID</td> 
   <td>Enter the Calendar ID for the calendar you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

### Other {#other}

#### Make an API&nbsp;Call

This module allows you to perform a custom API call.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>URL</p> </td> 
   <td> <p>Enter a path relative to <code>https://graph.microsoft.com</code>. Example:<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code>. Workfront Fusion adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p> Add the query for the API call in the form of a standard JSON object.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:   <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

