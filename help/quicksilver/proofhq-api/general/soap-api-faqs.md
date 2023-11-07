---
title: SOAP API FAQs
description: SOAP API FAQs
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
---
# SOAP API FAQs

## How do I create my first file proof?

It takes 3 simple steps:

**Step 1**: Upload the file to Workfront Proof by sending it via a Post request to&nbsp; [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). We will return you the file hash - this is very important! Note that at this stage you will not see anything in your account, all you've done so far is send us the file but not told us what to do with it.

**Step 2**: If you don't have Session ID yet, obtain one by using the doLogin() or getSessionID() methods. Use the former to 'log in' using a user's email address and password or the latter method if you have the user's email address and authentication token.

**Step 3:** Now it's time to create your proof. Use the createProof() method and send us at least the required fields (currently there's only 5 of them). Ensure you set the Hash parameter to the file hash returned during "Step 1" as this allows us to determine which file to use when creating your proof.

If you now log in to your account you will see the proof.

## How do I create my first web snapshot proof?

It takes 2 simple steps:

**Step 1**: If you don't have a Session ID yet, obtain one by using the doLogin() or getSessionID() methods. Use the former to 'log in' using a user's email address and password or the latter method if you have the user's email address and authentication token.

**Step 2:**Now it's time to create your proof. Use the createProof() method and send us at least the required fields (currently there's only 5 of them). Ensure you set the Hash parameter to "web" and the SourceName parameter as the URL of the web page you want to capture.

If you now log in to your account you will see the proof.

## What's the difference between a proof and a version?

In Workfront Proof versions are displayed as a single Proof. Clicking on a specific version in the Web UI will display that version's details. In reality, each version is a separate proof and the Web UI displays these together.

From the perspective of the API, each version is a separate proof and the proofs are linked together by their IDs.

**createProof()** will always create **version 1** of the proof. Let's assume for our example the ID returned for this proof "100".

When using&nbsp;**createProofVersion()** always send in the previous version's ID. If we want to create **version 2** on proof "100", we **pass in "100" for the ParentFileID** parameter. This tells the system that this proof should be version 2 of the set. The method will return a unique proof ID, for our example let's say this is "101".

If a third version i.e. **version 3** is required, you will call **createProofVersion()** again and this time **pass in "101" for the ParentFileID** which will ensure the linked list of versions is properly created.

## Do I need to obtain a new Session ID before every call?

It's important to point out that every Session ID is essentially a user performing the actions.&nbsp;

You do not need to obtain a new Session ID before every call to the API and it will remain valid for 24 hours. The expiry time resets every time you make a call to the API.

## What is a proof / personal URL?

**Team/Public**: Each proof version has a unique Team (Public) URL. If enabled, it will open the proof in read only mode. You can obtain the Team URL using the [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) method.

**Personal**: A personal URL is unique for every reviewer and proof version. If a proof set contains 3 versions and a reviewer is on all versions, the reviewer will have 3 unique personal URLs. A personal URL opens the proof version with the reviewer already identified and should therefore be kept safe and not shared. Personal URLs can be obtained by calling the [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers)&nbsp;method and then iterating over each&nbsp; [SOAPRecepientObject](http://api.proofhq.com/home/objects/soaprecipientobject)&nbsp;and getting the parameter "proof_url".

## >How to include custom parameters when opening the miniproof?

The miniproof allows you to embed the proofing tool in your own page. A "referer" parameter can be included as part of the miniproof in order to provide a redirect URL when a user clicks on the close button in the miniproof. You can include any number of custom parameters as part of this redirect URL by appending them using the escaped '&' character e.g. %26.

For example, the miniproof URL
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` must be encoded as&nbsp;
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` in order for the custom parameters to be passed through.

## How to create a Java Web Service Client?

[This video](http://screencast.com/t/xsSNrqs5b) shows how you can create a Java Web Service client using Eclipse and the Workfront Proof WSDL definition.
 