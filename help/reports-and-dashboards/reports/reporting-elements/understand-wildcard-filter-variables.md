---
filename: understand-wildcard-filter-variables
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Wildcard filter variables
description: Adobe Workfront supports filter variables or wildcards when building the following elements:
---

# Wildcard filter variables

*Adobe Workfront* supports filter variables or wildcards when building the following elements:

<ul> 
 <li> <p>Filters in lists, reports, and the Resource Planner</p> <p>For information about <em>Workfront</em> filters, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</p> </li> 
 <li> <p>Advanced searches</p> <p>For information about advanced searches, see the section <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search" class="MCXref xref">Use Advanced Search</a> in the article <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md" class="MCXref xref">Search Adobe Workfront</a>.</p> </li> 
 <li> <p>Calculated columns in views</p> </li> 
 <li> <p>Conditional formatting in views</p> <p>For information about conditional formatting, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Use conditional formatting in Views</a>.</p> </li> 
 <li> <p>Calculated custom fields</p> <note type="note">
   Wildcard filter variables are not supported when referencing nested collections in a calculated column.
  </note> <p>For information about calculated custom fields and columns, see the article <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md" class="MCXref xref">Calculated custom fields vs. calculated columns</a>.</p> </li> 
</ul>

By using wildcards, you can reference a generic user or date instead of a specific user or date. In this way, the elements you build are dynamic and the results change depending on the context in which they are used.  
For example, filtering for $$USER.homeGroupID in a project report retrieves only projects associated with the Home Group of the user who is logged in.

You can use date-based or user-based filter variables in *Workfront*.

## Date-based variables

The *Workfront* date-based wildcard options can be used in combination with any date filter attribute.

