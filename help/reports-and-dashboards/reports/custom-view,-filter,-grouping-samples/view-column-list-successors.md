---
filename: view-column-list-successors
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
---




# View (Column): list of successors {#view-column-list-of-successors}

You can add a column to a task view to show a list of the successors of the tasks. The **Task Successors** column includes the number of the successor as well as the name.


![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--600x202.png)




To add this column to a task view:



1. Go to an existing task view.
1. Expand the View drop-down menu, and select **Customize View**.
1. Click **Add Column**.
1. Click **Switch to Text Mode**.
1. Mouse over the **Show in this column** area, and click **Click to edit text**.

1. Remove all text in the Text Mode box, and replace it with the following code:  
   `<pre>displayname=Task Successors<br>listdelimiter=<br><br>listmethod=nested(successors).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})<br>valueformat=HTML</pre>`

1. Click **Save View**.


