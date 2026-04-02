---
title: Manage the List View in Adobe Workfront Planning
description: You can display objects and their fields in a list view, when accessing them in the Connected records page of a record, in Adobe Workfront Planning. This article describes how you can create or edit a list view in the Connected records page of a record.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
last-update: 2026-04-01T11:23:03-07:00
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
---

# Manage the list view in Adobe Workfront Planning

<!--
although list views in Planning are very similar to Workfront enhanced lists, keep this one separate with all the information, because of Planning standalone; some information here is also duplicated in this main Glist article: help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md
-->

<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can view objects in the list view in the following areas of Workfront Planning:

* A connected records page for projects in a record's details area

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

* A list of request forms at the record type level

    ![Request forms in list view](assets/request-forms-in-list-view.png)

This article describes how you can navigate, create, or edit a list view in Workfront Planning. 

## Access requirements

+++ Expand to view the access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront and any Planning package</p>
<p>Any Workflow and any Planning package</p>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Considerations about list views

* Consider the following for connected records page list view: 

    * You can only view projects in the list view in the connected records page of a record. The list view is not available for any other object or record type in a connected records page. 
    
    For information about creating a connected records page, see [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
    * Before you can view a list view in a connected records page of a record you must connect Workfront projects with Planning record types. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).  
    * You can create multiple list views for projects in a record's connected records page.

* Consider the following for the request forms list view: 

    * You cannot create or edit additional list views for Planning request forms. Workfront creates one list view for request forms. <!--this will change-->

        For information about request forms, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* Depending on where it displays, not every list view has all the elements described in this article.

## Manage a list view {#manage-a-list-view}

Workfront Planning list views are similar to Workfront's enhanced lists. Most elements from enhanced views also exist on list views in Workfront Planning. 

For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!--
Removed - more direct steps below: 
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. Go to a list view in one of the following areas:

    * A connected records page for projects in a record's details area
    * The Request forms page of a record type

1. (Conditional) When available, do one of the following to modify the list view: 

    1. Expand the dropdown views menu in the upper-left corner of the list to select another view, or click **New view** and create another one.

        >[!TIP]
        >
        >Views are shared throughout the system. If you create a Projects view for one record type, you can view it on other record types that display connected projects. 

    1. Hover over the name of an existing view and click the **More** menu ![More menu](assets/more-menu.png), then click one of the following:
        * **Rename**, to give the view a new name
        * **Share**, to share the view with others
        * **Delete**, to delete the view. 
            
        >[!NOTE]
        >
        >* You must have Manage permissions to a view to be able to edit, share, or delete it.
        >
        >* You cannot modify System Views. 
        >
        >* <span class="preview">You can reset a view that was shared with you to which you have only permissions to View, after you modified it to restore its original preferences, or you can copy it with your changes and share the copy. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
        
    1. Click the **Filter** icon ![Filter icon](assets/filter-icon.png) to add a filter to the view. Results are filtered immediately in the list. You cannot save and name filters. Filters are remembered when you access the page in future and they are part of shared views.

        >[!TIP]
        >
        ><span class="preview">To apply a personalized filter, select one of the following options for a field value: 
        >
        ><div class="preview">
        >
        >* **Me (logged in user)** to refer to the logged-in user in fields referring to users. 
        >
        >* **My teams** or **My home team** to refer to your teams in fields referring to teams. 
        >
        >* **My groups** or **My home group** to refer to your groups in fields referring to groups.
        >
        >* **My company** to refer to your company in fields referring to companies.
        > 
        >* **My roles** or **My primary role** to refer to your job roles in fields referring to roles. 
        >
        ></div>

    1. Click the **Columns** icon ![Columns icon](assets/columns-icon.png) to select which columns to display or to hide in the view. 
    1. Hover over the name of a column, then click the down-pointing arrow to the left of the column name, then click one of the following:
        * **Rename**, to add a **Custom label** for the column. The name of the original field in Workfront does not change. 
        * **Sort**, to sort the list by the selected field. A sorting icon indicating the direction of the sorting is added to the column header. 
    1. Click the **+** icon in the upper-right corner of the list to add or remove columns to the list, then click **Save**. 

        The **Column manager** opens. 
    
        You can add only existing fields to the list view. 
        You cannot remove the primary field in the list view which displays in the first column. 
    
    1. <span class="preview">Click the **Format cells** icon ![Format cells icon](assets/format-cells-icon.png). The **Format** box opens.</span> <!--change the name of the box when they update it-->
        <span class="preview">Do the following: </span>

        1. <span class="preview">Click **Add condition**.</span>
        1. <span class="preview">In the **If** line, select  a field and choose a field value and add a modifier. Modifiers change, depending on the field type you choose. </span>

            >[!TIP]
            >
            ><span class="preview">Only fields visible in the list view are available for conditional formatting.</span>

        1. <span class="preview">(Optional) Instead of adding a field value, click the **Compare to another field** icon ![Compare to another field](assets/compare-to-another-field-icon.png) and choose a field whose value you want to compare to the value of your selected field. For example, you can compare the Project Owner and the Project Sponsor fields. </span>

            >[!TIP]
            >
            ><span class="preview">Only fields visible in the list view are available for conditional formatting. The fields you compare must be of the same type. </span>

        1. <span class="preview">(Optional) Click **Add condition** in the **If** line to add more conditions to the same rule.</span>

            >[!TIP]
            >
            ><span class="preview">You can add up to 10 conditions in a conditioning rule and you can have up to 20 rules for a field.</span>

        1. <span class="preview">Click the **Or** connector between conditions to change to **And** and to indicate that multiple conditions must be met at the same time. **Or** is the default connector.</span>  
        1. <span class="preview">In the **Format** line, select a field to indicate which column will be formatted.</span> <!--edit this area, if it changes names??-->
        1. <span class="preview">(Optional) Click the **color circle** icon ![Color circle icon](assets/color-circle.png) next to the field selected, to expand it and choose another color in the **Cell fill** area to change the color of the background in a cell or pick a color from the **Text color** area to change the color of text in a cell.</span>
        1. <span class="preview">Click the **Text format** icon ![Text format icon](assets/text-format-icon.png) and select from the following options to format the text in a cell:</span> 
            * <span class="preview">Bold</span>
            * <span class="preview">Italic</span>
        
        1. <span class="preview">Turn on the **Apply to row** setting to apply the formatting to the entire row of the field that meets the conditions.</span>         
        1. <span class="preview">(Optional) Click **Add condition** in the **Format** box to add another rule for another field and the repeat the steps above.</span> 
        1. <span class="preview">(Optional) Click **Clear all** to remove all formatting.</span>
        1. <span class="preview">Click outside the **Format** box to close it.</span>

            <span class="preview">This returns you to the list view.</span> 
            <span class="preview">The formatting is applied immediately to the list view.</span>
            <span class="preview">There is a blue dot next to the **Format cells** icon to indicate that the view has special formatting applied.</span>
    
    1. <span class="preview">(Optional) Click the **Grouping** icon ![Grouping icon](assets/grouping-icon.png) <!-have they updated this to "Grouping"??-> to group items in the list by a common field. Select one of the options, or use the search bar to find a field.</span>

        <span class="preview">The field must be a column in the list before you can group by it. Not all field types can be used for groupings.</span>

    1. <span class="preview">Click the **Row height** icon ![Row height icon](assets/row-height-icon.png) to update the vertical length of a row. Choose from the following options: </span>

        <div class="preview">
    
        * Short
        * Standard. This is the default choice. 
        * Medium
        * Tall
    
        </div>

    <!--leave these here, although they duplicate for Enhanced lists in Workfront-->

