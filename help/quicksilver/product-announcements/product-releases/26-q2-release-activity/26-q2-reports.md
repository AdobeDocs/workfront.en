---
title: Second Quarter 2026 Reporting enhancements
description: Second Quarter 2026 Reporting enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
---
# Second Quarter 2026 Reporting enhancements

This page describes Reporting enhancements made with the Second Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Second Quarter 2026 release cycle, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Run reports as a specific user in Canvas dashboards

>[!NOTE]
>
>Preview: April 2, 2026
>Production fast release: April 15, 2026
>Production for everyone: April 16, 2026
>
>Canvas Dashboards is currently in beta.

You can now configure reports on Canvas dashboards to run as a specific user. When enabled, the report displays data based on the selected user's access instead of the viewer's permissions.

This ensures more consistent and reliable data across dashboard viewers, even when access to Planning workspaces, record types, or authorization settings differs.

For more information, see [Build a KPI report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [Build a chart report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md), or [Build a table report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

## Scheduled Report Delivery Now Supports Link-Based Emails

>[!NOTE]
>
>Preview: April 2, 2026
>Production fast release: April 15, 2026
>Production for everyone: April 16, 2026

Workfront now includes a new Link delivery type for scheduled reports. Instead of generating and attaching a file, this option sends an email containing a direct link to the report in Workfront, allowing recipients to view the most current data in the application. 

The Link option is now the default delivery type for newly created scheduled report delivery rules, while existing file-based formats (HTML, PDF, Excel, and TSV) remain available.

With this change, we've also updated the look-and-feel of the report delivery email.

For more information, see [Schedule an automatic report delivery](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## New Authentication Options for Data Connect Connection

>[!NOTE]
>
>Preview: March 12, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now authenticate to Data Connect using RSA keys or Programmatic Access Tokens (PAT) connections, adding more secure and flexible alternatives to traditional username/password credentials. 

These new options allow organizations to maintain stable connections from Power BI, Tableau, and other third‑party BI tools without relying on user-based login methods.

>[!IMPORTANT]
>
>In June 2026, username/password credentials will be required to use multi-factor authentication (MFA). We recommend transitioning to either RSA or PAT-based authentication for service user accounts used to load data from Data Connect into third-party visualization tools, data processors, and scripts that will not work with MFA in the authentication process.

## Custom field labels shown when building reports

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

The custom field label is now displayed before the field name and object in the report building tools, helping you locate fields more easily. Field labels are also shown when defining filters, views, and groupings in lists.

The custom field label is intended for the system interface, while the field name is frequently used for the API and back-end storage purposes, and may not be as helpful when locating a field.

For more information, see [Create a custom report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Shareable Report Folders

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now organize and share reports using shareable report folders. This new feature helps teams that manage large volumes of reports maintain scalable and consistent access control:

* **Create organized folder structures**: System administrators can create top-level folders, and users with manage access can create subfolders up to 4 levels deep.
* **Granular permission controls**: Share folders with two permission levels:
   * View: Users can open reports and share folders
   * Manage: Users can edit folder details, add/remove items, and automatically receive manage access to all reports within the folder
* **Inherited permissions**: Permissions cascade from parent folders to all subfolders and reports within the folder tree
* **Enhanced list experience**: When you enable sharable folders, you will have access to the enhanced list experience. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


For more information, see [Use shareable report folders](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

## Improved Date Labels for Chart Groupings in Canvas Dashboards

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

>[!NOTE]
>
>Canvas Dashboards is currently in beta.

Charts that group data by date now display clearer, more readable date labels. With this update, date labels dynamically adjust based on the selected Group by option—such as day, week, month, or year—making charts easier to read and interpret at a glance:

<table> <tbody> <tr> <td>Day</td> <td>Displays the full date. Example: 3/12/2026</td> </tr> <tr> <td>Week</td> <td>Displays a formatted week start date. Example, Mar 8, 2026</td> </tr> <tr> <td>Month</td> <td>Displays the month and year. Example Mar 2026</td> </tr> <tr> <td>Year</td> <td>Displays the year only. Example: 2026</td> </tr> </tbody> </table>

Previously, chart groupings always showed the start date of the selected period in a numeric format.
