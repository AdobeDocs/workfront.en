---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Correct the Start Day of the Work Week for Timesheets
description: The start day of the week on my timesheet does not match my expected weekly start day. 
author: Lisa
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
---
# Correct the start day of the work week for Timesheets

<!--Audited: 5/2025-->

## Problem

The start day of the week on my timesheet does not match my expected weekly start day. 

This typically occurs when you are not assigned to a Timesheet Profile and your timesheet was manually created. 


## Solution

Your Workfront administrator should create timesheet profiles and assign everyone to a profile, as described in [Create, edit, and assign timesheet profiles](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Your Workfront administrator might define the start date of a timesheet on a day other than your expected weekly start date. Check with them to find out what the start date of a timesheet profile is for your timesheet. 

If your timesheet was manually created, the start day of the week in the timesheet uses the Email Locale settings in your user's profile, as described in the article [Configure My Settings](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md). 

For example, with the Email Locale set to English (United States), the week in the timesheet starts on Sunday. Alternatively, with the Email Locale set to English (United Kingdom), the week in the timesheet starts on a Monday.


<!--This is the old content for this article but I found this was not working this way at all, so I changed it to what it is today: 

## Problem

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solution

The start day of the week of a timesheet in Adobe Workfront uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser. 

For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.

This setting also affects the start day of the week in the pop-up calendars across the system.

The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always starts on Sunday.

Following are the directions for changing language and locale settings for various browsers that are supported with Workfront.

* **Chrome:** Copy and paste the following link into your Chrome browser: `chrome://settings/languages` then go to Languages.
* **Firefox:**Copy and paste the following link into your Firefox browser: `about:preferences#content` then go to Languages.
* **IE 11:** Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.

-->

 
