---
product-area: reporting
navigation-topic: text-mode-reporting
title: Text mode syntax overview
description: You can use the text mode interface to create more complex views, filters, groupings, and customized prompts in lists and reports. By using text mode, you can access fields and their attributes that are not available in the standard mode interface.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
---
# Text mode syntax overview

<!--Audited: 1/2025-->

You can use the text mode interface to create more complex views, filters, groupings, and customized prompts in lists and reports. By using text mode, you can access fields and their attributes that are not available in the standard mode interface.

For information and considerations about text mode before you begin, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

For a complete list of all our reportable fields and their attributes, see the [API Explorer](../../../wf-api/general/api-explorer.md).

For more information about creating reports using text mode, including classes, videos, and tutorials, visit the Learn section on the Adobe Experience League site. 

## Considerations about text mode syntax

* You must understand the Adobe Workfront syntax before you can start building reporting elements in text mode. The Workfront syntax for text mode is unique to this application and it has unique characteristics that you must be familiar with.
* Before you start using text mode in your reports, we strongly recommend that you take our classes on advanced reporting, to gain a deeper understanding of our text mode language.
* You can customize views, filters, and groupings using the standard mode interface. However, you can build Custom Prompts only using text mode.

## Common guidelines for building reporting elements in text mode

The following are common guidelines when building any reporting or list element in text mode:

* Always use camel case when referencing objects or attributes in the Workfront database.
* Keep in mind the hierarchy of objects in Workfront. The following differences exist between views, filters and groupings:

   * You can display an object that is three objects away from the report or list object in a view.
   * You cannot reference objects that are more than 2 objects away from the main object in a grouping, filter, or custom prompt.

  **Example:** You can display the name or GUID of the Portfolio Owner in a task view:

  `valuefield=project:portfolio:ownerID`
  
  You cannot group, filter, or prompt for the Portfolio Owner in a task view:

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`

  In these examples, Portfolio Owner ID is three objects away from the object of the list.

  For information about the hierarchy of objects in Workfront, see:

   * [Understand objects in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 
   * [API Explorer](../../../wf-api/general/api-explorer.md)

* Use wildcards whenever possible to make your reports and lists more dynamic and avoid duplicating them for different users and similar timelines.

## Camel case overview

When referencing Workfront fields or their attributes in text mode, Workfront requires you to type their names in camel case. In this case, the single-name fields are spelled in lowercase. Compound fields are spelled according to the following pattern:

`camelCaseSyntax`

>[!IMPORTANT]
>
>All reporting elements follow this casing pattern.

The characteristics of camel case are:

* The first word always starts with a lowercase letter.
* The following words always start with an uppercase letter.
* There are no spaces between the words.

**Example:** To reference the Actual Completion Date of a project, the name of the field that you would use when building text mode reporting elements is 

`actualCompletionDate`

## Text mode syntax for various reporting elements

The following similarities exist between the syntax of the sets of reporting elements below, when creating them using text mode:

* The lines of code and syntax are similar for views and groupings.

  For information about the key lines of codes for views and groupings when building them in text mode, see:

   * [Edit a view using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md) 
   * [Edit a grouping using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* The lines of code and syntax are similar for filters and custom prompts.

  For more information, see:

   * [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md) 
   * [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Syntax for views and groupings 

The lines of code when building views and groupings are similar.

For information about creating views and groupings, see the following articles:

* [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) 
* [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

The most important line of code for a view or a grouping is the line that identifies the object referenced in the view's column or in the grouping. This line of code may start with `valuefield` or `valueexpression` based on whether this field is a direct reference to a Workfront database field or a calculation between several fields.

The following table lists the most common lines of codes in a view or grouping: 

| Code line       | Description                                                                                                                  |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield`      | Identifies the object referenced in the view's column or the grouping. This is a direct reference to the object referenced.  |
| `valueexpression` | Identifies the object referenced in the view's column or the grouping. This is a calculation between several fields.         |
| `valueformat`     | Identifies the format in which Workfront returns the value specified in the valuefield or valueexpression lines.             |
| `width`           | Identifies the width of a column in pixels.                                                                                  |
| `stretch`         | Identifies which columns occupy extra space not needed by the view.                                                          |

>[!TIP]
>
>* Although the lines of code in the examples below are similar between views and groupings, always remember that every line of code for a grouping starts with the grouping number.
>
>  To group by Project Name in a project list or report, use the following line for the first-tier grouping:
>
>  `group.0.valuefield=name`
>  
>* If you edit multiple columns in a view in the same column (as it is the case of shared columns), remember that every line of code for each column starts with the column number. 
>
>  Use the following format to identify the first column of a view: 
>
>  `column.0.valuefield=name`
>  
>  For information about sharing columns, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 
>

#### `Valuefield` syntax overview for views and groupings

`Valuefield=` is a key line of code in views and groupings that identifies the object you are referencing directly.

The syntax for directly referencing fields is identical for groupings and views.

