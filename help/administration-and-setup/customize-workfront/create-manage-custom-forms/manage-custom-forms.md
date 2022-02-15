



# Manage Custom Forms {#manage-custom-forms}

As a `Workfront administrator`, you can modify and deactivate Custom Forms.


For information about managing Custom Forms applied to objects, see [Manage Custom Forms attached to objects](manage-custom-forms-attached-to-objects.md).


## Modify an existing Custom Form {#modify-an-existing-custom-form}

You can modify a custom form any time after it has been created. There is no notification system to alert other users using the form of the changes you make on it. For this reason, we recommend reducing the number of times when you edit a custom form because it might be used by other users.


If you remove fields from a custom form, the historical data is removed also from the objects associated with the form.  
For more information about removing fields from a custom form without losing historical data, see [Remove fields from a Custom Form without losing data](#removing-fields-from-a-custom-form-without-losing-data).


To modify an existing custom form:



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1.  Click **Custom Forms**.


   Within the custom forms section, you can review all existing custom forms and all custom fields that have been created. In addition to reviewing this information, you can see who created a form and what fields are associated with what forms.  


1.  Click the name of the custom form that you want to modify.  



   For more detailed information about changes you can make, see [Create a Custom Form](create-a-custom-form.md).

1. Make any desired changes, then click **Save+Close**.




## Remove fields from a Custom Form without losing data {#remove-fields-from-a-custom-form-without-losing-data}

To improve system performance and to make forms easier to use for users, you might want to remove fields from a custom form when the fields are no longer being used. Depending on the method that you use to&nbsp;remove fields from a custom form, you might lose historical data associated with the fields that you are removing.


>[!IMPORTANT] {type="important"}
>
>&nbsp;Removing fields from a form that has over 500 fields cannot be undone. Remove fields from&nbsp;a custom form&nbsp;that has&nbsp;over 500 fields only if you are certain that you will not want to re-add fields to the custom form in the future. Each time you remove a field, another field cannot be added to the custom form until the custom form has fewer than 500 fields.&nbsp;


To remove fields from a custom form while maintaining the historical data:



1.  Determine which fields you want to remove from the original custom form. 


   Do not remove any fields from the original custom form at this time.

1. Create a new custom form, as described in [Create a Custom Form](create-a-custom-form.md).  

    
    
    1. Add the fields to the new form that you want to remove from the original custom form.
    1. Save the new custom form that includes all of the fields that you are going to remove from the original custom form.
    
    

1. Limit access to the custom form to only users with&nbsp;administrative access.&nbsp;
1.  Apply the new custom form to the object where the original custom form is already applied, as described in .


   Applying the new custom form to the object ensures that historical reporting data is not affected.

1.  Modify the original custom form and remove any fields. 


   Remove only the fields that you previously&nbsp;added to the new form (in Step 2).


   For information about how to modify a custom form, see [Modify an existing Custom Form](#modify%c2%a0a).  



   The fields that you removed from the original custom form are now available only on the new custom form that you created.&nbsp;Users are able to see the custom form on the object, but users without administrative access are not able to modify the custom form.





## Deactivate a Custom Form {#deactivate-a-custom-form}

You can deactivate Custom Forms you no longer use while retaining all of the associated historical data. If you deactivate a custom form, the form does not display in any drop-down menus on the object. However, the form does still display on any object it is attached to.


Fields on a deactivated custom form are still available to inline edit in a View. If you add a field during an inline edit, the form attaches automatically, even though the custom form is deactivated.



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png)..

1. Click the name of the Custom Form you want to deactivate.
1. Click the **Form Settings** tab.
1. Uncheck the **Is Active** box.
1. Click **Save + Close**.


