

# Reuse an existing custom field

When you are creating or editing a custom form, you can add a custom field that already exists in the system.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Reuse an existing custom field

1. Begin creating or editing a custom form, as described in [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Click **Field Library**, then select the field in the list that appears.

   You cannot use an existing field more than once on a form.

   >[!IMPORTANT]
   >
   >When you modify an existing field, any changes you make impact that field on all forms where it is used.

1. Click **Apply**.
1. (Optional) Repeat the two previous steps to add any other existing fields .

   >[!NOTE]
   >
   >You can add up to 500 fields on a single custom form. However, performance degradation can occur when more than 100 fields exist on a form, depending on the complexity of the form. 
   >
   >
   >Examples of complex forms include forms with cascading parameters, calculated custom data fields, and multiple value options in a single field.

1. (Optional) Create and add any new fields you need that have not yet been created for your organization, as explained in [Reuse an existing custom field](#create) in this article.
1. (Optional) To position fields on the same row, drag them next to each other until a line appears between them.

   When you drop the field where you want it, a gray outline box appears around the two fields, indicating that they share a row. If you drag a field until the blue line appears above or below another field, the fields do not share a row.

   >[!NOTE]
   >
   >
   >   
   >   
   >   * You can use the **Preview** button in the lower-right corner to get an idea of how the fields will display in the form.
   >   * Fields may not display exactly the same way in the form, depending on how much screen space is available when a user is viewing it. For example, the third field in a row of fields may wrap to the next row of fields if horizontal space is limited.
   >   
   >

1. If you want to add a new custom field to the form, continue on to [Reuse an existing custom field](#create) in this article.

   Or

   If you want to continue building your custom form in other ways, continue on to one of the following articles:

   * [Position fields and widgets in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md) 
   * [Add a section break to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md) 
   * [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-image-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an image widget in a custom form</a> </li>   
     -->   
   
   * [Using an existing calculated custom field on a new custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md) 
   * [Display logic and skip logic on a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md) 
   * [Preview and complete a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

