---
filename: view-proof-flash-shared-object
content-type: tips-tricks-troubleshooting
product: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problems With Viewing Proofs - Flash Shared Objects Explained
description: Note: The information in this article refers to functionality that is currently deprecated and will be removed from Workfront in 2018. We recommend that you use the new Web Proofing Viewer (as described in Reviewing Proofs in the Web Proofing Viewer) or the Desktop Proofing Viewer (as described in Reviewing Proofs in the Desktop Proofing Viewer).
---

# Problems With Viewing Proofs - Flash Shared Objects Explained

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

>[!NOTE]
>
>The information in this article refers to functionality that is currently deprecated and will be removed from Workfront in 2018. We recommend that you use the new Web Proofing Viewer (as described in [Reviewing Proofs in the Web Proofing Viewer](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer)) or the Desktop Proofing Viewer (as described in [Reviewing Proofs in the Desktop Proofing Viewer](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)).

## Flash Shared Objects

A local sared object, sometimes called a "Flash cookie," is a data file that can be created on your computer by the sites you visit. Shared objects are most often used to enhance your web-browsing experience. A Flash cookie is a message used in Adobe Flash that is sent from a Web server to a Web browser and is then stored as a data file in the browser.

Since the Workfront Proof Viewer is based on Flash, it would be worth to check what storage is allowed for Flash applications on your computer.

## Flash Shared Objects - known issues

&nbsp;If the Flash storage is set to 0 KB or has another setting that blocks Flash applications from saving the data locally, it may cause some known issues in the Workfront Proof Viewer:

* The 'Getting started' tour pop-up keeps appearing although the option to not show it again was chosen
* Workfront Proof Viewer performance slows down due to to the increasing number of comments added to the proofs
* Proofs are not loading and you get the 'grey screen' instead of an actual image

## Allowing Flash Shared Objects

Make sure that storing Flash Shared Objects is allowed on the computer and that the storage limit is not 0.

To check if the Shared Objects are allowed:

1. Right click in the Workfront Proof Viewer.
1. Select **Global Settings** from the context menu.
1. Go to the **Storage** tab.
1. Make sure that **Allow sites to save information on this computer** is selected (1).
1. ![2017-06-09_1929.png](assets/2017-06-09-1929-350x267.png)

## Increasing Flash storage

By default Flash applications may store up to 100 KB of data on the user's drive, but this can be easily modified by the users. The solution for the many Flash related issues is to increase internal Flash storage. This can be done directly from the Proof Viewer:

1. Open a proof.
1. Open the right-click menu on the proof.
1. Click **Settings** to open the Flash settings pop-up.
1. Go to the **Local** storage tab.
1. Increase the storage up to e.g. 100 KB (1).
1. Close the settings pop-up and re-open the proof . &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;

![2017-06-09_1926.png](assets/2017-06-09-1926-350x274.png)

