---
product-area: documents
navigation-topic: proofing-overview
title: Interactive content proofs overview
description: Interactive content provides multiple methods of engaging viewers. Agencies can measure the success of their campaigns using analytics gathered from responses to this content.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
---
# Interactive content proofs overview

<!-- Audited: 01/2024 -->

Interactive content provides multiple methods of engaging viewers. Agencies can measure the success of their campaigns using analytics gathered from responses to this content.

Examples of interactive content include:

* Websites
* Embedded or streaming videos
* Interactive banners
* HTML5 animations
* Microsites
* Interactive emails

## About creating proofs for interactive content

You can create a proof for interactive content in one of the following ways:

* Create a proof from a ZIP file containing the interactive content.

  Adobe Workfront unpacks the content from the ZIP file and stores it on a Workfront server. Because it is stored this way, you can rely on the content staying the same throughout the proof review cycle.

* Specify the URL for the content.

  This is the simplest way to create a proof for interactive content. This is also the only way you can review your content interactively, as users experience it on the internet.

  With this approach, an external server unknown to Workfront stores and hosts the content.

  We recommend this method for a large websites because it is difficult to gather all of the files that make up a large website. However, because the proof's content is stored externally, Workfront cannot protect it from changes made by the developers working on it, so you might not be able to rely on the content staying the same throughout the proof review cycle.

## About preparing interactive content in a ZIP file for proofing

When you bundle interactive content in a ZIP file for proofing, make sure that it includes the following specifications:

* All assets, such as CSS, JavaScript, videos, sounds, and images should be included in the bundle file.
* Interactive content should include the main file (index.html, index.htm). If this&nbsp;file is not placed in the root location, the tool automatically searches the folder to find it.&nbsp;The main file does not need to be named&nbsp;index.html/index.htm, however, there can be only one .html/.htm file placed in the main location.
* The file must contain at least one static file webpage.
* The maximum bundle size is 500 MB.
* In the case of .zip files created in iOS, the tool automatically identifies the folder where the content is located.
* Interactive projects are supported only as .zip archives. Standard .zip file submissions will fail.
* The website must be secure (HTTPS).

  This is not a requirement when using the Desktop Proofing Viewer.

  For more information, see [Understand the Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* The website must be allowed to be viewed in an iframe.

  This is not a requirement when using the Desktop Proofing Viewer.

  For more information, see [Understand the Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## About creating an interactive proof

After you prepare your ZIP bundle file, create an interactive proof.

For more information, see [Create a proof for interactive content in a ZIP file](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).

Or, if you are using Workfront Proof, see the section [Generate a proof for interactive content](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) in the article [Generate Proofs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## About reviewing interactive proofs

We recommend that you use the standalone Desktop Proofing Viewer as the default viewer for interactive proofs.&nbsp;However, if your organization's policies do not allow the use of the Desktop Proofing Viewer app, your Workfront administrator can configure your system so that you can review interactive content, bundled in a ZIP archive file, in the Web Proofing Viewer. For comparative information about the Desktop Proofing Viewer and the Web Proofing Viewer, see [Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
