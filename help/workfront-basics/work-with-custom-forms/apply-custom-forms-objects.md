



# Apply Custom Forms to objects {#apply-custom-forms-to-objects}

You can attach an existing custom form to an object.&nbsp;Custom forms contain additional custom fields where you can store additional information about the objects. 

Custom forms can be associated with the following objects, and&nbsp;can be applied only to the type of object for which the custom form&nbsp;was created:&nbsp;



* Companies
* Iterations
* Documents
* Expenses
* Issues
* Portfolios
* Programs
* Projects (including Business Cases)
* Tasks
* Users




## Access needed to add custom forms to objects {#access-needed-to-add-custom-forms-to-objects}

The following scenarios must exist before you can attach a custom form to an object:



* A user with administrative rights must create a custom form, as described in [Create a Custom Form](create-a-custom-form.md) before the form is available to be attached to an object. 
* You must have at least Contribute permissions to the object to be able to attach the custom form to the object. For information about permissions in `Workfront`, see [Permissions in the access model](permissions-in-the-access model.md). 

* You must have permissions to see the custom form, as described in [Share a Custom Form](share-a-custom-form.md)




## Apply Custom Forms&nbsp;to&nbsp;an object {#apply-custom-forms-to-an-object}




1. Go to the object where you want to apply the custom form, then do one of the following: 
    
    
    1. To attach the custom form in the Edit object box:     
        
        
        1. `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <b>More</b> menu  <img src="assets/more-icon.png">, then click Edit.  <img src="assets/edit-ojbect-icon.png"></MadCap:conditionalText>`
        1. Click&nbsp;**Custom Forms** > **Add Forms**, then select up to 10 forms from the drop-down menu. 
        
        1. (Optional)&nbsp;Update the information in the editable fields on the custom form. 
        1. Click **Save Changes**. 
        
        
       Or
    
    1. To attach the custom form in the Details area:     
        
        
        1. Click the **<Object type> Details** section in the left panel (for example, **Project&nbsp;Details** or **Issue Details**, depending on the type of object you want to attach the custom form to). 
        1. Click the **Add custom form** field in the upper-right corner, then select up to 10 custom forms from the list.
        1. (Optional) Update the information in the custom fields of the form, then click&nbsp;**Save Changes**.
        
        
    
    




## Multiple Custom Forms on an object {#multiple-custom-forms-on-an-object}

You can apply up to 10 custom forms on a given object, allowing you to make fields available to some users and not to others, or allowing you to better meet&nbsp;the form requirements of multiple projects.


For example, if an existing project has a custom form already, and more custom fields are needed which exist on another custom form, you can add a second form to the project with the additional fields, rather than add the fields to the existing custom form, if those fields are needed just for this one project. 


Adding multiple custom forms is identical to adding one form to an object, as described in the [Apply Custom Forms to an object](#applying-custom-forms-to-an-object) section in this article. 


## Apply Custom Forms to multiple objects in bulk {#apply-custom-forms-to-multiple-objects-in-bulk}

You can add custom forms to multiple objects by selecting them in a list.&nbsp;



1. Navigate to a list of objects.
1.  Select multiple objects in the list.  

1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <b>More</b> menu  <img src="assets/more-icon.png">, then click  <b> </b>the <b> Edit </b>icon  <img src="assets/edit-ojbect-icon.png"></MadCap:conditionalText>` or just click the **Edit** icon ![](assets/edit-ojbect-icon.png).
1. Click **Custom Forms** in the left panel.
1.  In the **Make a selection** drop-down menu, select the form you want to associate with all the selected objects.


   >[!NOTE]
   >
   >If you cannot find the form in the drop-down menu, this means that at least one of the objects has the form already associated with it. Determine which object that is, and eliminate it from your selection, before you can add the form to the remaining objects.&nbsp;



1. Click **Save Changes**.


