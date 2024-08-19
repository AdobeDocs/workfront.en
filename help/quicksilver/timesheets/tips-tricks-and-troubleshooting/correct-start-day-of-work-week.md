---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Correct the start day of the work week for Timesheets
description: The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile. 
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
---
# Correct the start day of the work week for Timesheets

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

 
