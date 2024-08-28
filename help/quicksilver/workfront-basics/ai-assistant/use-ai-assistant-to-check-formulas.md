---
title: Revise calculated field formulas with AI Assistant
content-type: reference
description: You can use AI Assistant to resolve errors in your invalid custom expressions in calculated fields.
author: Becky
feature: Get Started with Workfront
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
---
# Generate or revise calculated field formulas with AI Assistant

You can use AI Assistant to generate formulas based on a prompt you provide. You can also resolve errors in your invalid custom expressions in calculated fields.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>New: Prime or Ultimate</p>
       <p>or</p>
       <p>Current: Not available</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>or</p>
       <p>Current: Not available</p></td>
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Generate a calculated field expression

## Revise a calculated field expression

When you are creating the calculated field in the custom form builder, an error message appears under the field if the formula is invalid.

![Invalid expression error](assets/invalid-expression.png)

AI Assistant can help you revise your formula into a valid calculated field expression.

To revise an invalid calculated field expression:

1. Click the **AI Assistant** icon ![AI Assistant icon](assets/ai-assistant-icon.png) near the upper-right corner of the screen.
1. in the prompt area near the bottom of the AI Assistant panel, enter a prompt such as:
`Rewrite this formula to remove the invalid expression error`
1. Copy the invalid expression from the custom form builder, and paste it into the prompt area.
1. Press **Enter**.

   AI Assistant may take a few moments to generate the revised formula, depending on how large or complex the formula is.
1. View the revised formula in the AI Assistant panel.
1. (Optional) Copy the revised formula from the AI Assistant panel, and paste it into the calculated field in the custom form builder.

>[!NOTE]
>
>We recommend testing the calculated field to ensure that it retrieves the expected result.

For more information on calculated fields in Workfront, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

