---
filename: resource-scope
content-type: overview
product-area: projects
navigation-topic: task-information
---




# Overview of Resource Scope {#overview-of-resource-scope}



## Overview of the Resource Scope field {#overview-of-the-resource-scope-field}

Resource Scope is a task-level field that indicates whether you can assign other tasks to the user during the timeframe of a certain task. The default value of the Resource Scope field is None and in most cases you cannot edit it. 


When the **Task Constraint** of a task is **Fixed Dates**, you can edit the Resource Scope value and you can set it to Global. When you indicate that the Resource Scope of a task is Global, other tasks cannot be assigned to the same user during the same timeframe of the task. 


For information about the Fixed Dates Task Constraint, see [Task Constraint overview: Fixed Dates](fixed-dates.md).


## Edit the Resource Scope field on a task {#edit-the-resource-scope-field-on-a-task}




1.  Go to a task for which you want to edit the Resource Scope. 
1.  Click the **More** icon ![](assets/qs-more-icon-on-an-object.png)next to the task name, then **Edit**. 
1.  In the **Overview** section, in the **Task Constraint** field, select **Fixed Dates**. 

1.  Specify the **Planned Start Date** and the **Planned Completion Date** of the task. 

1.   In the **Settings** section, locate the **Resource Scope** field.


   Select from the following options: 



   >[!IMPORTANT] {type="important"}
   >
   >When the Task Constraint is not **Fixed Dates**, you cannot edit the Resource Scope. In that case, the Resource Scope always defaults to **None**, and the user assigned to the task can be assigned to other tasks during the same time frame.


   `<li value="6">Click <b>Save Changes</b>. </li>` 





## Tasks with a Global Resource Scope {#tasks-with-a-global-resource-scope}

When trying to assign a user to a task with a Fixed Dates constraint and a Resource Scope of Global, and that user is already assigned to another task with a Fixed Dates constraint and a Resource Scope of Global, you receive a scheduling conflict warning.  
![resource_scope_global_warning_for_tasks.png](assets/resource-scope-global-warning-for-tasks-600x93.png)




You cannot perform the following actions:



* Assign a user to a task that has a Global Resource Scope if the user is already assigned to another task that has a Global Resource Scope for the same time frame. 
* Reassign the task to a user who is already assigned to another task that has a Global Resource Scope for the same time frame.
* Change the dates on the task with Global Resource Scope to dates that belong to another task with a Global Resource Scope.




>[!IMPORTANT] {type="important"}
>
>All tasks to which the user is assigned must have the Resource Scope set to Global in order to receive this warning. The warning does not display for a user with scheduled tasks using any other task constraints or tasks with a Fixed Date constraint and a Resource Scope of None.