For information about adding a date-based wildcard to a report, see the article [Use date-based wildcards to generalize reports](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

Choose from the following date-based wildcards:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><span class="bold">$$TODAY</span> </p> </td> 
   <td> <p>We recommend that you build date-sensitive filters using this wildcard so you avoid building the filter again tomorrow, next week, or next month.</p> <p>For example, if you want to display all tasks due before today, you can use the following rule in a task filter: <em>Planned Start Date Less Than $$TODAY</em>.</p> <p>$$TODAY is always equal to midnight for the current day.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><span class="bold">$$NOW</span> </p> </td> 
   <td> <p>This is similar to the $$TODAY wildcard but includes the current date and time. $$NOW is equal to the current date and time.</p> <p>For example, if you want to display all hour entries provided up to the current time, you can do this by using the following rule in an hour filter: <em>Planned Start Date Less Than $$NOW</em>.</p> <p>Note: This wildcard is not supported in the Resource Planner.</p> </td> 
  </tr> 
 </tbody> 
</table>

To indicate various periods of time and various points in time (future or past), you can combine wildcards with the following:

| Attributes |&nbsp; |
|---|---|
| `q`  |calendar quarter |
| `h`  |hour |
| `d`  |day |
| `w`  |week |
| `m`  |month |
| `y`  |year |

| `Qualifiers`  |
|---|
| `b`  |beginning of the week (Sunday) |
| `e`  |ending of the week (Saturday)  |

| `Operators`  |
|---|
| `+`  |add value to wildcard value |
| `-`  |subtract value from wildcard value |

For example, the wildcard 

```
$$TODAYb+2w
```

refers to "2 weeks from the beginning of this week". The wildcard *

```
$$NOW+2h
```

* refers to '2 hours from now'.

## User-based variables

>[!IMPORTANT]
>
>If a filter or report contains a user-based wildcard filter variable the results always show information filtered by the user who is currently logged in. When you share such a filter or report with another user, the wildcard retrieves information for the user looking at the report. The two users see different results.

For information about adding a user-based wildcard to a report, see the article [Use user-based wildcards to generalize reports](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

*Workfront* provides the following user-based variables:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><span class="bold">$$USER.ID</span> </p> </td> 
   <td> <p>The most common user-based variable is $$USER.ID. This always returns the ID of the logged in user. This is the ID used to identify which user created each object and their work assignments.</p> <p>When used in reports, this wildcard decreases the number of reports that you need to create in your system. You can create one report and share it with several users, and the results change based on the user who is logged in and looking at the report.</p> <p>For example, to build a report for all issues assigned to the user who is logged in, you can use the following rule in an issue filter: <em>Assigned To ID Equals $$USER.ID</em>.</p> <p><em>Workfront</em> uses this variable in the following built-in filters:</p> 
    <ul> 
     <li>My Reports</li> 
     <li>My Projects</li> 
     <li>My Tasks</li> 
     <li>My Issues</li> 
     <li>My Hours</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><span class="bold">$$USER.categoryID</span> </p> </td> 
   <td> <p>The $$USER.categoryID variable refers to a specific custom form associated with the logged-in user.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.accessLevelID</span> </p> </td> 
   <td> <p>The $$USER.accessLevelID variable refers to the ID of the access level associated with the logged-in user.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.accessLevelRank</span> </p> </td> 
   <td> <p>The $$USER.accessLevelRank variable refers to the access level rank associated with the logged-in user.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.companyID</span> </p> </td> 
   <td> <p>The $$USER.companyID variable refers to the company associated with the logged-in user.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.customerID</span> </p> </td> 
   <td> <p>The $$USER.customerID variable refers to the ID of the customer account associated with your environment. For your environment, there is only one possible value for this variable and it is typically used only when building integrations through the API.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.firstName</span> </p> </td> 
   <td> <p>The $$USER.firstName variable refers to the first name of the logged-in user.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.lastName</span> </p> </td> 
   <td> <p>The $$USER.lastName variable refers to the last name of the logged-in user.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.name</span> </p> </td> 
   <td> <p>The $$USER.name variable refers to the full name of the logged-in user.</p> <p>Note:  <p>This wildcard variable works only when modifying a filter in text mode. You cannot use this wildcard in filters that do not support text mode.&nbsp;For example, you cannot use this wildcard in the filters in the following areas:</p> 
     <ul> 
      <li> <p>Resource Planner</p> </li> 
      <li> <p>Workload Balancer</p> </li> 
      <li> <p>Analytics</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.homeGroupID</span> </p> </td> 
   <td> <p>The $$USER.homeGroupID variable refers to the ID of the Home Group of the logged-in user. As a Group Administrator, you can use this variable to filter only for items that belong to the users in your Home Group.</p> <p>For example, to see all incomplete tasks on projects in the finance group, use the following filter rules in a task filter:<br><em>Project: Group ID Equals $$USER.homeGroupID </em><br><em>Percent Complete Less Than 100</em></p> <p>To see all incomplete tasks assigned to individuals in a specific group which is the Home Group of the logged-in user, use the following filter rules in a task filter:</p> <p><em>Assigned To: Group ID Equals $$USER.homeGroupID<br>Percent Complete Less Than 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.otherGroupIDs</span> </p> </td> 
   <td> <p>The $$USER.otherGroupIDs variable refers to all groups (including the Home Group) associated with the logged in user's profile.</p> <p>The functionality of this variable is similar to that of the $$USER.homeGroupID variable, except the results display information about the users who belong to any of the groups associated with the logged in user.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.homeTeamID</span> </p> </td> 
   <td> <p>The $$USER.homeTeamID variable refers to the ID of the Home Team of the logged-in user. As a team manager, you can use this variable to filter only for items that belong to the users in your Home Team.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.teamIDs</span> </p> </td> 
   <td> <p>The $$USER.teamIDs variable returns a list of all the teams associated with the logged-in user.</p> <p>The functionality of this variable is similar to that of the $$USER.homeTeamID variable, except the results display information about the user who belongs to any of the teams identified in the filter.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><span class="bold">$$USER.roleID</span> </p> </td> 
   <td> <p>The $$USER.roleID variable refers to Primary Role of the logged-in user. Using this variable, you can report on tasks or issues assigned to a specific job role.</p> <p>For example, to see all tasks assigned to the Primary Role of the logged-in user, you can use the following filter rule in a task filter:</p> <p><em>Task: Role ID Equals $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader">$$USER.roleIDs</td> 
   <td> <p>The $$USER.roleIDs variable refers to all job roles associated with the logged-in user. Using this variable, you can report on tasks or issues assigned to any of the job roles associated with the logged-in user. </p> <p>For example, to see all tasks assigned to any of the roles associated with the logged-in user, you can use the following filter rule in a task filter:</p> <p><i>Task: Role ID Equals $$USERID.roleIDs<br></i> </p> <p>Tip: The <i>Task: Role ID Equals $$USERID.roleIDs</i> filter rule exists in the built-in filters Unassigned Tasks In My&nbsp;Role and Unassigned Issues In My&nbsp;Role. </p> </td> 
  </tr> 
 </tbody> 
</table>

