---
title: Third Quarter 2025 Reporting enhancements
description: Third Quarter 2025 Project enhancements
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Third Quarter 2025 Reporting enhancements

This page describes all reporting enhancements made with the Third Quarter 2025 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Third Quarter 2025 release cycle, see [Third Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

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

