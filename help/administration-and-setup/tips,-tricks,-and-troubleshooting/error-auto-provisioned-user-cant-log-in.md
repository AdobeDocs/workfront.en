---
filename: error-auto-provisioned-user-cant-log-in
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# Error: Auto-Provisioned User Cannot Log In {#error-auto-provisioned-user-cannot-log-in}

When an auto-provisioned user tries to log in for the first time, the receive the following error: 


## Problem {#problem}

The system is not assigning&nbsp;the new user an access level. 


By default,&nbsp;auto-provisioning uses the Request license type. When no access levels with a Request license&nbsp;exists, the system cannot assign the user an access level.&nbsp;


## Solution {#solution}

Create a basic access level with a Request license:



1. Go to Setup > Access Levels.
1. Click **New Access Level**.
1. Enter a **Name**.
1. In the **License Type** drop-down menu, select Request.
1. Click **Save Changes**.


After you create an access level with a Request license, have the user log in with their SSO credentials.
