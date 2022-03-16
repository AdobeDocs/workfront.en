

# Add a section break to a custom form

In a custom form, if you need to limit access to custom fieldsor image widgets for certain users, you can place them under a section break, and then grant only certain users access to the section.

For example, if you needed to retire some fields on a custom form that are no longer used, you could create a section for them called "Retired fields" at the bottom of the form, then allow only system administrators to access it. This is better than deleting the fields and losing all of the historical data that was entered into it; some of that data might still be needed for reports.

The access settings you select for a section break are directly tied to the permissions users have on the Workfront object where the custom form is attached. You can hide or show the fields in a section based on whether the user has access to view, contribute to, or manage that object. Or you can set a section to Admin Only so that only users with a system administrator access level can access it. For information about permissions on objects, see [Overview of sharing permissions on objects in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms, fields, and section breaks](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> Adobe Workfront plan* Any 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> Access level configurations* Administrative access to custom forms For information about how Workfront administrators grants this access, see Grant users administrative access to certain areas.  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Add a section break to a custom form

1. Begin creating or editing a custom form, as described in [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Add custom fieldsand widgets to the form, as described in [Add a custom field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
1. While still creating or editing the custom form, on the **Add a field** tab, click **Section Break**.

   <!--
   RESHOOT THIS WHEN THEY ADD IMAGE WIDGET TO LIST OF FIELDS
   -->

   ![](assets/click-section-break-350x237.jpg)

1. On the `Field Settings` tab, configure the options that are available for the type of field you are adding:

   <table cellspacing="0"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label for the section. It displays above the section when users view the field on a custom form added to an object.</p> <p>You can change the label at any time.</p> <p>Important: Avoid using special characters in this label. They don't display correctly in reports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Type text if you want to explain to users what the section is for. This displays below the section's label on the custom form.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Specify which fields should appear on the form, based on selections users make in existing fields. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Display logic and skip logic on a custom form</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Additional settingsGrant access</p> </td> 
      <td> <p> Select the permissions that users need on an object where the custom form is attached in order to view this section and edit its field values. For information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects in Adobe Workfront</a>.</p> 
       <ul> 
        <li> <p role="rowheader">
          <!--
           Use if production/ifpreview structure when stories release
          --><b>In order to VIEW this section, people must have permission to</b>Users with the following access to the object can view the section </p> 
         <ul> 
          <li><span class="bold">View</span>: The user needs View permissions to the object in order to view the section.</li> 
          <li><b>ContributeLimited Edit</b>: (Available only if the object is a project, task, issue, or user) The user needs Contribute permissions to the object in order to view the section.</li> 
          <li><span class="bold">Manage</span>Edit: The user needs Manage permissions to the object to be able to view this section.</li> 
          <li> <p><span class="bold">Admin only</span>: Only Workfront administrators can see this section.</p> <p>Note: Users without the permissions you specify here can't see the values of the fieldsand image widgets in the section. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li> 
         </ul> </li> 
        <li> <p>
          <!--
           Use if production/ifpreview structure when stories release
          --><b>In order to EDIT this section, people must have permission to</b>Users with the following access to the object can edit field values in the section </p> 
         <ul> 
          <li><b>ContributeLimited Edit</b>: (Available only if the object is a project, task, issue, or user) The user needs Contribute permissions to the object in order to edit field values in the section.</li> 
          <li><![CDATA[
       ]]><b><span class="bold">Manage</span>Edit</b>: The user needs Manage permissions to the object to be able to edit field values in this section. </li> 
          <li><b>Admin only</b>: Only Workfront administrators can edit field values in this section. </li> 
         </ul> </li> Associating multiple object types with your form can impact the viewing and editing permissions you configure for a section in the form. For more information, see How multiple object types can affect a form's section breaks in this article. 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Drag at least one fieldor image widget to the new section.

   This is required before you save the section.

1. Click `Done`.

   >[!TIP]
   >
   >You can click `Apply` at any point while you are creating a custom form to save your changes and keep the form open.

1. If you want to continue building your custom form in other ways, continue on to one of the following articles:

  * [Add a custom field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2) 
  * [Reuse an existing custom field](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md) 
  * [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) 
  * [Position fields and widgets in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md) 
  * [Using an existing calculated custom field on a new custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md) 
  * [Display logic and skip logic on a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

Limit access to custom fields and image widgets that are not placed under a section break If you want to limit access for certain users on all fields and image widgets that are not placed under a section break, you can do so on the Form Settings tab. Begin creating or editing a custom form, as described in Create or edit a custom form. Add custom fields and widgets to the form, as described in Add a custom field to a custom form. While still creating or editing the custom form, open the Form settings tab.SHOW THIS WHEN THEY ADD SETTINGS Under Grant access, select the permissions that users need on an object where the custom form is attached in order to view this section and edit its field values. If you need information about permissions on objects, see Overview of sharing permissions on objects in Adobe Workfront. Users with the following access to the object can view the section View: Users need View permissions to the object in order to view the section. Limited Edit: (Available only if the object is a project, task, issue, or user) Users need needs Contribute permissions to the object in order to view the section. Edit: Users need Manage permissions to the object to be able to view this section. Admin only: Only Workfront administrators can see this section. Note: Users without the permissions you specify here can't see the values of the fields and image widgets in the section. This is also true if you display the values in reports or use them in calculated fields in text mode reporting. Users with the following access to the object can edit field values in the section Limited Edit: (Available only if the object is a project, task, issue, or user) The user needs Contribute permissions to the object in order to edit field values in the section. Edit: The user needs Manage permissions to the object to be able to edit field values in this section. Admin only: Only Workfront administrators can edit field values in this section. Note: Associating multiple object types with your form can impact the viewing and editing permissions you configure for a section in the form. For more information, see How multiple object types can affect a form's section breaks in this article. Click Done. Tip: You can click Apply at any point while you are creating a custom form to save your changes and keep the form open. If you want to continue building your custom form in other ways, continue on to one of the following articles: Add a custom field to a custom form Reuse an existing custom field Add or edit an image widget in a custom form Position fields and widgets in a custom form Add calculated data to a custom form Using an existing calculated custom field on a new custom form Display logic and skip logic on a custom form How multiple object types can affect a form's section breaks Some section break access settings are available only for certain object types. If you add an object type to a custom form that contains a section break, you might be prompted to switch to an access setting for the section break that is compatible with the new object type you are adding as well as the existing object types on the form. Example: The Limited Edit permission option is available for the Project, Task, Issue, and User object types; but not for the Portfolio, Program, Document, Company, Billing Record, Iteration, Expense, and Group object types. Imagine a custom form associated with the Project object type, with Limited Edit selected for a section break in the form. If you were to add the Portfolio object type to the form, the Limited Edit permission option would no longer be available for the section break in the form. An on-screen message would prompt you to choose the Edit option instead, because it is the most similar option to Limited Edit and it is compatible with both the Project object type and the Portfolio object type.  