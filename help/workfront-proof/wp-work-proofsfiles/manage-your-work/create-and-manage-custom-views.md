---
filename: create-and-manage-custom-views
product: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
---



# Create and Manage Custom Views in *`Workfront Proof`* Proof {#create-and-manage-custom-views-in-workfront-proof-proof}



>[!IMPORTANT] {type="important"}
>
>This article refers to functionality in the standalone product *`Workfront Proof`*. For information on proofing inside *`Adobe Workfront`*, see [Proofing](_proofing.md).


You can create custom views of your files and *`proofs`* to list the items you want in the ways you want them displayed. You can also export the information in your Custom view as a report (in CSV, comma separated value, file format). 


>[!NOTE]
>
>Custom views are available only on Select and Premium plans. Please contact our Sales team for a quote.x




## Creating a Custom View {#creating-a-custom-view}

When you create a custom view, you can choose:



* Whether to include *`proofs`*, files, or both
* Which columns are displayed
* Which column&nbsp;to sort by
* The sort order for the&nbsp;column (ascending or descending)
* Which types of filters to use for determining what information is included in the view


After the custom view is&nbsp;created, it is&nbsp;available to use immediately. The name of the new view is&nbsp;also included in the drop-down menu under the heading My custom views (below the Standard views).


To create a custom view:



1. Go to the `Views` page.
1. For more information about views, see [Manage Items on the Views Page in Workfront Proof](manage-items-on-views-page.md).
1. Do either of the following, depending on whether you want to create a new custom view from scratch, or create a new custom view based on an existing standard view:
    
    
    * To create a new custom view based on an existing standard view: From the drop-down menu, select the existing standard view you want to use as the basis for your new custom view. Click the `View Settings` icon, then click `Copy` to new custom view.
    
    * ![](assets/proof-custom-view-icon.png)    
    
    * To create a new custom view from scratch: Click the `New View` icon.
    * ![](assets/proof-newview.png)    
    
    
    
1.  In the `Details` section, specify the following information:

    
    
    * `Name` (required): The name for the new view. Use a unique name so users can easily find the custom view in the drop-down menu on the Views.
    * `Items`: Select whether you want both *`proofs`* and file, *`proofs`* only, or files only included in the view. By default, both *`proofs`* and files are included.
    
    
    

1. In the `Columns` section, determine which columns you want to include in the custom view.
    
    
    1. Click the Right arrow icon. 
    1. ![](assets/proof-view-rightarrow.png)    
    
    
    

    
    
    1. Double-click the name of the selected column.
    1. You must select at least one column, and a column can be added only once.
    1. Select a column from the `Available columns` area that you want to include in the new view.
    1. The columns are moved from the `Available columns` list to the `Selected columns` list.
    
    1. You can select from the standard columns, or you can choose Custom fields and Decision Reasons to be columns in your custom view. (If you have these configured in your account, they appear under the standard list of Available columns area.)
    1. Standard columns you can include
    1. `<col class="TableStyle-TableStyle-HeaderRow-Column-Column1">``<col class="TableStyle-TableStyle-HeaderRow-Column-Column1">``<thead> <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1">  <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Column</span></th>  <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"><span class="bold">Function</span></th> </tr></thead>``<tbody> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Active stage name</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Name of the active stage in the&nbsp;automated workflow.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Comments</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The number of comments received.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Counter</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Shows a number of the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> that has been uploaded on your account (you have to have a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> counter option enabled in Account Settings).</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Created</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The date and time the item was created.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Creator</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The user who created the item.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Date added to <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span></span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The date you were&nbsp;added to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.&nbsp;</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Deadline</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The deadline for the whole <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Decisions</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The number of decisions given out of the expected number (e.g. 0 of 1, 1 of 1, etc.)</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Downloads</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The number of times the original file has been downloaded.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Filename</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The name of the file or <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Folder</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The folder containing the item.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Last activity</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The date and time of the last activity on the item.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Latest decision on</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The date and time of the last decision made.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">My deadline</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Your own deadline on the <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> where you are explicitly added as a Reviewer/Approver (if applied).</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Owner</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The owner of the item.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Owner country</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The country registered in the system for the owner of the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.&nbsp;</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Parent <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span></span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The name of the parent <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Progress</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"><p>Progress bar.&nbsp;Displays <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> that are not yet Started, Opened, Commented on, or Decided on.</p><p>This information is not sorted on.</p></td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Proof name</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The name of the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Proof type</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"><p>The type of <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>: Static file, Static web page, Interactive web (.zip upload), Interactive web page (https), Video, Audio, and Other. </p><p>Combined <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> are identified as "Combined <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> type." File type of the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</p></td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Size on disk</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"><p>File size of the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> as it relates to the disk usage quota.</p><p>This information provided for the current version of the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>. If there is no current version, it is for the most recent version.</p></td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Stage deadlines</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Deadline of stages in&nbsp;the automated workflow.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Stage name</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Name of each&nbsp;stage in the automated workflow. This includes past stages, active stages, and future stages.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">State</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Active, Locked, Draft, or Submitted.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Status</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Pending, Changes required, Approved with changes, Approved, or Not relevant.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Tags</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Any tags attached to the item.</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Upcoming stage names</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> Name of each stage that has not yet started&nbsp;in the automated workflow. </td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Version counter</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> The number of versions of the item.&nbsp;</td> </tr> <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">  <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><span class="bold">Proof version number</span></td>  <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"><font size="2">The version number of the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.</font></td> </tr></tbody>`
    
    1. (Optional) Do either of the following to move the column to the `Selected columns` area so that it is included in the new view:    
        
        
        * Reorder any columns in the `Selected columns` list.
        * The order in which columns are shown in the `Selected columns` list determines the order in which the columns are displayed in the custom view.
        * The columns are visible in the `Selected columns` list in the order that you added them from the `Available columns` list.
        
        * To reorder a column in the `Selected columns` list, select the name of the column and drag it either up or down in the list.
        
        
    
        
        
        * Remove a column from the `Selected columns` list, by clicking the name of the selected column, then clicking the `Left` arrow. Alternatively, you can double-click the name of the selected column (the column is moved back to the `Available columns` list).
        
        * A&nbsp;column can be added only once. For example, if you move Comments column from Available to Selected columns list, the name of this column will disappear from Available columns list.
        
        
    
    
    

