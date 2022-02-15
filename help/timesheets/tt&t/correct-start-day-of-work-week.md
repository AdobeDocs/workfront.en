---
filename: correct-start-day-of-work-week
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
---




# Correct the start day of the work week for Timesheets {#correct-the-start-day-of-the-work-week-for-timesheets}



## Problem {#problem}

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in the section [Create or Edit a Timesheet Profile](create-timesheet-profiles.md#creating-a-timesheet-profile) in [Create Timesheet Profiles](create-timesheet-profiles.md).).


## Solution {#solution}

The start day of the week of a timesheet in `Workfront` uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser.&nbsp;


For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.


This setting also affects the start day of the week in the pop-up calendars across the system.


The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always&nbsp;starts on&nbsp;Sunday.


Following are the directions for changing language and locale settings for various browsers that are supported with `Workfront`.



* **Chrome:**&nbsp;Copy and paste the following link into your Chrome browser: [chrome://settings/languages](chrome://settings/languages) then go to Languages.

* **Firefox:**Copy and paste the following link into your Firefox browser: [about:preferences#content](about:preferences#content) then go to Languages.

* **IE 11:** &nbsp;Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.


&nbsp;
