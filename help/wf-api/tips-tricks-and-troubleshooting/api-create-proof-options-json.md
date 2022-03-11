---
filename: api-create-proof-options-json
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Add advanced proofing options when creating a proof through the Adobe Workfront API
description: You can create proofs through the Workfront API by using the Document createProof action. This action accepts the advancedProofingOptions parameter, which has the value type of string. To include advanced proofing options in your createProof action, you must input the options in the advancedProofingOptions parameter in JSON format.
---

# Add advanced proofing options when creating a proof through the Adobe Workfront API

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

This example shows fields and formatting that you can use when creating your JSON for the 

```
advancedProofingOptions
```

parameter. Your 

```
advancedProofingOptions
```

JSON&nbsp;file can have more or fewer fields than shown here. You may want to examine your organization's network data while using advanced proofing in Workfront, and base your JSON on the fields and values commonly used by your organization.

[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"stages"</span>: [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"name"</span>: <span style="color: #dd1144; ">"stage1"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"lockOn"</span>: <span style="color: #008080; ">1</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"position"</span>: <span style="color: #008080; ">1</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isPrivate"</span>: <span style="color: #008080; ">false</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"activateOn"</span>: <span style="color: #008080; ">1</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"recipients"</span>: [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"name"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"role"</span>: <span style="color: #008080; ">5</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"email"</span>: <span style="color: #dd1144; ">"user1_email@example.com"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"recipient_id"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"notifications"</span>: <span style="color: #008080; ">0</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isPrimaryDecisionMaker"</span>: <span style="color: #008080; ">null</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"name"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"role"</span>: <span style="color: #008080; ">5</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"email"</span>: <span style="color: #dd1144; ">"user2_email@example.com"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"recipient_id"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"notifications"</span>: <span style="color: #008080; ">0</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isPrimaryDecisionMaker"</span>: <span style="color: #008080; ">false</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;],<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isMandatory"</span>: <span style="color: #008080; ">false</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"deadlineDate"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"deadlineTime"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isOneApproval"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"activateOnDate"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"parentPosition"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"activateOnDecision"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"deadlineCalculateOn"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"deadlineBusinessDays"</span>: <span style="color: #008080; ">null</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;],<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"message"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"subject"</span>: <span style="color: #dd1144; ">""</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"templates"</span>: [],<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"hasMessage"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"canDownload"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customfields"</span>: [],<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"hasPublicSharing"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"isAutomatedWorkflow"</span>: <span style="color: #008080; ">true</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"stageBasedVisibility"</span>: <span style="color: #008080; ">0</span><br>}<br></code></pre>