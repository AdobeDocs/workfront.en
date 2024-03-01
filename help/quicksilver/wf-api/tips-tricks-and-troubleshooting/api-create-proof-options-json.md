---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Add advanced proofing options with Adobe Workfront API
description: Add advanced proofing options with Adobe Workfront API
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
---

# Add advanced proofing options when creating a proof through the Adobe Workfront API

When creating a proof in the Workfront API, you can add advanced proofing options.

Use one of the following workflows to add proofing options to a proof using the API:

* (Recommended) Create a simple proof using the Workfront API, then add advanced proofing options to the proof using the ProofHQ API 

* Create a proof with advanced proofing options using JSON in the Workfront API

## Create a proof using the Workfront and ProofHQ&nbsp;APIs (Recommended) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

This section describes how to create a proof with advanced proofing options through the Workfront API, using a combination of Workfront and ProofHQ APIs.

The ProofHQ API includes a variety of actions not available to proofs in the Workfront API. By using these actions, you can modify or configure the proof with more precision than is available in the Workfront API.

For an overview of the ProofHQ&nbsp;API, see the [PoofHQ Overview](../../proofhq-api/general/overview.md). You can also refer to the [ProofHQ Documentation](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* The Workfront API is a REST-ful API. The ProofHQ API is a SOAP API.
>* Proofs created in the ProofHQ API are not automatically linked to Workfront. Therefore, we recommend creating proofs in the Workfront API before updating them with the ProofHQ&nbsp;API.
>

### Create a proof with advanced proofing options

1. Create a proof using the `Document createProof` action in the Workfront API.

   >[!NOTE]
   >
   >When creating the proof, set `{}` as the value for the `advancedProofingOptions` parameter.

1. After the proof is created, use the ProofHQ&nbsp;API to add any advanced options.

### Examples

This section shows some sample updates that you can make with the ProofHQ API.

**Examples:** 

* [A Proof can be downloaded, has a message, and is shared publicly](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly) 
* [Update a stage so that it is not private, not mandatory, and requires only one approval](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval) 
* [Add two recipients to a proof with no primary decision maker](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**A Proof can be downloaded, has a message, and is shared publicly**

Documentation for this endpoint can be found on the [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html) page.

<!-- [Copy](javascript:void(0);) --> 

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**Update a stage so that it is not private, not mandatory, and requires only one approval**

Documentation for this endpoint can be found on the [ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) page.

<!-- [Copy](javascript:void(0);) --> 

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**Add two recipients to a proof with no primary decision maker**

Documentation for this endpoint can be found on the [ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) page.

<!-- [Copy](javascript:void(0);) --> 

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Create a proof using JSON&nbsp;in the Workfront API

This section describes how to create a proof with advanced proofing options through the Workfront API, using JSON as a parameter value in the Workfront API

### Create a proof with advanced proofing options

You can create proofs through the Workfront API by using the `Document createProof` action. This action accepts the `advancedProofingOptions` parameter, which has the value type of `string`. To include advanced proofing options in your `createProof` action, you must input the options in the `advancedProofingOptions` parameter in JSON format.

>[!NOTE]
>
>It can be difficult to predict the fields to include in your advancedProofingOptions JSON. You may want to examine your organization's network data while using advanced proofing in Workfront, and base your JSON on the fields and values commonly used by your organization.
>
>Because these fields can be difficult to predict, we recommend creating a proof using the Workfront API, then updating it using the ProofHQ&nbsp;API. For more information, see [Create a proof using the Workfront and ProofHQ APIs (Recommended)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) in this article

### Example

This example shows fields and formatting that you can use when creating your JSON for the `advancedProofingOptions` parameter. Your `advancedProofingOptions` JSON file can have more or fewer fields than shown here. 

**Example:** 

<!-- [Copy](javascript:void(0);) --> 

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
