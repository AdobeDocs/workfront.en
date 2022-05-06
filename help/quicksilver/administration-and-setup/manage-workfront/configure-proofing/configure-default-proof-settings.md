---
filename: configure-default-proof-settings
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configure default proof settings
description: These settings allow you to set default values that apply to all new proofs created by your users. However, users can override most of these settings when creating a proof.
---

# Configure default proof settings

These settings allow you to set default values that apply to all new proofs created by your users. However, users can override most of these settings when creating a proof.

## Configure new proof default settings

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup**.
1. In the left panel, click **Proofs** > **Proof settings**.
1. In the **New proof defaults** section, configure the following settings:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2">Recipients</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Require login</td> 
      <td> <p>Reviewers are required to log in using their email and password before they are allowed to view proofs created in your organization's account. When enabled, users cannot share the proof with Guest reviewers.</p> <p>Important: When enabled, login is required for all newly created proofs.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copy owner from original proof for new versions</td> 
      <td> <p>The owner of the first version a proof is also the owner of all consecutive versions of the proof, regardless of who creates these versions. This setting is enabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow users to delete their proof comments</td> 
      <td>Users can delete their own comments. This setting is enabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Require decisions to be electronically signed </td> 
      <td> <p>Decision makers are prompted to enter their Workfront login credential when they make a decision on a proof.</p> <p>Important: When enabled, users cannot share the proof with Guest reviewers who don't have login credentials.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2">Deadline</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Set the default deadline</td> 
      <td> <p>The system applies this deadline to all new proofs in your account that do not have an Automated Workflow.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notify recipients before proof is at-risk</td> 
      <td>Recipients are notified via email before the proof is considered at-risk depending on the deadline specified above.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2">Email notifications</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notify recipients when they are added to a proof</td> 
      <td>Recipients are notified via email when they are added to a proof.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

## Configure proof decisions

Users can use proof decisions to indicate the status of the proof after review.

>[!NOTE]
>
>The logic behind proof decisions is used to calculate the overall status of a proof workflow if there are multiple decisions of various levels. The decisions "Approved" and "Approved with changes" trigger the next stage in an automatic workflow.

To configure proof decisions:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click**Setup**.
1. In the left panel, click **Proofs** > **Proof settings**.
1. In the **Decisions**section, you can

   1. **Rename the decision**: Click on the text inside the decision box, and begin typing the new decision label.

      >[!TIP]
      >
      >Retain the logic for a decision when you rename it. For example, the default decision Rejected could be changed to *New version required*, but it should not be changed to *Send to Printers*.

      ![](assets/rename-decision-350x109.png)

   1. **Rearrange the decision order**: Drag the decision boxes in the order you want them to appear in the proofing viewer.

      ![](assets/move-decision-350x110.png)

   1. **Hide a decision**: Hover over the decision box, and click the Hide icon in the upper-right corner.

      ![](assets/hide-decision-350x109.png)

1. (Optional) To go back to the Workfront defaults, click **Restore defaults**.
1. Click **Save**.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Configure proof comment </h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Users can use actions to keep track of what needs to happen on each comment thread on a proof.</p>
-->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Actions</strong>section, you can</p>
   -->

   1. 
   
      <!--   
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Create a new action</strong>: Click New action</p>   
      -->   
   
   1. 
   
      <!--   
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Enable or disable an action</strong>: Select the toggle to </p>   
      -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create new actions</h3>
-->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click<strong>Setup</strong>.</p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the left panel, click <strong>Proofs</strong> > <strong>Proof settings</strong>.</p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Enable/Disable actions</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="adding-or-renaming-an-action"></a>Add or rename an action</h3>
-->

   <!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode"> From Workfront, click the Main Menu <img src="assets/main-menu-icon.png">, then click Proofing <img src="assets/proofing-in-main-menu.png"> to access Workfront Proof. </li>
   -->

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Settings</strong> >&nbsp;<strong>Account settings</strong> in the upper-right corner of the Workfront Proof interface, then click the <strong>Settings</strong> tab.</li>
   -->

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Do either of the following:
   <ul>
   <li>
   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new action, in the <strong>Actions</strong> section, click&nbsp;<strong>New action</strong>.</p>
   --><!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">There is no limit to the number of actions you can set up in your account.</p>
   --></li><!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">To rename an existing action, click <strong>Setup</strong> next to the action.</li>
   -->
   </ul></li>
   -->

   <!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Type a name for the action, then click <strong>Save</strong>.</li>
   -->

   <!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save.</strong></li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="deactivating-or-activating-an-action"></a>Deactivate or reactivate an action</h3>
-->

   <!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode"> From Workfront, click the Main Menu <img src="assets/main-menu-icon.png">, then click Proofing <img src="assets/proofing-in-main-menu.png"> to access Workfront Proof. </li>
   -->

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Settings</strong> >&nbsp;<strong>Account settings</strong> in the upper-right corner of the Workfront Proof interface, then click the <strong>Settings</strong> tab.</li>
   -->

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Setup</strong> next to the action you want to deactivate or reactivate.</li>
   -->

   <!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Activate</strong> or <strong>Deactivate</strong>, then click <strong>Save</strong>.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="reordering-actions"></a>Reorder actions</h3>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> From Workfront, click the Main Menu <img src="assets/main-menu-icon.png">, then click Proofing <img src="assets/proofing-in-main-menu.png"> to access Workfront Proof. </li>
<li value="2">Click <strong>Settings</strong> >&nbsp;<strong>Account settings</strong> in the upper-right corner of the Workfront Proof interface, then click the <strong>Settings</strong> tab.</li>
<li value="3"> <p>Click the blue up and down arrows next to&nbsp;<strong>Setup</strong>&nbsp;to reorder the actions.</p> <p> <img src="assets/re-order-actions-350x103.png" alt="Re-order_actions.png" style="width: 350;height: 103;"> </p> </li>
</ol>
-->

