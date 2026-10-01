---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Register a private listing for Workfront Data Connect
description: Register a Snowflake private listing to share your Workfront Data Connect data directly with your organization's Snowflake account.
author: Courtney
feature: Reports and Dashboards
exl-id: 
last-update: 2026-09-15T00:00:00.000Z
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Register a private listing for Workfront Data Connect

You can share your Workfront Data Connect data directly with your organization's Snowflake account by registering a private listing. This connection method uses Snowflake's private listing capability to securely share data between organizations without exposing it publicly, and it works across regions and hosting platforms.

A private listing is useful when you want to join your Workfront data with other data in your enterprise data warehouse. Because the data lands in your own Snowflake account, you can query it alongside the rest of your data.

## Access requirements

+++ Expand to view access requirements.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

You also need a Snowflake account with permissions to accept listings and create databases, and a Workfront Data Connect entitlement.

## What a private listing shares

A private listing gives you access to the following:

* Over 100 data views for Workfront objects. For descriptions of each view, see [Workfront Data Connect data dictionary](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md).
* The `*_event` data views, which contain each change transaction delivered to the Data Connect data pipelines.
* Custom data values for data-extendible objects. For an example, see the custom data query example in [Workfront Data Connect query examples](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md).

## Differences from a reader account connection

A private listing shares a different set of views than a reader account connection, and the data arrives on a different schedule. Keep the following differences in mind:

* A private listing shares the `*_event` views only. The `*_current` and `*_daily_history` views are available through a reader account, but not through a private listing. You can build them in your own Snowflake account. For more information, see [Set up Current and Daily History views](#set-up-current-and-daily-history-views) in this article.
* A private listing may not include every view available through a reader account. Examples of views that aren't shared include Workfront Planning objects, `MONITORING_DATA_REFRESHES`, `BOOKINGS`, and `CLASSIFIER`. This list isn't exhaustive.
* Data Connect loads change events every 4 hours. Because a private listing requires an additional replication step to surface the data, expect the data to take about 1 hour longer to arrive than it does through a reader account.
* Data replication runs at 01:01, 05:01, 09:01, 13:01, 17:01, and 21:01 UTC. Data is typically available within about 10 minutes after each run.
* The `MONITORING_DATA_REFRESHES` and `JOB_HISTORY` views don't reflect the times that data becomes available through a private listing. Although the `JOB_HISTORY` view is shared through the private listing, we recommend reading it through a reader account to identify failed jobs more quickly.

## Register a private listing

To register a private listing, first gather your Snowflake account details, then add the listing in Workfront.

### Gather your Snowflake account details

Workfront uses your Snowflake account details to target the listing to your account. Gather the following details:

* Account locator
* Account URL
* Account organization
* Account name

Each of these values is available from the Account Details modal in Snowflake.

To find your account details:

1. While logged in to your Snowflake account, click the user menu in the lower-left corner.

1. Select your account in the **Account** section of the menu.

1. Click **View account details** for the account.

1. Record each of the values listed above.

Also decide on the name of the database you want to access your linked Workfront data through. You enter this name when you register the listing.

### Add the private listing in Workfront

You register the private listing through the Adobe Workfront interface.

>[!IMPORTANT]
>
>You can create only one private listing per account locator.

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Setup**.

1. In the left panel, click **System** > **Data Connect**.

1. Click the **Snowflake connections** tab.

1. Click **Add private listing**.

1. Complete the form with the account details you gathered, including your preferred database name.

1. Click **Add private listing**.

### Connect to the listing in Snowflake

In your Snowflake account, establish a connection to the private listing as an external data source. You can then query your Workfront data alongside the rest of your data.

## Set up Current and Daily History views

A reader account connection provides three data views for each object table:

* **Current** — a low-latency representation of the data as it currently exists in the source application.
* **Daily History** — a representation of the data as it was at 11:59 PM UTC for each day.
* **Event** — each change transaction delivered to the Data Connect data pipelines.

A private listing shares the Event view only. This section provides SQL to build the Current, Daily History, and Event views in your own Snowflake account.

All of the event views included in the listing have the fields needed for the view logic below. These examples assume that you have created a new database and schema of your choice in the target Snowflake account, and they use the `projects_event` view. In each example, replace `<listing_db>` and `<listing_schema>` with your own values.

>[!TIP]
>
>We recommend that you replace `select *` with a list of the columns you use for your analytics. If you use `select *` and columns are later added to the listing's event view, you must re-create the view to enable the new columns.

### Current views

The Current view of an object is the last change event record stored in Data Connect. If the last record is in a deleted state, the record is omitted from the Current view. All event views have the same structure.

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

The `deleted` and `end_effective_timestamp` columns aren't necessary in the Current view. The view filters the data to a single value, and it removes the record completely if the record is deleted.

### Daily History views

The Daily History view identifies the change event record that was active at 23:59:59 of a given date, so you can trend the record's state over time. The following example gives the state of a project record at the end of each calendar day.

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### Event views

For consistency, we recommend that you create a copy of the event view from the listing database and place it in the same schema as your Current and Daily History views.

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