1. In the `Sorting` section, specify the following information:
    
    
    * `Sort by:`&nbsp;Use the Sorting tab if you want to set a particular order in which items are listed in your custom view. If you do not select a column for sorting, the default is No column - that is, no special sort column or order.
    * Only the columns you selected on the Columns tab are included in the Sort by column drop down list.
    * `Ascending or Descending:` Select whether you want to sort the column either ascending or descending by default.
    
    

1. Use the `Filters` section to define one or more criteria for selecting items to include in your Custom view. Filters are especially helpful if you want to use your custom view as a report.
1. To include all items in your custom view, skip the `Filters` section.
1. Available filters
1.  
    
    
    * `Field:`&nbsp;Select the Field for this filter (Comments is the default field.) The Field list contains all the Standard fields (as in the Columns tab). The list is not limited to the columns you selected for display.
    * `Operator:`&nbsp;The Operators available for the filter depend on the type of Field you selected. Select an Operator that shows the relationship between the Field and the value field. You will fill in this information later.
    * `Value:`&nbsp;Select or enter your chosen value in this Field, according to the field and the Operator you selected. Depending on the Operator you chose, there might be one Value field or two or none. &nbsp;See the examples below.
    *  `Filters are applied using the following logic:`&nbsp;Filter criteria between different fields will use the AND operator. Multiple filter criteria using the same field will use the OR operator for the same field.
    
    
      If you want to see only *`proofs`* with zero comments,select the following values:
    
        
        
        * Field: Comments
        * Operator: Equals
        * Value field: 0
        
        
      If you want to see only *`proofs`* with two or more comments, select the following values:
    
        
        
        * Field: Comments
        * &nbsp;Operator: Greater or equal to
        * Value field: 2
        
        
      If you want to see only *`proofs`* with between 1 and 4 comments, select the following values: 
    
        
        
        * Field: Comments
        * Operator: Between
        * Value field (first field): 1
        *  Value field (second field): 4
        
        
          You can change a filter that you have added to your Custom view without any problems or remove it by clicking the cross icon next to the setup filter if needed.
        
        
          Because the Field list is not limited to the columns you selected on the Columns tab, take care when you create a filter that includes a column you did not select for display in your custom view. For example, the following filter for the view will select all *`proofs`* with a Version counter value of 2 or more:        
            
            
            * Field = Version counter
            * Operator = Greater or equal to
            * Value field = 2
            
            
              >[!NOTE]
              >
              >You can change a filter that you have added to your Custom view without any problems or remove it by clicking the cross icon next to the setup filter if needed.
            
            
            
            
            

        
        
        
    
    
    
1. In the `Sharing` section, select which users in your account will be able to see your Custom view.
1. Custom views are specific to the user who creates them. By default the new Custom view is visible only for its creator; however, you can choose to share your custom view by choosing one of the following options:
1.  `<li><span class="bold">Only you can see this custom view</span> (default): Select this option if you want the custom view to be available only to you.</li>` `<li><span class="bold">All users can see this custom view</span>: Select this option to make the custom view available to all users on your account.</li>` `<li><span class="bold">Select users that can see this custom view</span>: Select this option to make the custom view available only to specific users.</li>` Begin typing the name or the email address of the user who you want to have access to the custom view, then click the name when it appears in the drop-down list.


   If you choose to not share your view with other users at this point, you can do so later by editing the custom view.

