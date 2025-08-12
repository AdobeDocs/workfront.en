---
product-area: documents
navigation-topic: proofing-overview
title: Review interactive content in the Web proofing viewer extension
description: The Adobe Workfront review tool is a browser extension that allows you to proof interactive content in a ZIP file or with a URL.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
---
# Review interactive content with the Adobe Workfront review tool


>[!IMPORTANT]
>
> We recommend using the desktop proofing viewer for interactive content that is hosted on a website that requires SSO authentication or prevents opening their site in iFrames, such as Figma.

The Adobe Workfront review tool is a web-based browser extension that allows you to markup interactive content in a ZIP file or with a URL. The Adobe Workfront review tool is available in the following browsers:

* Firefox
* Chrome
* Edge
* Safari

This extension is required to review content in GenStudio for Performance Marketing and Creative Cloud Express. Assets will automatically open in the web viewer. You do not need to update any account settings.



## Install the extension

### Prerequisites

* You must remove the Legacy Web Viewer extension to use the Adobe Workfront Review tool.

### Install the extension

Reviewers and approvers must install the Adobe Workfront review tool. in one of the following browsers:

* [Firefox extension](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome extension](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml) 

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen) 


For interactive proofs to open in the Adobe Workfront review tool automatically, a Workfront Administrator must update Proofing settings in workfront as described in the sections below.

## Update Workfront proofing defaults

To use the Workfront review tool as your default viewer for interactive content, you must update proofing defaults in Workfront. 

>[!IMPORTANT]
>
>We recommend using the Desktop Proofing Viewer if the content you need to review is on a website that
>
>* Requires SSO authentication
>* Prevents opening their site in iFrames, such as Figma

### Make the Adobe Workfront review tool the default viewer for URL and ZIP proofs

To use the web review tool for URL and ZIP proofs, a Workfront Administrator must adjust the default setting for interactive proofs. 

1. In Workfront's Main Menu, click **Proofing**.
1. Click **Account settings**, then click the **Settings** tab.
1. In the **Proof Defaults** section, find **Desktop Proofing Viewer for Interactive proofing** and click **Setup**.
1. In the drop-down menu, choose **Disabled**. Interactive proofs created from a URL or ZIP file now automatically open in the Adobe Workfront Review tool, which is a web-based browser.
1. Click **Save**.

>[!NOTE]
>
>This change applies to all interactive proofs in your Workfront instance. We recommend testing the new experience in your Preview environment before enabling it in Production. You can easily switch back to the Desktop Viewer by changing the **Desktop Proofing Viewer for Interactive proofing** account setting back to **Enabled for all interactive proofs**.

### Make the Adobe Workfront review tool the default viewer for ZIP proofs only

To use the web review tool for ZIP proofs only, a Workfront Administrator must adjust the default setting for interactive proofs. 

1. In Workfront's Main Menu, click **Proofing**.
1. Click **Account settings**, then click the **Settings** tab.
1. In the **Proof Defaults** section, find **Desktop Proofing Viewer for Interactive proofing** and click **Setup**.
1. In the drop-down menu, choose **Enabled only for interactive proofs created from a URL**. Interactive proofs created from a ZIP file now automatically open in the Adobe Workfront Review tool, which is a web-based browser. Interactive proofs created from a URL still still open in the Desktop Proofing Viewer.
1. Click **Save**.

>[!NOTE]
>
>This change applies to all ZIP proofs in your Workfront instance. We recommend testing the new experience in your Preview environment before enabling it in Production. You can easily switch back to the Desktop Viewer by changing the **Desktop Proofing Viewer for Interactive proofing** account setting back to **Enabled for all interactive proofs**.

