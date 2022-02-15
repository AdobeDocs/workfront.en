---
filename: error-message-field-used-in-multi-form-config
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# Error message: The Field Is Used in a Multi-Form Configuration {#error-message-the-field-is-used-in-a-multi-form-configuration}



## Problem {#problem}

You get the following error&nbsp;while editing a calculated Custom Field on a Custom Form:&nbsp;


*"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."* 


## Cause {#cause}

The error occurs because the following setup exists: currently you have at least one object in your system that has multiple Custom Forms attached. The calculated field you are editing exists on multiple forms attached to these objects.


You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.


[ ![](assets/calculated-field-error.png)](../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png) 


For example, you have a task&nbsp;with Custom Forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on Custom Form A.&nbsp;


## Solution {#solution}

Remove the field from the Custom Form and replace it with a new one containing the desired calculation.&nbsp;&nbsp;


To understand what Custom Forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.  
For more information about referencing Custom Forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in [Reference a Custom Form in a report](reference-custom-form-report.md).


To understand what Custom Form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in [Custom Forms overview](custom-forms-overview.md).


For more information about creating a Custom Form and adding or removing fields from it, see [Create a Custom Form](create-a-custom-form.md).
