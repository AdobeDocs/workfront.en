---
filename: preview-sandbox
content-type: overview;how-to-procedural
product: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Preview Sandbox Testing Environment- Workfront Proof
description: The Preview Sandbox is a testing environment that serves as a replica of your live environment and is refreshed each weekend by Workfront Proof.
---

# Preview Sandbox Testing Environment- `Workfront Proof`

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product `Workfront Proof`. For information on proofing inside `Adobe Workfront`, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

The Preview Sandbox is a testing environment that serves as a replica of your live environment and is refreshed each weekend by `Workfront Proof`.&nbsp;

## Understanding&nbsp;the Preview Sandbox

The Preview Sandbox serves as an environment where users in your organization&nbsp;can safely test and work with&nbsp;data from the Production&nbsp;environment without affecting the Production environment. It&nbsp;is ideal for running training sessions, testing out new features, and determining setup functionality.&nbsp;

Also, new product features are uploaded to the Preview Sandbox environment before they are&nbsp;delivered to the Production environment. Your users can try out new functionality there without affecting their usual workflow in the Production environment.

The Preview Sandbox contains your actual production&nbsp;data. Data flows from Production to Preview, and not in reverse. It refreshes every weekend, so the data can be up to one week behind the Production environment. Items created since the last refresh time are in the Preview Sandbox environment until the following refresh.

## Accessing the Preview Sandbox

By default, as a system administrator, you have access to the Preview Sandbox environment. If you cannot access the Preview Sandbox environment as described in this section, contact your `Workfront administrator` or our Support&nbsp;team.

* [Accessing the Preview Sandbox as a Stand-Alone Workfront Proof Customer](#accessing-the-preview-sandbox-as-a-stand-alone-proofhq-customer) 
* [Accessing the Preview Sandbox as a Workfront+Workfront Proof Customer](#accessing-the-preview-sandbox-as-a-workfront-proofhq-customer)

### Accessing the Preview Sandbox as a Stand-Alone `Workfront Proof`&nbsp;Customer

1. Navigate to this URL:  `https://preview.proofhq.com`.
1. Log in using your Preview credentials.  
   Your Preview credentials should be the same as your Production credentials unless you changed them in Production after the Preview refresh happened. The logins are synchronized only when a refresh occurs, which takes place every weekend. They do not synchronize automatically.

### Accessing the Preview Sandbox as a Workfront+ `Workfront Proof` Customer

As a system administrator, you can access the `Workfront Proof` Preview Sandbox via the `Workfront` interface.&nbsp;

To access the `Workfront Proof`&nbsp;Preview Sandbox:

<ol> 
 <li value="1"> Log in to your <span>Workfront</span> environment. </li> 
 <li value="2"> Click <span class="bold">Setup</span> in the Global Navigation bar. </li> 
 <li value="3">Click<span class="bold">&nbsp;System </span>><span style="line-height: 1.5;" class="bold">&nbsp;Preferences</span>.<br></li> 
 <li value="4"> In the <span class="bold">Test Environments</span> section, click <span class="bold">Sandbox Preview</span>.<br></li> 
 <li value="5"> Log in with your Preview credentials.<br>Your Preview credentials should be the same as your Production credential unless you changed them in Production after the Preview refresh happened.&nbsp;The logins are synchronized only when a refresh occurs. They do not synchronize automatically. </li> 
 <li value="6"> Click the <span>Workfront Proof</span>&nbsp;icon in the Global Navigation Bar.<br><img src="assets/proof-access-proofhq-350x39.png" alt="proof_access_proofhq.png" style="width: 350;height: 39;"><br>The <span>Workfront Proof</span>&nbsp;Preview environment displays. </li> 
</ol>

## Receiving Emails from the Preview Sandbox

Email notifications are never triggered from the `Workfront Proof`&nbsp;Preview environment.&nbsp;
