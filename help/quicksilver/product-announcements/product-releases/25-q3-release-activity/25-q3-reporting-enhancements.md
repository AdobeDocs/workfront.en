---
title: Third Quarter 2025 Reporting enhancements
description: Third Quarter 2025 Project enhancements
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
---
# Third Quarter 2025 Reporting enhancements

This page describes all reporting enhancements made with the Third Quarter 2025 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Third Quarter 2025 release cycle, see [Third Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Enhanced Report Delivery Security

* Preview: June 26, 2025
* Production: Phased rollout from June 26, 2025 to July 9, 2025

We've enhanced scheduled report delivery to ensure Workfront notifications are only sent to email domains approved in the allowlist.

Previously, if your organization had defined a limitation on which email domains Workfront notifications, we would execute a check against the allowlist as emails were being added. 

Now, we also perform a check as the email is being sent to ensure the email address entered complies with the email allowlist. This improved check applies to both email addresses associated with users and ad hoc emails added to the report recipients list.

For more information, see [Schedule an automatic report delivery](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


## User wildcards no longer return results with a null value when filtering 

>[!NOTE]
>
>* Preview: April 30, 2025
>* Production fast release: May 15, 2025 
>* Production for all customers:  July 17, 2025

We have updated the user wildcard behavior to exclude null value when filtering a report. This change helps the filter produce more accurate results, rather than returning results that do not have a user configured correctly (a null result).

Previously, when a user wildcard produced a null value, a report would display all records that also have a null value.

This change applies to the following wildcard filters:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
