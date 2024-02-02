---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Create and manage Automated Workflow templates
description: As an Adobe Workfront administrator, if your organization's content review process is often repeated or content is often reviewed by the same people, you can create Automated Workflow templates that contain those reviewers with proof roles and notification settings that you specify. An Automated Workflow template can be simple with just one or two reviewers or complex with many stages and dependencies.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
---
# Create and manage Automated Workflow templates

As an Adobe Workfront administrator, if your organization's content review process is often repeated or content is often reviewed by the same people, you can create Automated Workflow templates that contain those reviewers with proof roles and notification settings that you specify. An Automated Workflow template can be simple with just one or two reviewers or complex with many stages and dependencies.

Automated Workflow templates make it easy to create a proof with an Automated Workflow. When a user creates a proof, they simply choose the template they need.

You can easily change any Automated Workflow template, adding or removing reviewers and stages, at any time. And proof creators who use the template can add or remove reviewers for the proof.

Consider the following when you use an Automated Workflow template:

1. An Automated Workflow template's settings determine what you can do with the Automated Workflow for a proof. For example, if the Add a stage button disabled in the template, it is not visible as you work with the Automated Workflow settings for the proof. 
1. When a person is added to a sage in an Automated Workflow template, but also already present as a reviewer on the proof, applying the template removes the reviewer from the stage. If you don't add another reviewer to the stage, a message will prompt you to add one. 
1. Your ability to modify an Automated Workflow template depends on the template settings configured by the Workfront administrator, as described in . If the ability to modify the template is disabled, only the owner of the template can modify it.

