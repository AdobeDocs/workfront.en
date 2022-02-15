---
filename: view-project-all-project-team-users-roles
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
---




# View: project with all project team users and roles {#view-project-with-all-project-team-users-and-roles}

This project view shows a list of users and job roles assigned to the project team.


>[!NOTE]
>
>&nbsp;If the job role is listed on the same row as a user, this does not imply that the user is filling that role on the project, nor that the user is assigned that role in their profile.


![project_custom_view_with_all_users_and_roles_on_the_project_.png](assets/project-custom-view-600x89.png)




To apply this view:



1. Go to a list of projects.
1. From the **View** drop-down menu, select **New View**.

1. In the** Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, then click** Switch to Text Mode**.
1. Mouse over the text mode area, and click **Click to edit text**.
1.  Remove the text you find in the **Text Mode** box, and replace it with the following code:
   `<pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=60<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Team Users<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=userID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.page=/userView.cmd<br>column.1.listdelimiter=<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.namekey=user.plural<br>column.1.stretch=30<br>column.1.type=iterate<br>column.1.valuefield=user:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Team Roles<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.page=/roleView.cmd<br>column.2.listdelimiter=<br>column.2.listmethod=nested(roles).lists<br>column.2.namekey=jobrole.plural<br>column.2.stretch=10<br>column.2.type=iterate<br>column.2.valuefield=name<br>column.2.valueformat=HTML<br>column.2.width=150.stretch=0</pre>` 

1. Click **Save View**.


