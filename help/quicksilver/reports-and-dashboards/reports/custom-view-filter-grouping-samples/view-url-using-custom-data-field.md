---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: External URL Using Custom Data Field'
description: You can display a link to an internal custom URL by using a Calculated Custom Field named "Custom URL" in a Task View.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
---
# View: external URL using custom data field

<!--Audited: 11/2024-->

You can display a link to an internal custom URL by using a **Calculated Custom Field** named "Custom URL" in a **Task View**.

This helps you quickly link from certain objects in a view to certain areas of the application directly from your reports.

When creating a calculated custom field, you must first create the field, then create the View.

The following sections are an example of a calculated custom field for tasks. The custom field is called Custom URL. The custom view displays the field's value as well as the **URL** field for tasks.

Using the same steps, you can create similar calculated custom fields and custom views for all the objects in the system that have a Custom Form.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a view </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Create the "Custom URL" calculated custom field

For information about creating a calculated custom field, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

If you have access to create a custom form, you can create a calculated custom field for tasks called "Custom URL." This field links directly to the **Overview** subtab within the **Task Details** tab.

1. Create a calculated custom field.
1. In the Calculation field, enter the following code:

   CONCAT(''https://`<domain>`.my.workfront.com","/","task/",ID,"/overview'')

1. Replace "`<domain>`" with your actual domain name, without the brackets. The `/overview` portion of this URL directs the link to the **Overview** section in the left panel of the task.

1. After creating your **Calculated Custom Field**, attach the **Custom Form** with this field to several tasks in Adobe Workfront that you want display in your new view.

## Create the view which displays the "Custom URL" and "URL" fields of the task

The task **View** in the example below displays the **Calculated Custom Field** called "Custom URL" as a direct link to the **Overview** subtab within the task**Details** tab, as well as the **URL** field of the task.

(assets/task-view-with-custom-url-field-quicksilver-350x70.png)

To customize this view:

1. Go to a list of tasks.
1. Expand the **View** drop-down at the top of your task list.
1. Click **Customize View**.
1. Remove all the columns inside the view, except for the first column.
1. Click the header of the first column.
1. Click **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text in the **Edit Text Mode** box and replace it with the following code: 
   

      ```
      column.0.descriptionkey=name
      column.0.link.linkproperty.0.name=ID
      column.0.link.linkproperty.0.valuefield=ID
      column.0.link.linkproperty.0.valueformat= int
      column.0.link.lookup=link.view
      column.0.link.valuefield= objCode
      column.0.link.valueformat= val
      column.0.linkedname=direct
      column.0.listsort=string(name)
      column.0.namekey=name.abbr
      column.0.querysort=name
      column.0.shortview=false
      column.0.stretch=100
      column.0.valuefield=name
      column.0.valueformat=HTML
      column.0.width=150
      column.1.description=Custom URL
      column.1.link.isnewwindow=true
      column.1.link.url=customDataLabelsAsString(Custom URL)
      column.1.linkedname=direct
      column.1.listsort=customDataLabelsAsString(Custom URL)
      column.1.name=Custom URL
      column.1.querysort=URL
      column.1.shortview=false
      column.1.stretch=0
      column.1.valuefield=Custom URL
      column.1.valueformat=customDataLabelsAsString
      column.1.width=150
      column.2.descriptionkey=url
      column.2.linkedname=direct
      column.2.listsort=string(URL)
      column.2.namekey=url.abbr
      column.2.querysort=URL
      column.2.shortview=false
      column.2.stretch=0
      column.2.valuefield=URL
      column.2.valueformat=HTML
      column.2.width=150
      ```

    In this example the 'column.1.' lines display the value in the 'Custom URL' field as a link into the task's **Overview** section; 'column.2.' displays the value stored in the **URL Field** of the task.

1. Click **Done** > **Save View**.