1. (Optional) Add a keyword in the search box in the upper-right corner of the list to search for an item. 

    Items that match your search term are highlighted in the list.

1. (Optional and conditional) In the projects <!--change projects to items here when more items will display in the Glist--> connected page, to add more items to the list and automatically connect them to the selected record, do one of the following:

    * Click **Connect records** in the upper-right corner of the list to add existing items.
    * Click **New row** at the bottom of the list to add new items. 
1. Click the name of a connected item in the list to open it in another browser tab. 
1. Double-click inside of a cell in the list to edit the information of a field, then press Enter to save your changes. 

    Some fields are read-only. For example, the percent complete of a project is a field calculated by the system and you cannot manually edit it. 

1. Hover over an item's name in the list and click the **More** menu [More menu](assets/more-menu.png) and click **View** to open the project in another tab
     
      Or

      Select one or more items, and notice the actions bar at the bottom of the list, then click one of the following, when available. Depending on which area you access the list view from, click on one of the following options: 
      
    * **Delete** to delete the item. Deleting a project disconnects it from the record and moves it to the Workfront's Recycle Bin. Workfront administrators can recover deleted projects up to 30 days after they were deleted. Deleting a form does not delete the requests or records created when the form was submitted. 
    * **Disconnect** to disconnect the project from the record. Disconnecting a project removes it and all the values of its lookup fields from the current record. 

        <!--update screen shot at preview release-->

        ![Actions bar in Connected records page List view](assets/actions-bar-connected-records-page-list-view.png)

    * **Edit form**: Opens a Planning request form and allows you to edit it.
    * **Unpublish**: Unpublishes a request form. This removes the form from the Requests area and users can no longer add requests to this record type. 
    * **Share**: Opens the Sharing box for a request form where you can share with others.
    * **Copy link**: Copies a link to a Planning request form so you can share it with other users. If the form is shared publicly, you can share the link with people outside of Workfront Planning. 

        ![Actions bar in Planning requests list](assets/actions-bar-in-inake-forms-list.png)

    