The following rules apply when referencing Workfront objects using a `valuefield` line:

* Use camel case to reference fields directly.

  **Example:** To reference the Task Actual Completion Date in a task view, use the following line:

  `valuefield=actualCompletionDate`

* Use camel case and colons to separate fields related to one another for the same object.

  **Example:** To reference the Project Planned Completion Date in a task view, use the following line:

  `valuefield=project:plannedCompletionDate`
  
  For information about how objects are referencing one another in the Workfront database, see the [API Explorer](../../../wf-api/general/api-explorer.md).

* When referencing a custom field, use the name of the field exactly as it appears in the interface.

  **Example:** To reference a project custom field labeled Additional Details in a task view, use the following line:

  `valuefield=project:Additional Details`
  
#### `Valueexpression` syntax overview for views and groupings  

You can replace the `valuefield=` line of code with `valueexpression=` when building views and groupings in text mode when you want to reference a calculation between 2 or more fields.

>[!TIP]
>
>Although you can build calculated fields which you can display in reports, calculated views and groupings are more dynamic. Calculated views and groupings refresh with new information every time you run the report or display a list.
>
>For information about creating calculated columns in a view, see [Calculated custom fields vs. calculated columns](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Building a calculated grouping is similar to building a calculated column in a view.

The following rules apply when referencing Workfront objects using a `valueexpression` line:

* Use camel case to reference fields directly and enclose each field in curly brackets.

  **Example:** To display the Task Name field in a task column using `valueexpression`, use the following line:

  `valueexpression={name}`
  

* Use camel case and periods to separate fields related to one another.

  **Example:** To display the name of a project concatenated with the name of the task in a task report, use the following lines:

   * In a view:    
   
     `valueexpression=CONCAT({project}.{name},' - ',{name})`
     
   * In a grouping:    
   
     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`
     
  For information about how objects are referencing one another in the Workfront database, see the [API Explorer](../../../wf-api/general/api-explorer.md).

* When referencing a custom field, use following rules:

   * Use the name of the field exactly as it appears in the interface.
   * Precede the name of the field with "DE:".
   * Enclose the field in curly brackets.
   * Separate the fields related to the object by periods.

  **Example:** To display the Additional Details project custom field in a task view in a valueexpression line, use the following line:

  `valueexpression={project}.{DE:Additional Details}`

* You can use a wildcard in a `valueexpression` but not in a `valuefield` line.

  For information about wildcards, see [Wildcard filter variables overview](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` overview for views and groupings

The second most important line of code in a view or grouping is the `valueformat=` line. This tells Workfront in what format to return the value you specify in the `valuefield` or `valueexpression` lines. Although you can use various formats for the `valueformat` lines, we recommend that you always use the following value when using `valueexpression`: 

`valueformat=HTML`

For additional `valueformat` values, also see the following articles:

* [Format dates in text mode reports](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Format numbers, currency and percentage values in text mode reports](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` overview for views

`width=` is the line of code where you can specify the width of each column in pixels. Workfront provides a suggested width for each field, though depending on the type of field and format, you may want to make adjustments. 

You must use the additional `usewidths=true` line of code to enforce the width specified for the column.

**Example:** To display a column with a width of 80 pixels, use the following lines:

`width=80`

`usewidths=true`

#### `stretch` overview for views

The `stretch` is used to identify which columns occupy extra space not needed by the view. The user interface width of the workspace for a typical user is about 850 pixels. This means that if you have a view with four columns (150 pixels each) that your view occupies 600 of 850 pixels. There are 250 extra pixels in the UI that will be added to the columns that have a stretch percentage provided.

The stretch of a column is enforced when you use the additional line of code: `usewidths=true` for at least one of the columns in the view.

**Example:** To indicate that a column could use a 70% of the empty space in a view, use the following lines:

`stretch=70`

`usewidths=true`

### Syntax for filters and custom prompts

The syntax for creating filters is similar to that for creating custom prompts.

>[!TIP]
>
>You can create a custom prompt by first building a filter for the statement you want to include in the prompt. Connect all the lines of code in a filter by "&" without any spaces between the lines and that becomes your custom prompt.

For information about building filters and custom prompts, see:

* [Filters overview](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
* [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

For information about creating filters in text mode, see [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

You can use the following elements to build filters and custom prompts in text mode:

* A line of code referencing the object of the filter statement. Use camel case for the filter object.
* A line of code referencing the filter object and the modifier for the value of the filter object. Use camel case for the filter object in this line.

  >[!TIP]
  >
  >When referencing ranges, this requires 2 modifier lines.

* A statement connector that connects multiple filter statements:

   * AND

     This is the default connector between filter statements.
   
   * OR

     >[!TIP]
     >
     >Statement connectors are case sensitive and always uppercase. "AND" can be omitted in text mode.

* Wildcards to make filters more dynamic and customize them for the current time or the user who is logged in. For information about wildcards, see [Wildcard filter variables overview](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
