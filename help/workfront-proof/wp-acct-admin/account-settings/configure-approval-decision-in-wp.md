---
filename: configure-approval-decision-in-wp
product: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configure approval decision options in Workfront Proof
description: As a Workfront Proof administrator using a Select or Premium edition plan, you can configure approval decision options in the following ways for all proofs created by Workfront Proof users in your organization:
---

# Configure approval decision options in Workfront Proof

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

As a Workfront Proof administrator using a Select or Premium edition plan, you can configure approval decision options in the following ways for all proofs created by Workfront Proof users in your organization:

* Change the name of the decision
* Change the order of the decisions shown in the proofing viewer
* Decide which decisions should display

This article explains the following:

## Configuring Decision Settings

<ol> 
 <li value="1">Click <span class="bold">Account Settings</span>.</li> 
 <li value="2">Open the <span class="bold">Decisions</span> tab.</li> 
 <li value="3">Make any of the following changes: 
  <ul>
   <li>To hide a decision, click <span class="bold">Hide</span> to the right of the decision you do not need.</li>
   <li><p>To rename a decision, click the decision name, edit it, then click outside of the box (or press Enter). Workfront Proof updates the name of the decision on all existing proofs in your system.</p><note type="important">
     Retain the logic for a decision when you rename it. For example, the default decision "Rejected" could be changed to "New version required," but it should not be changed to "Send to Printers").
    </note><p>If you would like to go back to the Workfront Proof defaults, you can click Restore default decisions.</p></li>
  </ul></li> 
</ol>

>[!NOTE]
>
><ul> 
 <li>The logic behind the decisions is used to calculate the overall status of a proof workflow if there are multiple decisions of various levels.</li> 
 <li>The decisions "Approved" and "Approved with changes" trigger the next stage in an automatic workflows.</li> 
 <li> <p>If you rename a decision and you&nbsp;would like to verify the logic, you can click <span class="bold">Activity</span> in the left navigation panel and check your Activity log where&nbsp;the original decisions display in brackets.</p> <p> <img src="assets/2016-12-20-1921-350x132.png" alt="2016-12-20_1921.png" style="width: 350;height: 132;"> </p> </li> 
</ul>

## Creating Decision Reasons

Decision reasons are a good way of capturing additional decision information about a proof.&nbsp;

<ol> 
 <li value="1">Click <span class="bold">Settings</span> > <span class="bold">Account Settings</span>.</li> 
 <li value="2">Open the <span class="bold">Decisions</span> tab.<br>By default, reasons are available to all decision makers on your proofs, but you can restrict that to Primary decision makers only.<br>Depending on your requirements, you can allow multiple reasons to be selected or you can make it a single choice list. You can also make reasons mandatory, which means that reviewers will have to pick a reason before they are allowed to save their decision on a proof.<br><img src="assets/reasons-setup-350x121.png" alt="Reasons_setup.png" style="width: 350;height: 121;"></li> 
 <li value="3">In the <span class="bold">Reasons</span> section, click <span class="bold">New reason</span>.<br><img src="assets/new-reason-350x135.png" alt="New_reason.png" style="width: 350;height: 135;"></li> 
 <li value="4">Type a title for the reasons section in the box that appears under <span class="bold">Reason</span>.</li> 
 <li value="5">If you want to include a text box, select <span class="bold">Include text box</span>.</li> 
 <li value="6">Click <span class="bold">Save</span>. <br><img src="assets/reasons-setup-2-350x146.png" alt="reasons_setup_2.png" style="width: 350;height: 146;"><br>The most important step is selecting the decisions that reasons should display on. If you forget to do that, the reasons are not going to show on your proofs.</li> 
 <li value="7">Check the boxes in the <span class="bold">Display reasons</span> column in the decisions list at the top of the page. You can select one or more decisions for your reasons.<br><img src="assets/reasons---decision-selection-350x150.png" alt="reasons_-_decision_selection.png" style="width: 350;height: 150;"></li> 
</ol>

## Creating a Post Decision Message

You can create a post decision message to display after a reviewer saves their decision on the proof.&nbsp;

<ol> 
 <li value="1">Click <span class="bold">Settings</span> > <span class="bold">Account Settings</span>.</li> 
 <li value="2">Open the <span class="bold">Decisions</span> tab.</li> 
 <li value="3">In the <span class="bold">Post decision message</span> section, click <span class="bold">Edit</span> at the end of the <span class="bold">Message</span> row.<br>You can also decide if you want the message to be displayed to all decision makers or if you want to limit it to the Primary decision maker.<br><img src="assets/post-decision-message-set-up-350x125.png" alt="post_decision_message_set_up.png" style="width: 350;height: 125;"></li> 
 <li value="4">In the&nbsp;<span class="bold">Display message column</span>, specify the decisions this message should be displayed on. <br>If you do not&nbsp;select at least one decision, the message will not&nbsp;show on your proofs. Be sure to check at least one box in this column.<br><img src="assets/post-decision-message-set-up-2-350x151.png" alt="post_decision_message_set_up_2.png" style="width: 350;height: 151;"></li> 
</ol>

