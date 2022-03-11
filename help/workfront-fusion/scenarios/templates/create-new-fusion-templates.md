---
filename: create-new-fusion-templates
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Create new templates in Adobe Workfront Fusion
description: You can create new scenario templates in Adobe Workfront Fusion.
---

# Create new templates in `Adobe Workfront Fusion`

You can create new scenario templates in `Adobe Workfront Fusion`.

>[!TIP]
>
>Before creating a new template, you can check the Public templates tab to ensure that the template you want to create is not already available.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Create a new template

<ol> 
 <li value="1"> <p>Click <span class="bold">Templates </span><img src="assets/fusion-template-icon.png"> in the left navigation panel.</p> </li> 
 <li value="2"> <p>Click <span class="bold">Create a new template</span> in the top-right corner.</p> </li> 
 <li value="3"> <p>(Optional) Rename the template by replacing the default <span class="bold">New template name</span> in the top-left corner.</p> </li> 
 <li value="4"> <p>(Optional) To change the language of your template, click Set up a template <img src="assets/fusion-scenario-settings-icon.png"> and select the language from the Language drop-down. </p> <note type="important">
   The Languages selection corresponds to the languages available in the system settings and concerns only the name of the public template and its description. You can't change a template language once the template has been saved.
  </note> </li> 
 <li value="5"> <p>(Optional) To enter a description of the template, click Set up a template <img src="assets/fusion-scenario-settings-icon.png"> and enter the description.</p> </li> 
 <li value="6"> <p>Add apps, modules, and tools in the same way as you would do when creating a standard scenario. </p> <p>To add contextual help to the modules, see <a href="#wizard" class="MCXref xref">Set up Wizard functionality</a> in this article.</p> <p>For more information on building a scenario, see <a href="../../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario</a>.</p> <note type="note">
   If your template includes modules that require adding the connection, credentials, or other privacy-sensitive information, this information is not shared with the template users.
  </note> </li> 
 <li value="7"> <p>(Optional) Click <span class="bold">Run once</span> to test your template.</p> </li> 
 <li value="8"> <p>Click the <span class="bold">Save</span> icon <img src="assets/save-icon.png">.</p> </li> 
</ol>

>[!NOTE]
>
>By saving your template you make it visible for all your team members. If you want your template to be accessible outside of your team you need to publish it and then use a shared link, or ask your administrator to approve and publish the template.

## Set up Wizard functionality

The `Workfront Fusion` template wizard allows you to provide future users of your template with instructions or information related to the specific fields used in modules.

1. Click the module added to the template to see the module's fields.
1. Locate the field where you want to add Wizard information, and enable `Use in Wizard` for that field.
1. Enter the information you want to make visible for users into the Help field.
1. (Optional) To allow users to see this text when using the template, enable `Use as default value`.
1. Repeat steps 2-4 for each field that you want to provide information for.
1. Click `OK` to save changes and close the module.

