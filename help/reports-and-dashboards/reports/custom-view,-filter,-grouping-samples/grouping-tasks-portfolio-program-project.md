---
filename: grouping-tasks-portfolio-program-project
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
---




# Grouping: tasks by portfolio, program, and project {#grouping-tasks-by-portfolio-program-and-project}

Use this task grouping to group tasks by the portfolio, by program, and then by the project they are associated with.


![](assets/portfolio-program-project-grouping-for-tasks-600x206.png)




To apply this grouping:



1. Go to a list of tasks.
1. From the **Grouping**&nbsp;drop-down menu, select **New Grouping**.

1. Click** Switch to Text Mode**.
1. Remove the text&nbsp;in the **Group your Report** area.
1. Replace&nbsp;the text with the following code:  
   `<pre>group.0.linkedname=project<br>group.0.namekey=portfolio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.namekey=program<br>group.1.notime=false<br>group.1.valuefield=project:program:name<br>group.1.valueformat=string<br>group.2.name=Project<br>group.2.valuefield=project:name<br>group.2.valueformat=HTML<br>textmode=true<br></pre>`

1. Click **Save Grouping**.


&nbsp;
