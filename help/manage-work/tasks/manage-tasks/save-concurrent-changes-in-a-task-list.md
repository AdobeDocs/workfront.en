---
filename: save-concurrent-changes-in-a-task-list
product-area: projects
navigation-topic: manage-tasks
---



# Overview of saving concurrent changes within a task list {#overview-of-saving-concurrent-changes-within-a-task-list}


When you edit tasks in a list, you can use separate saving settings for indicating whether you want your changes saved automatically on manually when editing tasks in a list. 


For information about editing tasks in a task list, see the article [Edit tasks in a list](edit-tasks-in-a-list.md). 


Sometimes, conflicts may appear if two users are making changes on the same tasks. 


Consider the following when editing tasks in a task list: 



* *`Adobe Workfront`* saves the changes you make to tasks immediately when you select to save your changes automatically if the project Update Type is Automatic or Automatic or On Change. For information about the project Update Type, see [Select the project Update Type](select-project-update-type.md).

* *`Workfront`* updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. 


The following scenarios exist when multiple users are editing the same tasks:



* `One user saves the changes in a task list automatically and another one manually`: If a user (User A) saves changes manually while User B is editing the same tasks but they are saving their changes automatically, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user saving manually (User A) sees a warning message before they can save their changes. The warning message shows the items that have the conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) 




>[!NOTE]
>
>When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.





* `Several users are saving the changes in a task list manually`: If several users that are making changes to tasks in a list are saving manually at the same time, *`Workfront`* saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. *`Workfront`*then compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. 





>[!IMPORTANT] {type="important"}
>
>When you select to keep your changes over all other changes, all your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost. 


