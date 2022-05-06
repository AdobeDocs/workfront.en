---
filename: api-create-proof-options-json
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Add advanced proofing options when creating a proof through the Adobe Workfront API
description: When creating a proof in the Workfront API, you can add advanced proofing options.
---

# Add advanced proofing options when creating a proof through the Adobe Workfront API

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

When creating a proof in the Workfront API, you can add advanced proofing options.

Use one of the following workflows to add proofing options to a proof using the API:

* (Recommended) Create a simple proof using the Workfront API, then add advanced proofing options to the proof using the ProofHQ API 
* Create a proof with advanced proofing options using JSON in the Workfront API

## Create a proof using the Workfront and ProofHQ&nbsp;APIs (Recommended) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

This section describes how to create a proof with advanced proofing options through the Workfront API, using a combination of Workfront and ProofHQ APIs.

The ProofHQ API is a powerful tool with a wide variety of actions not available to proofs in the Workfront API. by using these actions, you can modify or configure the proof with more precision than is available in the Workfront API.

For an overview of the ProofHQ&nbsp;API, see [Overview](../../proofhq-api/general/overview.md).

For ProofHQ&nbsp;API documentation, see [ProofHQ](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* The Workfront API is a REST-ful API. The ProofHQ API is a SOAP API.
>* Proofs created in the ProofHQ API are not automatically linked to Workfront. Therefore, we recommend creating proofs in the Workfront API before updating them with the ProofHQ&nbsp;API.
>

### Create a proof with advanced proofing options

1. Create a proof using the 

   ```
   Document createProof
   ```

   action in the Workfront API

   >[!NOTE]
   >
   >When creating the proof, do not include a value for the advancedProofingOptions parameter.

1. After the proof is created, use the ProofHQ&nbsp;API to add any advanced options.

### Examples

This section shows some sample updates that you can make with the ProofHQ API.

``` ```**Examples: **``````

* [Proof can be downloaded, has a message, and is shared publicly](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly) 
* [Update a stage so that it is not private, not mandatory, and requires only one approval](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval) 
* [Add two recipients to a proof with no primary decision maker](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

#### Proof can be downloaded, has a message, and is shared publicly  {#proof-can-be-downloaded-has-a-message-and-is-shared-publicly}

Documentation for this endpoint can be found on the [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html) page.

[Copy](javascript:void(0);) 
<pre><code><span style="color: #63a35c; "><soapenv:Envelope xmlns:<span style="color: #795da3; ">soapenv</span><span style="color: #df5000; ">="http://schemas.xmlsoap.org/soap/envelope/"</span> xmlns:<span style="color: #795da3; ">soap</span><span style="color: #df5000; ">="https://{{soap_host}}/"</span>></span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><soapenv:Header/></span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><soapenv:Body></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><soap:updateProof></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><SessionID></span>{{session_id}}<span style="color: #63a35c; "></SessionID></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><FileID></span>{{file_id}}<span style="color: #63a35c; "></FileID></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><OwnerID></span>0<span style="color: #63a35c; "></OwnerID></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><Name></span>{{proof_name}}}<span style="color: #63a35c; "></Name></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><Subject></span>Email subject here<span style="color: #63a35c; "></Subject></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><Message></span>Email message here<span style="color: #63a35c; "></Message></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><EnableDownload></span>true<span style="color: #63a35c; "></EnableDownload></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><EnableTeamURL></span>true<span style="color: #63a35c; "></EnableTeamURL></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></soap:updateProof></span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></soapenv:Body></span><br><span style="color: #63a35c; "></soapenv:Envelope></span><br></code></pre>

#### Update a stage so that it is not private, not mandatory, and requires only one approval {#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval}

Documentation for this endpoint can be found on the [ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) page.

[Copy](javascript:void(0);) 
<pre><code><span style="color: #63a35c; "><soapenv:Envelope xmlns:<span style="color: #795da3; ">soapenv</span><span style="color: #df5000; ">="http://schemas.xmlsoap.org/soap/envelope/"</span> xmlns:<span style="color: #795da3; ">soap</span><span style="color: #df5000; ">="https://{{soap_host}}/"</span>></span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><soapenv:Header/></span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><soapenv:Body></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><soap:updateWorkflowProofStage></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><SessionID></span>{{session_id}}<span style="color: #63a35c; "></SessionID></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><FileID></span>{{proof_id}}<span style="color: #63a35c; "></FileID></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><Stage></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><stage_id></span>{{stage_id}}<span style="color: #63a35c; "></stage_id></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><name></span>{{stage_name}}<span style="color: #63a35c; "></name></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><stage_one_decision_only></span>true<span style="color: #63a35c; "></stage_one_decision_only></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><stage_private></span>false<span style="color: #63a35c; "></stage_private></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><mandatory></span>false<span style="color: #63a35c; "></mandatory></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></Stage></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></soap:updateWorkflowProofStage></span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></soapenv:Body></span><br><span style="color: #63a35c; "></soapenv:Envelope></span><br></code></pre>

#### Add two recipients to a proof with no primary decision maker {#add-two-recipients-to-a-proof-with-no-primary-decision-maker}

Documentation for this endpoint can be found on the [ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) page.

[Copy](javascript:void(0);) 
<pre><code><span style="color: #63a35c; "><soapenv:Envelope xmlns:<span style="color: #795da3; ">soapenv</span><span style="color: #df5000; ">="http://schemas.xmlsoap.org/soap/envelope/"</span> xmlns:<span style="color: #795da3; ">soap</span><span style="color: #df5000; ">="https://{{soap_host}}/"</span>></span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><soapenv:Header/></span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><soapenv:Body></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><soap:addWorkflowProofReviewers></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><SessionID></span>{{session_id}}<span style="color: #63a35c; "></SessionID></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><FileID></span>{{proof_id}}<span style="color: #63a35c; "></FileID></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><Recipients></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><item></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><email></span>{{recipient_email_1}}<span style="color: #63a35c; "></email></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><role></span>5<span style="color: #63a35c; "></role></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><name></span>{{recipient_name_1}}<span style="color: #63a35c; "></name></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><primary_decision_maker></span>false<span style="color: #63a35c; "></primary_decision_maker></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><stage_id></span>{{stage_id}}<span style="color: #63a35c; "></stage_id></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></item></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><item></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><email></span> {{recipient_email_2}} <span style="color: #63a35c; "></email></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><role></span>5<span style="color: #63a35c; "></role></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><name></span> {{recipient_name_2}} <span style="color: #63a35c; "></name></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><primary_decision_maker></span>false<span style="color: #63a35c; "></primary_decision_maker></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><stage_id></span>{{stage_id}}<span style="color: #63a35c; "></stage_id></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></item></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></Recipients></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "><SuppressNewProofNotification></SuppressNewProofNotification></span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></soap:addWorkflowProofReviewers></span><br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #63a35c; "></soapenv:Body></span><br><span style="color: #63a35c; "></soapenv:Envelope></span><br></code></pre>

## Create a proof using JSON&nbsp;in the Workfront API

This section describes how to create a proof with advanced proofing options through the Workfront API, using JSON as a parameter value in the Workfront API

### Create a proof with advanced proofing options

You can create proofs through the Workfront API by using the 

```
Document createProof
```

action. This action accepts the 

```
advancedProofingOptions
```

parameter, which has the value type of 

```
string
```

. To include advanced proofing options in your 

```
createProof
```

action, you must input the options in the 

```
advancedProofingOptions
```

parameter in JSON format.

>[!NOTE]
>
>It can be difficult to predict the fields to include in your advancedProofingOptions JSON. You may want to examine your organization's network data while using advanced proofing in Workfront, and base your JSON on the fields and values commonly used by your organization.
>
>Because these fields can be difficult to predict, we recommend creating a proof using the Workfront API, then updating it using the ProofHQ&nbsp;API. For more information, see [Create a proof using the Workfront and ProofHQ APIs (Recommended)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) in this article

### Example

This example shows fields and formatting that you can use when creating your JSON for the 

```
advancedProofingOptions
```

parameter. Your 

```
advancedProofingOptions
```

JSON&nbsp;file can have more or fewer fields than shown here. 

``` ```**Example: **`````` 
[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"stages"</span>: [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"name"</span>: <span style="color: #dd1144; ">"stage1"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"lockOn"</span>: <span style="color: #008080; ">1</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"position"</span>: <span style="color: #008080; ">1</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isPrivate"</span>: <span style="color: #008080; ">false</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"activateOn"</span>: <span style="color: #008080; ">1</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"recipients"</span>: [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"name"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"role"</span>: <span style="color: #008080; ">5</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"email"</span>: <span style="color: #dd1144; ">"user1_email@example.com"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"recipient_id"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"notifications"</span>: <span style="color: #008080; ">0</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isPrimaryDecisionMaker"</span>: <span style="color: #008080; ">null</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"name"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"role"</span>: <span style="color: #008080; ">5</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"email"</span>: <span style="color: #dd1144; ">"user2_email@example.com"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"recipient_id"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"notifications"</span>: <span style="color: #008080; ">0</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isPrimaryDecisionMaker"</span>: <span style="color: #008080; ">false</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;],<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isMandatory"</span>: <span style="color: #008080; ">false</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"deadlineDate"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"deadlineTime"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isOneApproval"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"activateOnDate"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"parentPosition"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"activateOnDecision"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"deadlineCalculateOn"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"deadlineBusinessDays"</span>: <span style="color: #008080; ">null</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;],<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"message"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"subject"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"templates"</span>: [],<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"hasMessage"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"canDownload"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customfields"</span>: [],<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"hasPublicSharing"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isAutomatedWorkflow"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"stageBasedVisibility"</span>: <span style="color: #008080; ">0</span><br>}<br></code></pre>