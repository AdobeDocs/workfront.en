---
filename: filter-cross-project-predecessors
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
---




# Filter: cross-project predecessors {#filter-cross-project-predecessors}

This task filter returns incomplete cross-project predecessors.


To apply this filter:



1. Go to a list of tasks.
1. From the **Filter**&nbsp;drop-down menu, select **New Filter**.

1. Click** Switch to Text Mode**.
1. In the Set Filter Rules for your Report area, paste the following code:  
   `<pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>`

1. Click **Save Filter**.