For information about Automated Workflows, see [Automated Workflow overview](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>New: Any</p><p>Current: Pro or Higher</p><p>Legacy: Premium or Select</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p><p>Current: Work or Plan</p> <p>Legacy: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must have Administrator selected in your Proof Permission Profile. For more information, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configure a user's proofing access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Create an Automated Workflow template

{{step1-to-proofing}}

1. Click **Workflows** in the left panel.
1. On the **Workflow** tab, click **New** > **New template**.

1. In the **Details** section, specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Template name</td> 
      <td>(Required) Type a name for your template. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Template owner</td> 
      <td>You can select the Workfront administrator or Workfront Proof administrator who will manage the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Template group</td> 
      <td> <p> If your organization's Automated Workflows are organized into groups, you can select the name of the group. See <a href="#create-automated-workflow-template-groups" class="MCXref xref">Create Automated Workflow template groups</a> later in this article for more information.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Template timezone </td> 
      <td> <p>The default timezone for the template is the one you are working in. If the timezone of the proof creators and reviewers who will be using the template is different, you can change it here to ensure that stage deadlines are set at the right times for those users. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow</td> 
      <td> <p>You can select the stage activities you want available to the person creates proofs using the template.</p> 
      <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Stages** section, configure each stage of the Automated Workflow template.

   You can add multiple stages and create between them.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>The stage name displays on the Automated Workflow diagram at the top of the Workflow section, on the Proof Details page, and in the email notifications sent to reviewers.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activate stage</td> 
      <td> <p>Specify whether the stage is activated automatically or manually. For the first stage, you can select <strong>On proof creation</strong>, <strong>On a specific date &amp; time</strong>, or <strong>Manually</strong>.</p> <p>The other options become available when you add a second stage because they require you to select a parent stage. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deadline calculated from</td> 
      <td> <p>Specify how you want the deadline to be calculated:</p> 
       <ul> 
        <li> <p><strong>Proof creation</strong>: In the drop-down list under <strong>Deadline (+ business days)</strong>, select the number of business days you want to add to the proof creation date to automatically set a deadline on the proof.</p> </li> 
        <li><strong>When stage starts</strong>: In the drop-down list under <strong>Deadline (+ business days)</strong>, select the number of business days you want to add to the stage activation date to automatically set a deadline on the proof.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lock stage</td> 
      <td>Specify whether you want to allow the stage to be locked for comments. The options are to lock a stage manually or automatically, either when the next stage starts or when all decisions are made on the parent stage.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Primary decision maker</td> 
      <td> <p>The available decision makers display in the list only after you have added the reviewers to the stage.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Only one decision required</td> 
      <td>The review process for the stage will be completed as soon as one of the decision makers submits their decision. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Private stage</td> 
      <td>Hides comments and decisions from to people who are not added to the stage or who are not Workfront administrators<!--
        DRAFTED IN FLARE:
         Supervisors and above
        
       -->. For more information, see <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Automated Workflow overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Do not allow this stage to be deleted</td> 
      <td> <p>Makes the stage mandatory.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. If the proofs that will use this template are always sent to the same people in the stage, add them here so that users don't have to add them every time they create a proof..

   Choose each person's **Role** on the proofs that will use this template and the **Email alerts** you want the user to receive when working on proofs that use this template.

   For information about roles on a proof, see [Configure default proofing roles](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). For information about proof email alerts, see the section [Configure proof defaults for a user](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) in the article  [Configure email notification settings in Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Each user can be added to only one stage. You can add as many users as you want to a stage.

   >[!TIP]
   >
   >You can drag and drop reviewers names between stages on the stages diagram. Available stages are highlighted in blue.

1. Repeat the two previous steps for any other stages you want to add to the template.

   At the top of the **Workflow** section, you can see a diagram of the Automated Workflow you are setting up. As you continue to add stages, they appear on the diagram with lines showing the dependencies between them. You can click on a stage in the diagram to view the settings for that stage.

   If you don't need to see the diagram, you can click **Hide Diagram**.

1. In the **Share template with** section, click an option (if the template is not already shared with the whole organization) to specify who will be able to use it.

   By default, new Automated Workflow templates are shared with everyone in your organization.

1. Click **Create**. 

## Modify an Automated Workflow template

As a Workfront Proof administrator, you can modify an Automated Workflow template. Your changes are saved automatically as you make them.

1. From Workfront, click the Main Menu ![](assets/main-menu-icon.png), then click Proofing ![](assets/proofing-in-main-menu.png) to access Workfront Proof. 
1. Click **Workflows** in the left panel.
1. In the **Workflow templates** list that appears, click the template you want to modify.
1. In the **Details** section, specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Template name</td> 
      <td>(Required) Type a name for your template. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Template owner</td> 
      <td>You can select the Workfront administrator or Workfront Proof administrator who will manage the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Template group</td> 
      <td> <p> If your organization's Automated Workflows are organized into groups, you can select the name of the group. See <a href="#create-automated-workflow-template-groups" class="MCXref xref">Create Automated Workflow template groups</a> later in this article for more information.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Template timezone </td> 
      <td> <p>The default timezone for the template is the one you are working in. If the timezone of the proof creators and reviewers who will be using the template is different, you can change it here to ensure that stage deadlines are set at the right times for those users. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow</td> 
      <td> <p>Select the stage activities you want available to those who create proofs using the template. </p> <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Workflow** section, change the name of any stage and expand it's settings ![](assets/arrow-button.png) to make any needed changes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Deadline calculated from</td> 
      <td> <p>Specify how you want the deadline to be calculated:</p> 
       <ul> 
        <li> <p><strong>Deadline calculated from proof creation</strong>: In the <strong>Set the stage deadline</strong> drop-down list, select the number of business days you want to add to the proof creation date to automatically set a deadline on the proof.</p> </li> 
        <li><strong>Deadline calculated from stage activation</strong>: In the <strong>Set the stage deadline</strong> drop-down list, select the number of business days you want to add to the stage activation date to automatically set a deadline on the proof.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activate stage</td> 
      <td> <p>Specify whether the stage is activated automatically or manually. For the first stage, you can select <strong>On proof creation</strong>, <strong>On a specific date &amp; time</strong>, or <strong>Manually</strong>.</p> <p>The other options become available when you add a second stage because they require you to select a parent stage. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lock stage</td> 
      <td>Specify whether you want to allow the stage to be locked for comments. The options are to lock a stage manually or automatically, either when the next stage starts or when all decisions are made on the parent stage.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decision</td> 
      <td>Ends the stage the first time one of the decision makers submits their decision. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privacy</td> 
      <td>Hides comments and decisions from to people who are not added to the stage or who are not Supervisors and above in the account. For more information, see <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Automated Workflow overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stage deletion</td> 
      <td>Makes the stage mandatory.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">More <img src="assets/more-icon.png"></td> 
      <td>Add reviewers to the stage or delete the stage.<p>If each of your proofs is sent to the same people in a particular stage, you can specify their names here name so that you don't have to add them every time you create a proof. Type and select the name of a user you want to add to the stage, then add their <strong>Role</strong> on the proof and <strong>Email alerts</strong> settings you want for the user. For information about proofing roles, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configure default proofing roles</a>. For information about proof email alerts, see the section <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configure proof defaults for a user</a> in the article <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.</p><p>You can add as many users as you want to a stage</p><p>Tip: You can drag and drop reviewers names between stages on the stages diagram. Available stages are highlighted in blue.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Repeat the step for any other stages you want to add to the template.

   At the top of the **Workflow** section, you can see a diagram of the Automated Workflow you are setting up. As you continue to add stages, they appear on the diagram with lines showing the dependencies between them. You can click on a stage in the diagram to view the settings for that stage.

   If you don't need to see the diagram, you can click **Hide Diagram**.

1. In the **Shared with** section, if you want to delete a user, click the More ![](assets/more-icon.png) button to the right, then click **Remove**.

## Create Automated Workflow template groups {#create-automated-workflow-template-groups}

As a Workfront administrator, you can view and manage all of the Automated Workflow templates in your organization's account. It can be helpful to organize templates into groups.

To create an Automated Workflow template group:

1. From Workfront, click the Main Menu ![](assets/main-menu-icon.png), then click Proofing ![](assets/proofing-in-main-menu.png) to access Workfront Proof. 
1. Click **Workflows** in the left panel.
1. On the **Workflow** tab, click **New** > **New template group**.
1. Type a descriptive name for the new template group, then press **Enter**.

You can move the templates between groups by dragging and dropping.

## Manage Automated Workflow templates

1. From Workfront, click the Main Menu ![](assets/main-menu-icon.png), then click Proofing ![](assets/proofing-in-main-menu.png) to access Workfront Proof. 

1. In the left panel in Workfront Proof, click **Workflows**.
1. On the **Workflows** page that appears, do any of the following:

   * Add a new template
   * Add a new template group 
   * Delete one or more template groups
   * Access a template's details
   * Drag a template to a different template group
