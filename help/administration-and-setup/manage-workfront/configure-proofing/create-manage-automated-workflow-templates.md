---
filename: create-manage-automated-workflow-templates
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Create and manage Automated Workflow templates
description: As an Adobe Workfront administrator, if your organization’s content review process is often repeated or content is often reviewed by the same people, you can create Automated Workflow templates that contain those reviewers with proof roles and notification settings that you specify. An Automated Workflow template can be simple with just one or two reviewers or complex with many stages and dependencies.
---

# Create and manage Automated Workflow templates

As an *Adobe Workfront administrator*, if your organization’s content review process is often repeated or content is often reviewed by the same people, you can create Automated Workflow templates that contain those reviewers with *proof* roles and notification settings that you specify. An Automated Workflow template can be simple with just one or two reviewers or complex with many stages and dependencies.

Automated Workflow templates make it easy to create a *proof* with an Automated Workflow. When a user creates a *proof*, they simply choose the template they need.

You can easily change any Automated Workflow template, adding or removing reviewers and stages, at any time. And *proof* creators who use the template can add or remove reviewers for the *proof*.

Consider the following when you use an Automated Workflow template:

1. `<li style="font-style: normal;">An Automated Workflow template's settings determine&nbsp;what you can do with the Automated Workflow for a <em>proof</em>. For example, if the Add a stage button disabled in the template, it is not visible as you work with the Automated Workflow settings for the <em>proof</em>. </li>` `<li style="font-style: normal;">When a person is added to a sage in an Automated Workflow template, but also already present as a reviewer on the <em>proof</em>, applying the template removes the reviewer from the stage. If you don't add another reviewer to the stage, a message will prompt you to add one. </li>` `<li style="font-style: normal;">Your ability to modify an Automated Workflow template depends on the template settings configured by the <em>Workfront administrator</em>, as described in <a href="#" class="MCXref xref selected">Create and manage Automated Workflow templates</a>. If the ability to modify the template is disabled, only the owner of the template can modify&nbsp;it.</li>`

