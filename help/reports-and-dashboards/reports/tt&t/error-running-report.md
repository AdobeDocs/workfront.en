---
filename: error-running-report
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
---




# Error message when running a report: "You are not currently logged in." {#error-message-when-running-a-report-you-are-not-currently-logged-in}



## Problem {#problem}

When running a report, or displaying it in a dashboard, the following error returns:  
*Let's try that again. You are not currently logged in.*  



No results are displayed in the report. 


## Cause {#cause}

The report is currently set to run as a deactivated user. 


## Solution {#solution}

You must have Manage permissions to the report to be able to change the report settings.  
To adjust the report and see the results: 



1. Go to the report.
1. Click **Report Actions > ****Edit > ****Report Settings.**

1. Specify the name of an active user in the **Run this report with the Access Rights of:** field.  
   Or  
   Leave the **Run this report with the Access Rights of:** field blank. 

1. Click **Done**.
1. **Save + Close.  
   **The error should not appear again when running this report. 


