---
filename: create-and-manage-custom-fields
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Create and manage custom fields in Workfront Proof
description: A Select or Premium Workfront Plan is required to use this feature. For more information about the various plans available, see Workfront Plans.
---

# Create and manage custom fields in Workfront Proof

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

A Select or Premium Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)

Custom fields allow you to capture additional data when creating a new proof, a new user, or a new guest.

For example, users creating a new proof may want to include an additional section that will allow them to capture a Job Number, Department Code, or Supplier Reference.

>[!NOTE]
>
>* Capturing this type of information on the New proof page via Custom fields will also let you reduce the length of your proof name, as these details will not have to be included in the name. For information about the New proof page, see "Creating Proofs in Workfront Proof."
>
>Once a Custom field has been used on a proof, user, or contact, you will not be able to delete it or edit the field type. However, you will be able to hide it (via the Custom field Settings page) so that it is not used for new items.
>
>If you make a Custom field Section hidden, all the fields within the section will also be hidden even if the individual fields are set as visible.

This article explains how to do the following:

## Create custom fields

First, you need to set up the Custom Field section to which you will add custom fields.&nbsp;

1. Click **Settings** >**Account Settings**, then open the **Custom fields** tab.

1. Click **Add custom field section**&nbsp;in the relevant module (Proof, Users, or Contacts).
1. Type a **Name** for custom field section, then click **Save**.

   Now you can set up custom fields within the section:

1. Click the **Custom fields settings** tab to refresh the page.&nbsp;
1. Click the name of your new custom field section top open the **Custom field section** page for the new section.
1. Click the **New custom field** near the upper-right corner.
1. In the **New custom field** page that appears, specify the details for the custom field:

   | **Mandatory** |Workfront requires users to complete the field. |
   |---|---|
   | **Searchable** |Allows users to be able to find items by searching on the Custom field data. |
   | **Hidden** |Hides the custom field on the New proof, New guest, and New user pages |

   {style="table-layout:auto"}

1. Click **Save**.
1. In the **Custom field** page that appears, click the **Custom fields settings** tab to refresh the page.&nbsp;

1. Make any further changes to the settings for the field:

   * Hide or unhide the custom field section by clicking the **More**&nbsp;(three dot) menu to the right of the custom field section name, then clicking **Hide section** or **Unhide section**.
   
   * Hide or unhide the custom field by clicking the **More**&nbsp;(three dot) menu to the right of the custom field section name, then clicking **Hide custom field** or **Unhide custom field**.
   
   * Change the order of the fields using the up/down arrows that display to the right of their names (if you have added multiple fields in a section).

1. Open the **Visibility rules** tab.  
   Visibility rules allow you to dictate which additional fields are shown, based on the completion of the initial Custom field. For example, if the dependent field is A and the Controlling field is X, this means that Field A will only be visible if field X is completed.

   You can use controlling values&nbsp;to determine the values in the controlling field which, if picked, will result in the dependent field being visible. For example, imagine that the dependent field is A and the controlling field is X and you set the controlling values in X to be options 1 and 2 only. This means that field A will be visible only if field X option 1 or 2 is selected. This means that if field X options 3 or 4 are selected, then field A does not display. Open the **Visibility rules** tab.

   To add a visibility rule:

   1. Click **New visibility rule**&nbsp;for the module where you want to add the rule.
   1. Select the settings you want for the rule, then click **Save**.

1. Open the **Dependency rules** tab.

   Dependency rules let you determine the options available in the dependent field when certain options are selected in the controlling field. For example, if the dependent field is "B" and the controlling field is "Y," you could set it up as follows:

   If option 1 in field Y is chosen, only options 1 and 2 in field B are shown.

   If option 2 in field Y is chosen, only options 3 and 4 in field B are shown.

   To add a dependency rule:

   1. Click **New dependency rule** for the module you want to add the rule.
   1. Select the settings you want for the dependency, then click **Save**.

## Manage your custom fields

You can view and edit the details of your Custom field section or individual Custom fields.

1. Click **Settings** >**Account Settings**, then open the **Custom fields** tab.

1. Click the name of the custom field section or individual custom field.&nbsp;
1. (Conditional) If you are managing a custom field section, make any of the following changes in the **Custom field section** page:

   * Edit the name of the section.
   * Move it to a different module.
   * Hide/show the section.

1. (Conditional) If you are managing a custom field, make any of the of the following changes on the **Custom field**&nbsp;page:

   * Move the field to a different section.
   * Edit the name of the field.
   * Input help text (a question mark icon will appear next to the field section and the text will appear on hover over).
   * Enable/disable the **Mandatory** setting on the field.
   * Enable/disable the **Searchable** setting on the field.
   * Hide/unhide the field.
   * Edit the field type.
   * Set/edit a default value for the field.
   * Set up visibility and dependency rules (as described above in steps 11 and 12).

