---
filename: view-user-job-role-percentage-fte-availability
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
---




# View: user Job Role percentage of FTE availability {#view-user-job-role-percentage-of-fte-availability}

You can add a column to the view of a user list to display a list of the Job Roles the user is associated with as well as the percentage of FTE availability for each job role, as defined in the user profile.


For information about defining the percentage of FTE availability for users, see [Edit a user's profile](edit-a-users-profile.md).


![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-600x237.png)




To add this column to a user view:



1. Go to a list of users.
1. From the&nbsp;**View**&nbsp;drop-down menu, select&nbsp;**New View**.

1. In the**&nbsp;Column Preview**&nbsp;area, click **Add Column**.

1. Click the header of the new column, then click**&nbsp;Switch to Text Mode**.
1. Mouse over the text mode area, and click&nbsp;**Click to edit text**.
1. Remove the text you find in the&nbsp;**Text Mode**&nbsp;box, and replace it with the following code:  
   `<pre>displayname=Roles Time Percentage<br>listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>`

1. Click **Save**.
1. Click **Save View**.
1. (Optional) Specify a name for your view, then click **Save View**.


