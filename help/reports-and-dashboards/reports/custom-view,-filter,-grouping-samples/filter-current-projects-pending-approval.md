---
filename: filter-current-projects-pending-approval
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
---




# Filter: current projects pending approval {#filter-current-projects-pending-approval}

The following project filter displays projects in the Current - Pending Approval status,&nbsp;where the logged-in user is either the Project Sponsor or the Portfolio Manager.


To apply this filter:



1. Go to a list of projects.
1. From the **Filter**&nbsp;drop-down menu, select **New Filter**.

1. Click** Switch to Text Mode**.
1. In the **Set Filter Rules for your Report** area, copy and paste the following code:  
   `<pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>`

1. Click **Save Filter**.


