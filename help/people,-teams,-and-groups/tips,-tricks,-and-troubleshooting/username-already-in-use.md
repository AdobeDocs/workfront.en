---
filename: username-already-in-use
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
---




# Username Already in Use {#username-already-in-use}



## Question {#question}

When creating a new user a Whoops error is displayed stating that the username is already taken. There are no other occurrences of this email in the system. Why is this being displayed?


## Solution {#solution}

This can occur either because the username or email address is not unique in the current `Workfront` instance or in another `Workfront` instance.


### In a Single `Workfront` Instance {#in-a-single-workfront-instance}

Ensure that the username and email address is unique in the current `Workfront` instance:



1. As the `Workfront administrator`, go to the **People** tab, then click the **People** subtab.

1. In the list of people, look in the **Email** column to ensure there are no duplicate emails.
1. Add a column for username to the view. 
    
    
    1. In the **View** drop-down menu, click&nbsp;**Customize View**.
    
    1. Click&nbsp;**Add Column**.
    1. In the search field, type *username*.
    1. Select **User** > **Username**.
    
    1. Save the view.  
       This results&nbsp;in a view to display the usernames where you can look for the duplicate.
    
    
1. In the list of people, look in the **Username** column to ensure there are no duplicate usernames.




### In Another `Workfront` Instance {#in-another-workfront-instance}

Ensure that the username and email address is unique across all instance of `Workfront` in your organization. This is commonly the case for consultants that work with other companies who use `Workfront`. The solution for this issue is to use a different case for the new username.


For example, if johndoe@domain.com is the duplicate, you could use JohnDoe@domain.com for the new user.