1.  Click `Create`.
1. The&nbsp;Custom view is displayed&nbsp;and is&nbsp;available on the Views page. For more information about views, see [Manage Items on the Views Page in Workfront Proof](manage-items-on-views-page.md).




## Editing Custom Views {#editing-custom-views}

You can edit a custom view easily. To edit a custom view:



1. Go to the `Views` page.  
   For more information about views, see [Manage Items on the Views Page in Workfront Proof](manage-items-on-views-page.md).

1. Click on the Views button (1)
1. Select the view you want to edit from the drop-down menu.  
   ![](assets/proof-view-edit.png)


1. Click the  `View Options` button, then click `Edit view`.  
   ![](assets/proof-view-options.png)  
   The Edit Custom View page is displayed.

1. Click on the Actions menu. (3)  
   This button is available only if you include the Proof name column in your view.
1. Select Edit view from the menu.&nbsp;(4)&nbsp;  
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)


1. The Edit custom view page&nbsp;is displayed.


![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)




`NOTE`If you edit your Custom view, the&nbsp;columns in Selected columns list will arrange in an alphabetical order automatically. You will need to rearrange them if needed before updating the view. 


## Copying Custom Views {#copying-custom-views}

The Copy view function lets you easily make a copy of an existing custom view. This is really useful, for example, if you want to set up separate views for all your designers, with each view being the same except for the *`proof`* owner (designer).


To copy a custom view:



1. Go to the `Views` page.  
   For more information about views, see [Manage Items on the Views Page in Workfront Proof](manage-items-on-views-page.md).

1. Click on the `Views` button. (1)
1. Select your Custom view from the list. (2)
1. Click the `Actions` menu. (3)  
   This button is available only if you include the Proof name column in your view.

1. Select Copy from the menu. (4)  
   ![copying_custom_view.png](assets/copying-custom-view-350x258.png)


1. In the Copy custom view page, all the original settings are populated. Modify the Custom view as per your choice and click the `Copy view` button. You will be taken to your new view immediately.  
   ![](assets/copy-custom-view-page-350x542.png)






## Sharing Custom Views {#sharing-custom-views}

The Share view function lets you share a view with other users in your account if you did not already select them on the Sharing section&nbsp;for the view. When you share a custom view with other users, the view appears in their My custom views section of the Views drop down menu.


To share a custom view with other users:



1. Go to the `Views` page.  
   For more information about views, see [Manage Items on the Views Page in Workfront Proof](manage-items-on-views-page.md).

1. Click on the `Views` button (1)
1. Select your Custom View from the list (2)
1. Click the `Actions` menu. (3)  
   This button is available only if you include the Proof name column in your view.

1. Select Share view from the menu (4)
1. The Edit custom view page will come up.
1. In the Sharing section elect the users you want to share the view with and click  `Update view`.


&nbsp; ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)




## Exporting Custom Views to CSV Files {#exporting-custom-views-to-csv-files}

To export the data from a custom view to a CSV file:



1. Go to the `Views` page.  
   For more information about views, see [Manage Items on the Views Page in Workfront Proof](manage-items-on-views-page.md).

1. Click on the `Views` button. (1)
1. Select your Custom View from the list. (2)
1. Click the `Actions` menu. (3)  
   This button is available only if you include the Proof name column in your view.

1. Select Export to CSV from the menu. (4)  
   ![exporting_custom_view.png](assets/exporting-custom-view-350x258.png)  
   In a separate browser window, 'Generating report: 100%' appears plus the number of records (the number of items included in the report from your custom view)

1. (Conditional) If a security message appears indicating that the report download is currently blocked, click&nbsp;to allow the download to proceed.
1. Click `Save` when the File Download window appears asking if you want to open or save the file.
1. Select a location on your computer and save the file.




## Deleting Custom Views {#deleting-custom-views}

You can delete a Custom view easily. To do this:



1. Go to the `Views` page.  
   For more information about views, see [Manage Items on the Views Page in Workfront Proof](manage-items-on-views-page.md).

1. Click on the `Views` button.
1. Select your Custom view from the list
1. Click the `Actions` menu. (3)  
   This button is available only if you include the Proof name column in your view.

1. Select Delete from the menu. (4)  
   ![deleting_custom_view.png](assets/deleting-custom-view-350x258.png)


1. Click `Delete`&nbsp;(5) to confirm that you want to delete the current Custom view  
   ![delete__1_.png](assets/delete--1--350x187.png)


1. The default All items view is displayed and your deleted custom view no longer appears in the `Views` drop-down menu.


