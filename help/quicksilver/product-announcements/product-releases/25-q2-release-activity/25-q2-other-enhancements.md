---
title: Other enhancements during the Second Quarter 2025 release timeframe
description: Other enhancements during the Second Quarter 2025 release time frame
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
---
# Other enhancements during the Second Quarter 2025 release timeframe

This page describes enhancements made with the Second Quarter 2025 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Second Quarter 2025 release cycle, see [Second Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md).

## Upgrade to the new event subscription version with version upgrade endpoints

>[!NOTE]
>
>Production for all customers: March 6, 2025

Workfront now has versions of event subscriptions. The new version is not a change to the Workfront API, but rather a change to the event subscription functionality. 

The ability to upgrade or downgrade event subscriptions ensures that when changes are made to the structure of events, existing subscriptions do not break, allowing you to test and upgrade to the new version without a gap in your event subscription.

For more information on the differences between the two versions, see the article [Event subscription versioning](/help/quicksilver/wf-api/general/event-subs-versioning.md).

For information on the endpoints used to upgrade or downgrade an event subscription between versions, see the section [Event subscription versioning](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) in the article Event subscription API.

## Represent Adobe Admin Console user changes as "System" in the Workfront update feed

>[!NOTE]
>
>Preview release: January 23, 2025; Production for fast release: With the 25.2 release (February 13, 2025); Production for quarterly release: With the 25.4 release (April 2025)

Now, when the administrator of the Adobe Admin Console makes a change to the user information of a Workfront user, Workfront records this change in the System activity tab of the user's Updates area as belonging to the "System". This refers to the Adobe Admin Console administrator.  

Prior to this update, user changes made by the administrator of the Admin Console were recorded as made by the main Workfront system administrator.   

For information about managing users in the Adobe Admin Console, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
