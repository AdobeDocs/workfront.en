---
filename: create-status-web-proof
product: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Create a Static Website Proof using Workfront Proof
description: Important: This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see Proofing.
---

# Create a Static Website Proof using *Workfront Proof*

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product *Workfront Proof*. For information on proofing inside *Adobe Workfront*, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

You can create static *proofs* from your web pages. In addition, you can simulate various devices by defining screen resolution of the captures.

## Creating a Static Website Proof

<ol> 
 <li value="1">Open the New <em>proof</em> page, as described in <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md" class="MCXref xref" xrefformat="{para}">Generate Proofs in Workfront Proof</a>.</li> 
 <li value="2">Paste or type your URL in the <span class="bold">www.shareyourlink.com</span>&nbsp;box.</li> 
 <p>You can repeat this step to add multiple URLs.</p> 
 <li value="3">Just below this box, click the&nbsp;resolution (the default is 1366x768), then select any resolutions you want in the <span class="bold">Screensot resolution</span> box.<br>Select a smaller resolution if you want to <em>proof</em> designs for mobile devices. Generally, designs load as per screen/browser window resolution.</li> 
 <li value="4">Click <span class="bold">Look for subpages</span> if you&nbsp;want to&nbsp;include connected pages that are in the same domain/subdomain&nbsp;as the&nbsp;entered&nbsp;URL.<br><em>Workfront Proof</em> scans the connected pages and lists them below the <span class="bold">Look for subpages</span> option. You can select the pages you want to include.<br></li> <note type="tip">
   With the Combine 
  <em>proofs</em> feature you can submit all the web pages as a single multi-page 
  <em>proof</em>.
 </note> 
 <li value="5">Click <span class="bold">Done</span>, then finish configuring your <em>proof</em> as explained in <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md" class="MCXref xref" xrefformat="{para}">Generate Proofs in Workfront Proof</a>.</li> 
</ol>

## About Password-Protected Pages and Pages Requiring Authorization

*Workfront Proof* cannot capture a password-protected website as a static *proof*.

In order to create *proofs* from pages that require authorization, your IT team must add one of the following URLs to your company's Allowlist through which our web capture tool connects:

`AWS clusters in the US`: webcapture.proofhq.com

`GCP clusters in the US`: webcapture.gcp.proofhq.com

`EMEA clusters`: webcapture.proofhq.eu

>[!NOTE]
>
>We recommend interactive *proofing* rather than static *proofing* for internal pages requiring authorization and password-protected websites. For more information, see [Interactive content proofs overview](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## About Processing Static Website Proofs

* Animations, embedded videos, scripts, and interactions cannot be included in static website *proofs*. If you want to *proof* interactive content, see [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Proof pages are generally prepared captured at the rate of about 20 seconds per page. However overall preparation time depends also on the servers where the pages are hosted. The tool waits 60 seconds for each submitted URL to load. If this waiting time is exceeded, the *proof* fails.
* For combined *proofs*, if any of the URLs is not responding to the capture tool, the *proof* fails.

* *Workfront Proof* captures web pages up to 195&nbsp;inches long after rasterizing. If the web page is longer than this,&nbsp;the *proof* fails.

* Text extraction is available&nbsp;on all the text elements, but text placed as images is not extracted.
* Text hyperlinks are clickable on the *proofs*,&nbsp;and the&nbsp;linked pages open in the new browser tabs.
* Hyperlinks on the images are&nbsp;not be clickable if the&nbsp;style="display:block" elements are used inside the <a> tags.&nbsp;We recommend adjusting these parts of the page design.
* For best results we recommend to creating the pages using the best coding practices and acknowledged standards.

