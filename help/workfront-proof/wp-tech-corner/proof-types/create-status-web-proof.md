---
filename: create-status-web-proof
product: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Create a Static Website Proof using Workfront Proof
description: You can create static proofs from your web pages. In addition, you can simulate various devices by defining screen resolution of the captures.
---

# Create a Static Website Proof using Workfront Proof

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

You can create static proofs from your web pages. In addition, you can simulate various devices by defining screen resolution of the captures.

## Creating a Static Website Proof

1. Open the New proof page, as described in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Paste or type your URL in the `www.shareyourlink.com`&nbsp;box.
1. You can repeat this step to add multiple URLs.
1. Just below this box, click the resolution (the default is 1366x768), then select any resolutions you want in the `Screensot resolution` box.  
   Select a smaller resolution if you want to proof designs for mobile devices. Generally, designs load as per screen/browser window resolution.

1. Click `Look for subpages` if you&nbsp;want to&nbsp;include connected pages that are in the same domain/subdomain&nbsp;as the&nbsp;entered&nbsp;URL.  
   Workfront Proof scans the connected pages and lists them below the `Look for subpages` option. You can select the pages you want to include.  

1. With the Combine proofs feature you can submit all the web pages as a single multi-page proof.
1. Click `Done`, then finish configuring your proof as explained in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## About Password-Protected Pages and Pages Requiring Authorization

Workfront Proof cannot capture a password-protected website as a static proof.

In order to create proofs from pages that require authorization, your IT team must add one of the following URLs to your company's Allowlist through which our web capture tool connects:

`AWS clusters in the US`: webcapture.proofhq.com

`GCP clusters in the US`: webcapture.gcp.proofhq.com

`EMEA clusters`: webcapture.proofhq.eu

>[!NOTE]
>
>We recommend interactive proofing rather than static proofing for internal pages requiring authorization and password-protected websites. For more information, see [Interactive content proofs overview](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## About Processing Static Website Proofs

* Animations, embedded videos, scripts, and interactions cannot be included in static website proofs. If you want to proof interactive content, see [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Proof pages are generally prepared captured at the rate of about 20 seconds per page. However overall preparation time depends also on the servers where the pages are hosted. The tool waits 60 seconds for each submitted URL to load. If this waiting time is exceeded, the proof fails.
* For combined proofs, if any of the URLs is not responding to the capture tool, the proof fails.
* Workfront Proof captures web pages up to 195&nbsp;inches long after rasterizing. If the web page is longer than this,&nbsp;the proof fails.
* Text extraction is available&nbsp;on all the text elements, but text placed as images is not extracted.
* Text hyperlinks are clickable on the proofs,&nbsp;and the&nbsp;linked pages open in the new browser tabs.
* Hyperlinks on the images are&nbsp;not be clickable if the&nbsp;style="display:block" elements are used inside the <a> tags.&nbsp;We recommend adjusting these parts of the page design.
* For best results we recommend to creating the pages using the best coding practices and acknowledged standards.

