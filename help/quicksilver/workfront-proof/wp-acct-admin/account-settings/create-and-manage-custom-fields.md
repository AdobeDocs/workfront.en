---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Create and manage custom fields in [!DNL Workfront Proof]
description: A Select or Premium [!DNL Workfront] Plan is required to use this feature. For more information about the various plans available, see Workfront Plans.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
---
# Create and manage custom fields in [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

A Select or Premium [!DNL Workfront] Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://business.adobe.com/products/workfront/pricing.html).

Custom fields allow you to capture additional data when creating a new proof, user, or guest. For example, users creating a new proof may want to include an additional section that will allow them to capture a Job Number, Department Code, or Supplier Reference.

>[!NOTE]
>
>* Capturing this type of information on the New proof page via custom fields also lets you reduce the length of your proof name, as these details will not have to be included in the name. 
>
>* Once a custom field has been used on a proof, user, or contact, you can't delete it or edit the field type. However, you will be able to hide it via the Custom field Settings page so it's not used for new items.
>
>* If you hide a custom field section, all the fields within the section will also be hidden, even if the individual fields are set as visible.

## Create custom fields

{{step1-to-proofing}}

1. In the upper-right corner of the page, click **Account settings**.

1. On the **Account settings** page select the **Custom fields** tab. 

1. Click **[!UICONTROL Add custom field section]** on the right side of the module (**Proof**, **Users**, or **Contacts**) you want to add the custom field to. The **Section details** tab opens.

1. Type a **Name** for custom field section, then click **[!UICONTROL Save]**.

1. Click the **[!UICONTROL Custom fields settings]** tab to refresh the page. The new custom field section displays under its assigned module.

      ![Custom fields settings tab](assets/custom-field-settings-tab.png)

1. Click the name of your new custom field section to open the **Custom fields section** tab.

1. On the upper-right side of the page, click the **[!UICONTROL New custom field]** button. The **New custom field** page appears.

1. Specify the **Field details**: 

   * **Name**: Enter the custom field name.
   * **Help**: Enter help text that will display in a tooltip.
   * **Mandatory**: Check this box to require the user to complete the field.
   * **Searchable** (Conditional): Check this box to make the custom field searchable.
   * **Hidden**: Check this box to hide the custom field on the **New proof**, **New guest**, and **New user** pages.

1. Specify the **Field type** and details:

   * **Type**: Select the custom field type. 
   * **List items**: (Conditional) Add the list items that will appear in the custom field.
   * **Default value**: Select the default value for this custom field. This option will vary depending on the custom field type that's selected.

1. Click **[!UICONTROL Save]**.

1. Make any further changes to the settings for the field:

   * Hide or unhide the custom field section by clicking the **More** ![More button](assets/more-button-small.png) menu to the right of the custom field section name, then clicking **[!UICONTROL Hide section]** or **[!UICONTROL Unhide section]**.
   * Hide or unhide the custom field by clicking the **More** ![More button](assets/more-button-small.png) menu to the right of the custom field section name, then clicking **[!UICONTROL Hide custom field]** or **[!UICONTROL Unhide custom field]**.
   * Change the order of the fields using the up/down arrows that display to the right of their names (if you have added multiple fields in a section).

1. Click the **[!UICONTROL Visibility rules]** tab.

   Visibility rules allow you to dictate which additional fields are shown based on the completion of the initial custom field. For example, if the dependent field is A and the Controlling field is X, this means that Field A will only be visible if field X is completed.

   You can use controlling values to determine the values in the controlling field which, if picked, will result in the dependent field being visible. For example, imagine that the dependent field is A and the controlling field is X and you set the controlling values in X to be options 1 and 2 only. This means that field A will be visible only if field X option 1 or 2 is selected. Additionally, if field X options 3 or 4 are selected, then field A doesn't display. 

   >[!NOTE]
   >
   >Only List and Radio custom field types can be used for the controlling field in a visibility rule, while the dependent field can be any field type.

   To add a visibility rule:

   1. Click **[!UICONTROL New visibility rule]** for the module you want to add the rule to.

   1. Select the settings you want for the rule, then click **[!UICONTROL Save]**.

1. Open the **[!UICONTROL Dependency rules]** tab.

   Dependency rules let you determine the options available in the dependent field when certain options are selected in the controlling field. For example, if the dependent field is "B" and the controlling field is "Y," you could set it up as follows:

   * If option 1 in field Y is chosen, only options 1 and 2 in field B are shown.

   * If option 2 in field Y is chosen, only options 3 and 4 in field B are shown.

   >[!NOTE]
   >
   >Only List and Radio custom field types can be used for the dependent and controlling fields in a dependency rule.

   To add a dependency rule:

   1. Click **[!UICONTROL New dependency rule]** for the module you want to add the rule to.

   1. Select the settings you want for the dependency, then click **[!UICONTROL Save]**.

## Manage your custom fields

You can view and edit the details of your Custom field section or individual custom fields.

{{step1-to-proofing}}

1. In the upper-right corner of the page, click **Account settings**.

1. On the **Account settings** page select the **Custom fields** tab. 

1. Click the name of the custom field section or individual custom field.

1. (Conditional) If you are managing a custom field section, make any of the following changes in the **[!UICONTROL Custom field section]** page:

   * Edit the name of the section.
   * Move it to a different module.
   * Hide/show the section.

1. (Conditional) If you are managing a custom field, make any of the of the following changes on the **[!UICONTROL Custom field]** page:

   * Move the field to a different section.
   * Edit the name of the field.
   * Edit help text.
   * Enable/disable the **[!UICONTROL Mandatory]** setting on the field.
   * (Conditional) Enable/disable the **[!UICONTROL Searchable]** setting on the field.
   * Hide/unhide the field.
   * Edit the field type.
   * Set/edit a default value for the field.
   * Set up visibility and dependency rules.