For information about Automated Workflows, see [Automated Workflow overview](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><em>Adobe Workfront</em> plan</a> </td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access configurations</td> 
   <td> <p>You must have Administrator selected in your <em>Proof</em> Permission Profile. For more information, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configure a user's proofing access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create an Automated Workflow template

<ol> 
 <li value="1"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     From 
     <em>Workfront</em>, click the Main Menu 
     <img src="assets/main-menu-icon.png">, then click Proofing 
     <img src="assets/proofing-in-main-menu.png"> to access 
     <em>Workfront Proof</em>.
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    From 
    <em>Workfront</em>, click the Main Menu 
    <img src="assets/main-menu-icon.png">, then click Proofing 
    <img src="assets/proofing-in-main-menu.png"> to access 
    <em>Workfront Proof</em>.
   </MadCap:conditionalText> </p> </li> 
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
     <td>You can select the <em>Workfront administrator</em> or <em>Workfront Proof administrator</em> who will manage the template.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Template group</td> 
     <td> <p> If your organization's Automated Workflows are organized into groups, you can select the name of the group. See <a href="#group" class="MCXref xref">Create Automated Workflow template groups</a> later in this article for more information.</p> </td> 
    </tr> <draft-comment>
     <tr data-mc-conditions=""> 
      <td role="rowheader">Template timezone </td> 
      <td> <p>The default timezone for the template is the one you are working in. If the timezone of the proof creators and reviewers who will be using the template is different, you can change it here to ensure that stage deadlines are set at the right times for those users. </p> </td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions=""> 
     <td role="rowheader">Template timezone </td> 
     <td> <p>The default timezone for the template is the one you are working in. If the timezone of the proof creators and reviewers who will be using the template is different, you can change it here to ensure that stage deadlines are set at the right times for those users. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Allow</td> 
     <td> <p>You can select the stage activities you want available to the person creates <em>proofs</em> using the template.</p> <draft-comment>
       <p class="warning" data-mc-autonum="<b>Warning: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="autonumber"><span><b>Warning: </b></span></span>If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any <em>proof</em> using this template will be able to add a stage or share the <em>proof</em>. <draft-comment>
         <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
        </draft-comment><span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span><br></p>
      </draft-comment><p class="warning" data-mc-autonum="<b>Warning: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="autonumber"><span><b>Warning: </b></span></span>If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any <em>proof</em> using this template will be able to add a stage or share the <em>proof</em>. <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span><br></p> </td> 
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
       <li> <p><span class="bold">Proof creation</span>: In the drop-down list under <span class="bold">Deadline (+ business days)</span>, select the number of business days you want to add to the <em>proof</em> creation date to automatically set a deadline on the <em>proof</em>.</p> </li> 
       <li><span class="bold">When stage starts</span>: In the drop-down list under <span class="bold">Deadline (+ business days)</span>, select the number of business days you want to add to the stage activation date to automatically set a deadline on the <em>proof</em>.</li> 
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
     <td>Hides comments and decisions from to people who are not added to the stage or who are not <em>Workfront administrators</em><draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Supervisors and above
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Supervisors and above
      </MadCap:conditionalText>. For more information, see <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Automated Workflow overview</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Do not allow this stage to be deleted</td> 
     <td> <p>Makes the stage mandatory.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>If the <em>proofs</em> that will use this template are always sent to the same people in the stage, add them here so that users don't have to add them every time they create a <em>proof</em>..</p> <p> Choose each person's <span class="bold">Role</span> on the <em>proofs</em> that will use this template and the <span class="bold">Email alerts</span> you want the user to receive when working on <em>proofs</em> that use this template. </p> <p>For information about roles on a <em>proof</em>, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configure default proofing roles</a>. For information about <em>proof</em> email alerts, see the section <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configure proof defaults for a user</a> in the article&nbsp;<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.</p> <p>Each user can be added to only one stage. You can add as many users as you want to a stage.</p> <note type="tip">
   You can drag and drop reviewers names between stages on the stages diagram. Available stages are highlighted in blue.
  </note> </li> 
 <li value="7"> <p>Repeat the two previous steps for any other stages you want to add to the template.</p> <p>At the top of the <span class="bold">Workflow</span> section, you can see a diagram of the Automated Workflow you are setting up. As you continue to add stages, they appear on the diagram with lines showing the dependencies between them. You can click on a stage in the diagram to view the settings for that stage.</p> <p>If you don't need to see the diagram, you can click <span class="bold">Hide Diagram</span>.</p> </li> 
 <li value="8"> <p>In the <span class="bold">Share template with</span> section, click an option (if the template is not already shared with the whole organization) to specify who will be able to use it. </p> <p>By default, new Automated Workflow templates are shared with everyone in your organization.</p> </li> 
 <li value="9"> <p>Click <span class="bold">Create</span>.&nbsp;</p> </li> 
</ol>

## Modify an Automated Workflow template

As a *Workfront Proof administrator*, you can modify an Automated Workflow template. Your changes are saved automatically as you make them.

<ol> 
 <li value="1"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     From 
     <em>Workfront</em>, click the Main Menu 
     <img src="assets/main-menu-icon.png">, then click Proofing 
     <img src="assets/proofing-in-main-menu.png"> to access 
     <em>Workfront Proof</em>.
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    From 
    <em>Workfront</em>, click the Main Menu 
    <img src="assets/main-menu-icon.png">, then click Proofing 
    <img src="assets/proofing-in-main-menu.png"> to access 
    <em>Workfront Proof</em>.
   </MadCap:conditionalText> </p> </li> 
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
     <td>You can select the <em>Workfront administrator</em> or <em>Workfront Proof administrator</em> who will manage the template.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Template group</td> 
     <td> <p> If your organization's Automated Workflows are organized into groups, you can select the name of the group. See <a href="#group" class="MCXref xref">Create Automated Workflow template groups</a> later in this article for more information.</p> </td> 
    </tr> <draft-comment>
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Template timezone </td> 
      <td> <p>The default timezone for the template is the one you are working in. If the timezone of the proof creators and reviewers who will be using the template is different, you can change it here to ensure that stage deadlines are set at the right times for those users. </p> </td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
     <td role="rowheader">Template timezone </td> 
     <td> <p>The default timezone for the template is the one you are working in. If the timezone of the proof creators and reviewers who will be using the template is different, you can change it here to ensure that stage deadlines are set at the right times for those users. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Allow</td> 
     <td> <p>Select the stage activities you want available to those who create <em>proofs</em> using the template. </p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span>If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any <em>proof</em> using this template will be able to add a stage or share the <em>proof</em>.<br></p> </td> 
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
       <li> <p><span class="bold">Deadline calculated from proof creation</span>: In the <span class="bold">Set the stage deadline</span> drop-down list, select the number of business days you want to add to the <em>proof</em> creation date to automatically set a deadline on the <em>proof</em>.</p> </li> 
       <li><span class="bold">Deadline calculated from stage activation</span>: In the <span class="bold">Set the stage deadline</span> drop-down list, select the number of business days you want to add to the stage activation date to automatically set a deadline on the <em>proof</em>.</li> 
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
     <td>Add reviewers to the stage or delete the stage.<p>If each of your <em>proofs</em> is sent to the same people in a particular stage, you can specify their names here name so that you don't have to add them every time you create a <em>proof</em>. Type and select the name of a user you want to add to the stage, then add their <span class="bold">Role</span> on the <em>proof</em> and <span class="bold">Email alerts</span> settings you want for the user. For information about <em>proofing</em> roles, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configure default proofing roles</a>. For information about <em>proof</em> email alerts, see the section <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configure proof defaults for a user</a> in the article&nbsp;<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.</p><p>You can add as many users as you want to a stage</p><note type="tip">
       You can drag and drop reviewers names between stages on the stages diagram. Available stages are highlighted in blue.
      </note></td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>Repeat the step for any other stages you want to add to the template.</p> <p>At the top of the <span class="bold">Workflow</span> section, you can see a diagram of the Automated Workflow you are setting up. As you continue to add stages, they appear on the diagram with lines showing the dependencies between them. You can click on a stage in the diagram to view the settings for that stage.</p> <p>If you don't need to see the diagram, you can click <span class="bold">Hide Diagram</span>.</p> </li> 
 <li value="7"> <p>In the <span class="bold">Shared with</span> section, if you want to delete a user, click the More <img src="assets/more-icon.png"> button to the right, then click <span class="bold">Remove</span>. </p> </li> 
</ol>

## Create Automated Workflow template groups

As a *Workfront administrator*, you can view and manage all of the Automated Workflow templates in your organization's account. It can be helpful to organize templates into groups.

To create an Automated Workflow template group:

<ol> 
 <li value="1"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     From 
     <em>Workfront</em>, click the Main Menu 
     <img src="assets/main-menu-icon.png">, then click Proofing 
     <img src="assets/proofing-in-main-menu.png"> to access 
     <em>Workfront Proof</em>.
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    From 
    <em>Workfront</em>, click the Main Menu 
    <img src="assets/main-menu-icon.png">, then click Proofing 
    <img src="assets/proofing-in-main-menu.png"> to access 
    <em>Workfront Proof</em>.
   </MadCap:conditionalText> </p> </li> 
 <li value="2"> <p>Click <span class="bold">Workflows</span> in the left panel.</p> </li> 
 <li value="3"> <p>On the <span class="bold">Workflow</span> tab, click&nbsp;<span class="bold">New</span>&nbsp;>&nbsp;<span class="bold">New template group</span>.</p> </li> 
 <li value="4">Type a descriptive name for the new template group, then press <span class="bold">Enter</span>.</li> 
</ol>

You can move the templates between groups by dragging and dropping.

## Manage Automated Workflow templates

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    From 
    <em>Workfront</em>, click the Main Menu 
    <img src="assets/main-menu-icon.png">, then click Proofing 
    <img src="assets/proofing-in-main-menu.png"> to access 
    <em>Workfront Proof</em>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   From 
   <em>Workfront</em>, click the Main Menu 
   <img src="assets/main-menu-icon.png">, then click Proofing 
   <img src="assets/proofing-in-main-menu.png"> to access 
   <em>Workfront Proof</em>.
  </MadCap:conditionalText> </li> 
 <li value="2">In the left panel in <em>Workfront Proof</em>, click <span class="bold">Workflows</span>.</li> 
 <li value="3">On the <span class="bold">Workflows</span> page that appears, do any of the following:
  <ul>
   <li>Add a new template</li>
   <li>Add a new template group </li>
   <li>Delete one or more template groups</li>
   <li>Access a template's details</li>
   <li>Drag a template to a different template group</li>
  </ul></li> 
</ol>

