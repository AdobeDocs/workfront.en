---
filename: view-project-user-list
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
---




# View: project user list {#view-project-user-list}

You can apply this view in a project list or report to display a list of users that are associated with the project, as well as a list of the job roles they are performing on each project.&nbsp;


The information in this report can also be found in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> People area</MadCap:conditionalText>` of the project.  
![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-600x171.png)




To apply this view to a project list:



1. Go to a list of projects.
1. From the&nbsp;**View**&nbsp;drop-down menu, select&nbsp;**New View**.

1. In the**&nbsp;Column Preview**&nbsp;area, eliminate all columns except for one.
1. Click the header of the remaining column, then click**&nbsp;Switch to Text Mode**.
1. Mouse over the text mode area, and click&nbsp;**Click to edit text**.
1. Remove the text you find in the&nbsp;**Text Mode**&nbsp;box, and replace it with the following code:  
   `<pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.displayname=Project Users<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={user}.{name}<br>column.1.valueformat=HTML<br>column.2.displayname=Project Roles<br>column.2.listdelimiter=&lt;br&gt;<br>column.2.listmethod=nested(projectUserRoles).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={role}.{name}<br>column.2.valueformat=HTML</pre>`

1.  Click **Save View**. 


