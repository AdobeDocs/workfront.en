---
filename: grouping-projects-entry-date
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
---




# Grouping: projects by Entry Date {#grouping-projects-by-entry-date}

`In this custom project grouping, you can display projects grouped by their Entry Date values.` 


`Each grouping shows projects with an Entry Date within:` 



* `The last 30 days` 
* `30-60 days` 
* `60 days or older` 


`To apply this grouping:` 



1. `Go to an existing Project report, or create a new Project report.  
   For more information about creating a report, see the article [Create a report](create-report.md)`.
1. `From the`**Grouping** `tab, click`**Add Grouping** `.` 

1. `Click`** Switch to Text Mode** `.` 

1. `Remove the text in the`**Group your Report** `area.` 

1.  `Replace the text with the following code:` 




   ```
   group.0.linkedname=direct<br>
   ```



   ```
   group.0.name=Project Entry<br>
   ```



   ```
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))<br>
   ```



   ```
   group.0.valueformat=atDateAsMonthString<br>
   ```



   ```
   textmode=true
   ```



1. `Click`**Save + Close** `.` 



