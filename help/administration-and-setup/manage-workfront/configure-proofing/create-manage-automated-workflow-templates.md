---
filename: create-manage-automated-workflow-templates
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Create and manage Automated Workflow templates
description: As an Adobe Workfront administrator, if your organization’s content review process is often repeated or content is often reviewed by the same people, you can create Automated Workflow templates that contain those reviewers with proof roles and notification settings that you specify. An Automated Workflow template can be simple with just one or two reviewers or complex with many stages and dependencies.
---

# Create and manage Automated Workflow templates

As an `Adobe Workfront administrator`, if your organization’s content review process is often repeated or content is often reviewed by the same people, you can create Automated Workflow templates that contain those reviewers with `proof` roles and notification settings that you specify. An Automated Workflow template can be simple with just one or two reviewers or complex with many stages and dependencies.

Automated Workflow templates make it easy to create a `proof` with an Automated Workflow. When a user creates a `proof`, they simply choose the template they need.

You can easily change any Automated Workflow template, adding or removing reviewers and stages, at any time. And `proof` creators who use the template can add or remove reviewers for the `proof`.

Consider the following when you use an Automated Workflow template:

1. `<li style="font-style: normal;">An Automated Workflow template's settings determine&nbsp;what you can do with the Automated Workflow for a <span>proof</span>. For example, if the Add a stage button disabled in the template, it is not visible as you work with the Automated Workflow settings for the <span>proof</span>. </li>` `<li style="font-style: normal;">When a person is added to a sage in an Automated Workflow template, but also already present as a reviewer on the <span>proof</span>, applying the template removes the reviewer from the stage. If you don't add another reviewer to the stage, a message will prompt you to add one. </li>` `<li style="font-style: normal;">Your ability to modify an Automated Workflow template depends on the template settings configured by the <span>Workfront administrator</span>, as described in <a href="#" class="MCXref xref selected">Create and manage Automated Workflow templates</a>. If the ability to modify the template is disabled, only the owner of the template can modify&nbsp;it.</li>`

