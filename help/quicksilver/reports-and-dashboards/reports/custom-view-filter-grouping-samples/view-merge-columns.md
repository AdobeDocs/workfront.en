---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Merge Information from Multiple Columns in One Shared Column'
description: You can merge the information that displays in multiple separate columns and display it in one shared column.
author: Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
---
# View: merge information from multiple columns in one shared column

<!-- Audited: 11/2024 -->

You can merge the information that displays in multiple separate columns and display it in one shared column.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p> Current: 
   <ul>
   <li>Request to modify a view</li> 
   <li>Plan to modify a report</li>
   </ul>
     </p>
     <p> New: 
   <ul>
   <li>Contributor to modify a view</li> 
   <li>Standard to modify a report</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations when sharing or merging columns

* You can merge two adjacent columns and display the information from each column separated by a line break, or you can merge the information in two adjacent columns with no separator between the information from each column.
* You can merge the information from more than two columns by applying the same syntax described in this article to an already shared column and an adjacent one. 
* The `valueformat=HTML` line is mandatory in a shared column. Otherwise, the columns contain no information (they will be blank) when the report is exported from Adobe Workfront.
* Conditional formatting may not be supported in merged columns.

  The following exceptions exist:

   * When viewing information in Workfront, the formatting of the first column is kept and the formatting for all other columns is ignored if the columns that make up a merged column have different formatting from one another,. 
   * When exporting the view to a PDF file, conditional formatting applies to the first column in a merged column. 
   * When exporting the view to an Excel file, merged columns display as separate columns. The individual columns also display their respective conditional formatting rules.

* Columns with the **viewalias** attribute can limit the amount of columns that you can merge. To avoid these limits, avoid using the **viewalias** attribute. If you must include the **viewalias** attribute in a column, make sure that it is the last item listed in the column.

* If you export a list with shared columns to an Excel or Tab Delimited format, these columns are separated out in the exported file.

* When one or both of the columns display a `tile` type field, a forced line-break is automatically introduced in the merged column. For example, Text Fields with Formatting are `tile` type fields. In this case, there is a line code of `type=tile` when viewing the columns in Text Mode. 

## Merge data from two columns without a line break

You can merge the data from multiple separate columns to display it in one column with no breaks or spaces between the values from each column.

>[!TIP]
>
>This approach is recommended when you merge two columns that can never show a value for the same record at the same time. For example, in a Work Item report, the Issue Name and Task Name columns can be merged without a line break between them because a Work Item can never have an Issue Name and a Task name at the same time. A Work Item can be either an Issue or a Task in Workfront.

To merge data from two columns without a line break:

1. Go to a list of objects. 
1. From the **View** drop-down, select a view, then click the **Edit** icon ![Edit icon](assets/edit-icon.png) to edit the view. 
1. Go to the first colum you want to merge, then click **Switch to Text Mode** > **Edit Text Mode**.
1. Add the following text to the first column you want to merge:

   `sharecol=true`
   
   When you merge the first two columns of a list or report, Workfront precedes each line of text that contains information about the object in the first column with `column.0.` and the lines of text that contain information about the second column with `column.1.` .

   You must precede the column number of the first column with the number of that column. Column counting always starts with the leftmost column of the list or report labeled as `column.0.`.

   If you share more than one column, ensure you add the column number in the lines of code that contain the sharing information for each column. 


   **EXAMPLE:** The following is the text mode code for a merged column that contains three separate columns, starting with the second column of the list. The merged values are Project Name, Planned Start Date, and Project Owner's name and there is no break between the three values:
    
     ```
     column.1.valuefield=name
     column.1.valueformat=HTML
     column.1.sharecol=true
     column.2.valuefield=plannedStartDate
     column.2.valueformat=atDate
     column.2.sharecol=true
     column.3.valuefield=owner:name
     column.3.valueformat=HTML
     ```
   
   ![Shared column with no line breaks](assets/shared-column-no-line-breaks-350x142.png)


1. Click **Done**, then **Save View**.

## Merge data from two columns with a line break

Do the following to merge the data from multiple columns to display it in one common column with a line break between the values from each column:

1. Go to a list of objects. 
1. From the **View** drop-down, select a view, then click the **Edit** icon ![Edit icon](assets/edit-icon.png) to edit the view. 
1. Add a third column between the two columns you want to merge.

   >[!TIP]
   >
   >* The columns you want to merge must be adjacent to each other.
   >* You must click the first column that you want to merge.

1. Click **Switch to Text Mode** > **Edit Text Mode**, and add the following code in the middle column that you added in step 1:

   ```
   value=<br>
   valueformat=HTML
   width=1
   sharecol=true
   ```

1. Click the first column and click **Switch to Text Mode** > **Edit Text Mode**, then add the following text to the column:

   `sharecol=true`
   
   When you merge the first two columns of a list or report, Workfront precedes each line of text that contains information about the object in the first column with `column.0.`, the column with the sharing information with `column.1.`,  and the lines of text that contain information about the second column with `column.2.`.
   
   If the combined column is in the middle of the view, the columns are numbered according to their place in the view. Column counting always starts with the leftmost column of the list or report labeled as `column.0.`.

   If you share more than one column, ensure you add the column number in the lines of code that contain the sharing information. 

      **EXAMPLE:** The following is the text mode code for a shared column that contains Project Name, Planned Start Date, and Project Owner's name with a line break. The shared column is the second column of a project view.

      ```
      column.1.displayname=Project_StartDate_Owner
      column.1.sharecol=true
      column.1.textmode=true
      column.1.valuefield=name
      column.1.valueformat=HTML
      column.2.value=<br>
      column.2.width=1
      column.2.valueformat=HTML
      column.2.sharecol=true
      column.3.valuefield=plannedStartDate
      column.3.valueformat=atDate
      column.3.sharecol=true
      column.4.value=<br>
      column.4.width=1
      column.4.valueformat=HTML
      column.4.sharecol=true
      column.5.textmode=true
      column.5.valuefield=owner:name
      column.5.valueformat=HTML 
      ```

      ![Shared column with line breaks](assets/shared-column-with-line-breaks-350x199.png)

1. Click **Done**, then **Save View**.
