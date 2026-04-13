---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 22
description: Adobe Workfront released API version 22 on October 23, 2025. API version 22 features the following changes from version 21.
author: Becky
feature: Workfront API
role: Developer
---
# What's new in API version 22

>[!IMPORTANT]
>
>This API version change features a breaking change that may affect your existing API calls. This is due to the fact that API version 21 uses Event Subscriptions version 2.
>
> For multi-select fields, Event Subscriptions version 2 always sends as an array. Version 1 sent an array if more than one value selected. If only one value was selected, it sent a string.

Adobe Workfront released API version 21 on October 23, 2025. API version 21 features the following changes from version 20.

## Added resources

The following resources were added for API version 22.

### ReportShareableFolder (RPSHFD)

You can use shareable report folders to organize reports and share those folders with other users. This feature is designed for teams that manage large volumes of reports and need scalable, consistent access control.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## Removed resources

The following resources were removed from API version 22.

### UserLocation (USRLOC)

This object has been removed.

## Modified resources

The following resources were modified for API version 22.