For information about Automated Workflows, see [Automated Workflow overview](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span>Adobe Workfront</span> plan</a> </td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access configurations</td> 
   <td> <p>You must have Administrator selected in your <span>Proof</span> Permission Profile. For more information, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configure a user's proofing access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Create an Automated Workflow template

<ol> 
 <li value="1"> <p> From Workfront, click the Main Menu , then click Proofing to access Workfront Proof. </p> </li> 
 <li value="2"> <p>Click <span class="bold">Workflows</span> in the left panel.</p> </li> 
 <li value="3">On the <span class="bold">Workflow</span> tab, click&nbsp;<span class="bold">New</span>&nbsp;>&nbsp;<span class="bold">New template</span>.</li> 
 <li value="4"> <p>In the <span class="bold">Details</span> section, specify the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Template name</td> 
     <td>(Required) Type a name for your template. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Template owner</td> 
     <td>You can select the <span>Workfront administrator</span> or <span>Workfront Proof administrator</span> who will manage the template.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Template group</td> 
     <td> <p> If your organization's Automated Workflows are organized into groups, you can select the name of the group. See <a href="#group" class="MCXref xref">Create Automated Workflow template groups</a> later in this article for more information.</p> </td> 
    </tr> Template timezone The default timezone for the template is the one you are working in. If the timezone of the proof creators and reviewers who will be using the template is different, you can change it here to ensure that stage deadlines are set at the right times for those users. 
    <tr> 
     <td role="rowheader">Allow</td> 
     <td> <p>You can select the stage activities you want available to the person creates <span>proofs</span> using the template.</p> <!--
       Warning: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. Test this. Andrzej thinks it's wrong info or a bug.
      --> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>In the <span class="bold">Stages</span> section, configure each stage of the Automated Workflow template.</p> <p>You can add multiple stages and create between them.</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Name</td> 
     <td> <p>The stage name displays on the Automated Workflow diagram at the top of the Workflow section, on the Proof Details page, and in the email notifications sent to reviewers.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Activate stage</td> 
     <td> <p>Specify whether the stage is activated automatically or manually. For the first stage, you can select <span class="bold">On proof creation</span>, <span class="bold">On a specific date & time</span>, or <span class="bold">Manually</span>.</p> <p>The other options become available when you add a second stage because they require you to select a parent stage. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Deadline calculated from</td> 
     <td> <p>Specify how you want the deadline to be calculated:</p> 
      <ul> 
       <li> <p><span class="bold">Proof creation</span>: In the drop-down list under <span class="bold">Deadline (+ business days)</span>, select the number of business days you want to add to the <span>proof</span> creation date to automatically set a deadline on the <span>proof</span>.</p> </li> 
       <li><span class="bold">When stage starts</span>: In the drop-down list under <span class="bold">Deadline (+ business days)</span>, select the number of business days you want to add to the stage activation date to automatically set a deadline on the <span>proof</span>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Lock stage</td> 
     <td>Specify whether you want to allow the stage to be locked for comments. The options are to lock a stage manually or automatically, either when the next stage starts or when all decisions are made on the parent stage.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Primary decision maker</td> 
     <td> <p>The available decision makers display in the&nbsp;list only after you have added the reviewers to the stage.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Only one decision required</td> 
     <td>The review process for the stage will be completed as soon as one of the decision makers submits their decision. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configure Proof Settings in Workfront Proof</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Private stage</td> 
     <td>Hides comments and decisions from to people who are not added to the stage or who are not <span>Workfront administrators</span><!--
       Supervisors and above
      -->. For more information, see <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Automated Workflow overview</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Do not allow this stage to be deleted</td> 
     <td> <p>Makes the stage mandatory.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>If the <span>proofs</span> that will use this template are always sent to the same people in the stage, add them here so that users don't have to add them every time they create a <span>proof</span>..</p> <p> Choose each person's <span class="bold">Role</span> on the <span>proofs</span> that will use this template and the <span class="bold">Email alerts</span> you want the user to receive when working on <span>proofs</span> that use this template. </p> <p>For information about roles on a <span>proof</span>, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configure default proofing roles</a>. For information about <span>proof</span> email alerts, see the section <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configure proof defaults for a user</a> in the article&nbsp;<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.</p> <p>Each user can be added to only one stage. You can add as many users as you want to a stage.</p> <note type="tip">
   You can drag and drop reviewers names between stages on the stages diagram. Available stages are highlighted in blue.
  </note> </li> 
 <li value="7"> <p>Repeat the two previous steps for any other stages you want to add to the template.</p> <p>At the top of the <span class="bold">Workflow</span> section, you can see a diagram of the Automated Workflow you are setting up. As you continue to add stages, they appear on the diagram with lines showing the dependencies between them. You can click on a stage in the diagram to view the settings for that stage.</p> <p>If you don't need to see the diagram, you can click <span class="bold">Hide Diagram</span>.</p> </li> 
 <li value="8"> <p>In the <span class="bold">Share template with</span> section, click an option (if the template is not already shared with the whole organization) to specify who will be able to use it. </p> <p>By default, new Automated Workflow templates are shared with everyone in your organization.</p> </li> 
 <li value="9"> <p>Click <span class="bold">Create</span>.&nbsp;</p> </li> 
</ol>

## Modify an Automated Workflow template

As a `Workfront Proof administrator`, you can modify an Automated Workflow template. Your changes are saved automatically as you make them.

<ol> 
 <li value="1"> <p> From Workfront, click the Main Menu , then click Proofing to access Workfront Proof. </p> </li> 
 <li value="2"> <p>Click <span class="bold">Workflows</span> in the left panel.</p> </li> 
 <li value="3">In the <span class="bold">Workflow templates</span> list that appears, click the template you want to modify.</li> 
 <li value="4"> <p>In the <span class="bold">Details</span> section, specify the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Template name</td> 
     <td>(Required) Type a name for your template. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Template owner</td> 
     <td>You can select the <span>Workfront administrator</span> or <span>Workfront Proof administrator</span> who will manage the template.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Template group</td> 
     <td> <p> If your organization's Automated Workflows are organized into groups, you can select the name of the group. See <a href="#group" class="MCXref xref">Create Automated Workflow template groups</a> later in this article for more information.</p> </td> 
    </tr> Template timezone The default timezone for the template is the one you are working in. If the timezone of the proof creators and reviewers who will be using the template is different, you can change it here to ensure that stage deadlines are set at the right times for those users. 
    <tr> 
     <td role="rowheader">Allow</td> 
     <td> <p>Select the stage activities you want available to those who create <span>proofs</span> using the template. </p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span>If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any <span>proof</span> using this template will be able to add a stage or share the <span>proof</span>.<br></p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>In the <span class="bold">Workflow</span> section, change the name of any stage and expand it's settings <img src="assets/arrow-button.png"> to make any needed changes:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Deadline calculated from</td> 
     <td> <p>Specify how you want the deadline to be calculated:</p> 
      <ul> 
       <li> <p><span class="bold">Deadline calculated from proof creation</span>: In the <span class="bold">Set the stage deadline</span> drop-down list, select the number of business days you want to add to the <span>proof</span> creation date to automatically set a deadline on the <span>proof</span>.</p> </li> 
       <li><span class="bold">Deadline calculated from stage activation</span>: In the <span class="bold">Set the stage deadline</span> drop-down list, select the number of business days you want to add to the stage activation date to automatically set a deadline on the <span>proof</span>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Activate stage</td> 
     <td> <p>Specify whether the stage is activated automatically or manually. For the first stage, you can select <span class="bold">On proof creation</span>, <span class="bold">On a specific date & time</span>, or <span class="bold">Manually</span>.</p> <p>The other options become available when you add a second stage because they require you to select a parent stage. </p> </td> 
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
     <td>Add reviewers to the stage or delete the stage.<p>If each of your <span>proofs</span> is sent to the same people in a particular stage, you can specify their names here name so that you don't have to add them every time you create a <span>proof</span>. Type and select the name of a user you want to add to the stage, then add their <span class="bold">Role</span> on the <span>proof</span> and <span class="bold">Email alerts</span> settings you want for the user. For information about <span>proofing</span> roles, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configure default proofing roles</a>. For information about <span>proof</span> email alerts, see the section <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configure proof defaults for a user</a> in the article&nbsp;<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.</p><p>You can add as many users as you want to a stage</p><note type="tip">
       You can drag and drop reviewers names between stages on the stages diagram. Available stages are highlighted in blue.
      </note></td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>Repeat the step for any other stages you want to add to the template.</p> <p>At the top of the <span class="bold">Workflow</span> section, you can see a diagram of the Automated Workflow you are setting up. As you continue to add stages, they appear on the diagram with lines showing the dependencies between them. You can click on a stage in the diagram to view the settings for that stage.</p> <p>If you don't need to see the diagram, you can click <span class="bold">Hide Diagram</span>.</p> </li> 
 <li value="7"> <p>In the <span class="bold">Shared with</span> section, if you want to delete a user, click the More <img src="assets/more-icon.png"> button to the right, then click <span class="bold">Remove</span>. </p> </li> 
</ol>

## Create Automated Workflow template groups

As a `Workfront administrator`, you can view and manage all of the Automated Workflow templates in your organization's account. It can be helpful to organize templates into groups.

To create an Automated Workflow template group:

1. From Workfront, click the Main Menu , then click Proofing to access Workfront Proof. 
1. Click `Workflows` in the left panel.
1. On the `Workflow` tab, click  `New` >  `New template group`.
1. Type a descriptive name for the new template group, then press `Enter`.

You can move the templates between groups by dragging and dropping.

## Manage Automated Workflow templates

1. From Workfront, click the Main Menu , then click Proofing to access Workfront Proof. 
1. In the left panel in `Workfront Proof`, click `Workflows`.

1. On the `Workflows` page that appears, do any of the following:

  * Add a new template
  * Add a new template group 
  * Delete one or more template groups
  * Access a template's details
  * Drag a template to a different template group

