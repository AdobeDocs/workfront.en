---
filename: filter-cross-project-successors
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
---




# Filter: cross-project successors {#filter-cross-project-successors}

This task filter returns incomplete cross-project successors.


To apply this filter:



1. Go to a list of tasks.
1. From the **Filter**&nbsp;drop-down menu, select **New Filter**.

1. Click** Switch to Text Mode**.
1. In the **Set Filter Rules for your Report** area, paste the following code:  
   `<pre>percentComplete=100<br>percentComplete_Mod=ne<br>successorsMM:projectID=FIELD:projectID<br>successorsMM:projectID_Mod=ne</pre>`

1. Click **Save Filter**.


