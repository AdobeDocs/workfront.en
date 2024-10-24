---
product-area: documents
navigation-topic: proofing-overview
title: Review interactive content in the Web proofing viewer extension
description: The Adobe Workfront review tool is a browser extension that allows you to proof interactive content in a ZIP file or with a URL.
author: Courtney
feature: Digital Content and Documents

---

# Review interactive content with the Adobe Workfront review tool

<span class="preview">The Adobe Workfront Review tool will be available on November 7, 2024. This extension is currently in beta.</span>

The Adobe Workfront review tool is a web-based browser extension that allows you to proof interactive content in a ZIP file or with a URL. The Adobe Workfront review tool is available in the following browsers:

* Firefox
* Chrome
* Edge

For websites that prevent opening their site in iFrames, such as Figma, we recommend using Desktop Proof Viewer.


## Make the Adobe Workfront review tool the default viewer for URL and ZIP proofs

To use the web review tool for URL and ZIP proofs, a Workfront Administrator must adjust the default setting for interactive proofs. 

1. In Workfront's Main Menu, click **Proofing**.
1. Click **Account settings**, then click the **Settings** tab.
1. In the **Proof Defaults** section, find **Desktop Proofing Viewer for Interactive proofing** and click **Setup**.
1. In the drop-down menu, choose **Disabled**. Interactive proofs created from a URL or ZIP file now automatically open in the Adobe Workfront Review tool, which is a web-based browser.
1. Click **Save**.

>[!IMPORTANT]
>
>This change applies to all interactive proofs in your Preview and Production environments. We recommend testing the new experience in your Preview environment before enabling it in Production. You can easily switch back to the Desktop Viewer by changing the account setting back to either **Enabled for all interactive proofs**.

## Make the Adobe Workfront review tool the default viewer for ZIP proofs only

To use the web review tool for ZIP proofs only, a Workfront Administrator must adjust the default setting for interactive proofs. 

1. In Workfront's Main Menu, click **Proofing**.
1. Click **Account settings**, then click the **Settings** tab.
1. In the **Proof Defaults** section, find **Desktop Proofing Viewer for Interactive proofing** and click **Setup**.
1. In the drop-down menu, choose **Enabled only for interactive proofs created from a URL**. Interactive proofs created from a ZIP file now automatically open in the Adobe Workfront Review tool, which is a web-based browser. Interactive proofs created from a URL still still open in the Desktop Proofing Viewer.
1. Click **Save**.

>[!IMPORTANT]
>
>This change applies to all interactive proofs in your Preview and Production environments. We recommend testing the new experience in your Preview environment before enabling it in Production. You can easily switch back to the Desktop Viewer by changing the account setting back to either **Enabled for all interactive proofs**. 

## Install the extension

Reviewers and approvers must install the Adobe Workfront review in one of the following browsers:

* [Firefox extension](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome extension](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml) 

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen) 

Once you install the extension, interactive proofs open in the Adobe Workfront review tool automatically. 

 
The setting to open the Desktop Proofing Viewer for Interactive Proofing must be disabled to use the Workfront review tool. See the [Prerequisites](#prerequisites) section above for information on disabling this setting.
 

 