---
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview
description: Learn the differences between the desktop and web proofing viewers.
author: Courtney
feature: Digital Content and Documents
exl-id: 72ce147b-29c9-4c3b-a03c-2da0758bc178
---
# Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview

Adobe Workfront provides two different proofing viewers:

* **Web Proofing Viewer:**&nbsp;Designed primarily for proofing static and video files. Runs in Google Chrome, Firefox, or Safari. 
* **Desktop Proofing Viewer:** Designed for proofing interactive files as well as video and static files.&nbsp;Runs as&nbsp;a standalone application on your workstation. For more information, see [Understand the Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)

* If your organization cannot use the Desktop Proofing Viewer app for security reasons, your Workfront administrator can configure your system so that you can review interactive content, bundled in a ZIP archive file, in the Web Proofing Viewer. For more information, see&nbsp; [Set up interactive content proofing in Web Proofing Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

The following list can help you understand what Proofing Viewer you can use to proof certain types of content:

* **Interactive web content - URL**: If you create a proof for web content using a URL and you want to proof the content interactively, you must use the Desktop Proofing Viewer.
* **Interactive web content - ZIP file**: If you create a proof for web content using a ZIP file, you can use either the Web Proofing Viewer (with some limitations) or the Desktop Proofing Viewer. For information about the limitations involved in using the Web Proofing Viewer for interactive content, see [Set up interactive content proofing in Web Proofing Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

* **Static and video content**: If you create a proof containing static content, you can use either the Web Proofing Viewer or the Desktop Proofing Viewer.

## Static proofs

| **Feature** |**Web Proofing Viewer** |**Desktop Proofing Viewer** |
|---|---|---|
| Open static proofs |✓ |✓&#42; |
| Single, magazine, and continuous views |✓ |✓&#42; |
| Panning |✓ |✓&#42; |
| Zooming |✓ | ✓&#42; |
| Rotate |✓ | ✓&#42; |
| Measurement tool |✓ (set a custom-sized area) | ✓&#42; |
| Thumbnail view |✓ | ✓&#42; |
| Static proof navigator |✓ | ✓&#42; |
| Document search |✓ | ✓&#42; |
| Post comment on multiple pages |✓&nbsp;(available on all views) | ✓&#42; (available on all views) |
| Advanced static proof shortcuts |✓&nbsp;(for more information, see [Keyboard shortcuts in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |✓&#42;(for more information, see [Keyboard shortcuts in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |

{style="table-layout:auto"}

&#42; This functionality works only if your Workfront administrator has configured the Desktop Proofing Viewer as the default viewer for all proofs.

## Video proofs

| **Feature**&nbsp; |**Web Proofing Viewer** |**Desktop Proofing Viewer** |
|---|---|---|
| Open video proofs |✓ |✓&#42; |
| Buffering |✓ |✓&#42; |
| Review using time |✓ |✓&#42; |
| Review using frames or timecode |✓ |✓&#42; |
| Review faster or slower |✓ |✓&#42; |
| Volume regulation |✓ | ✓&#42;&nbsp; |
| full-screen mode |✓ | ✓&#42;&nbsp; |
| Range comments |✓ | ✓&#42;&nbsp; |
| Loop video proofs (videos finish and start automatically) |✓ | ✓&#42;&nbsp; |
| Advanced video shortcuts |✓&nbsp;(for more information, see [Keyboard shortcuts in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;&nbsp; |

{style="table-layout:auto"}

&#42; This functionality works only if the Desktop Proofing Viewer is configured as the default viewer for all proofs.

## Interactive proofs

| **Feature**&nbsp; |**Web Proofing Viewer** |**Desktop Proofing Viewer** |
|---|---|---|
| Open interactive proofs created from content bundled in a ZIP file |✓ |✓ (recommended) |
| Open an interactive proof created from a URL |Not supported |✓ |
| View interactive proofs (created from content bundled in a ZIP file) in various screen sizes |✓ |✓ |
| View interactive proofs (created from content bundled in a ZIP file) for various devices |Not supported |✓ |
| Review unsecured (HTTP) sites |Not supported |✓ |
| Review iFrame-protected sites (sites that are protected from being viewed within an iFrame) |Not supported |✓ |

{style="table-layout:auto"}

## Comments

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Feature</th> 
   <th>Web Proofing Viewer </th> 
   <th>Desktop Proofing Viewer </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Add, delete, and edit comments</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Add and delete replies</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Rectangle, arrow, line, freehand, and highlight markup tools</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Polyline tool</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Crop mask markup tools</p> </td> 
   <td>Not supported</td> 
   <td>Not supported</td> 
  </tr> 
  <tr> 
   <td> <p>Text selection markup tool</p> </td> 
   <td>✓ Static proofs only</td> 
   <td>✓ Static proofs only</td> 
  </tr> 
  <tr> 
   <td> <p>Change markup color</p> </td> 
   <td>✓&nbsp;(32 colors available)&nbsp;</td> 
   <td>✓&nbsp;(32 colors available)&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Change markup opacity</p> </td> 
   <td>✓</td> 
   <td> ✓&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Change markup thickness</p> </td> 
   <td>✓</td> 
   <td> ✓&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Cut, copy, and paste markups</p> </td> 
   <td> Not supported</td> 
   <td> Not supported</td> 
  </tr> 
  <tr> 
   <td> <p>Undo and redo last operation</p> </td> 
   <td>✓</td> 
   <td> ✓&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Duplicate markups</p> </td> 
   <td> Not supported</td> 
   <td> Not supported</td> 
  </tr> 
  <tr> 
   <td>Set actions to comments</td> 
   <td>✓&nbsp;(Actions are visible on comments immediately after the action is set)</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Set markup color as default</p> </td> 
   <td>✓</td> 
   <td>&nbsp;✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Resolve comments</p> </td> 
   <td>✓</td> 
   <td>&nbsp;✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Lock comments</p> </td> 
   <td>Not supported</td> 
   <td> Not supported</td> 
  </tr> 
  <tr> 
   <td> <p>Tag users</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Resume comments</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>View the comment list in a compact view</p> </td> 
   <td>✓</td> 
   <td> ✓&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>View the comment list in a standard, full, or single view</p> </td> 
   <td>Planned for the future</td> 
   <td>Planned for the future</td> 
  </tr> 
  <tr> 
   <td> <p>Search comments</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filter comments by user</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filter comments and replies by user</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sort comments</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Comment auto-updates</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Decisions

| Feature |Web Proofing Viewer  |Desktop Proofing Viewer  |
|---|---|---|
| Make decisions |✓ |✓ |
| Customize decisions |✓ |✓ |

{style="table-layout:auto"}

## Compare proofs

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Feature</th> 
   <th>Web Proofing Viewer </th> 
   <th>Desktop Proofing Viewer </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Compare different versions of proofs</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>Compare separate proofs</td> 
   <td>&nbsp;✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## Proof operations

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Feature</th> 
   <th>Web Proofing Viewer </th> 
   <th>Desktop Proofing Viewer </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Change the proof version&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;✓ </td> 
  </tr> 
  <tr> 
   <td>Create a new version</td> 
   <td> <p>Available only in Workfront Proof(planned for the future when proofing within Workfront)<br></p> </td> 
   <td>Available only in Workfront Proof(planned for the future when proofing within Workfront)</td> 
  </tr> 
  <tr> 
   <td>Review proof details&nbsp;</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Review proof workflows</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Edit workflow stages</td> 
   <td>Not supported</td> 
   <td>Not supported</td> 
  </tr> 
  <tr> 
   <td>Share proofs</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Get team URL</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Change email notifications</td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Download original file</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Lock and unlock proofs and stages</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Print proof summary</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Delete proofs</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Manage proofs from the same folder</td> 
   <td><strong>Available only in Workfront Proof</strong> </td> 
   <td><strong>Available only in Workfront Proof</strong> </td> 
  </tr> 
  <tr> 
   <td>Branding (custom logos)</td> 
   <td>✓</td> 
   <td>&nbsp;✓<br>(Workfront Logo on launch page) </td> 
  </tr> 
  <tr> 
   <td>Custom links&nbsp;(Workfront Proof only)</td> 
   <td>Not supported</td> 
   <td> Not supported&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Basecamp integrations&nbsp;(Workfront Proof only)&nbsp;</td> 
   <td>Planned for future</td> 
   <td>Planned for future</td> 
  </tr> 
  <tr> 
   <td>Presence indicator&nbsp;</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Proof auto-updates (permission changes and new versions)</td> 
   <td>✓</td> 
   <td>✓&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

## Miniviewer

| **Feature**&nbsp; |**Web Proofing Viewer**&nbsp; |**Desktop Proofing Viewer** |
|---|---|---|
| Embedded code |Planned for future for static and native video proofs |Not supported&nbsp; |

{style="table-layout:auto"}

## Translations

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Feature</strong>&nbsp;</th> 
   <th><strong>Web Proofing Viewer</strong> </th> 
   <th><strong>Desktop Proofing Viewer</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Support languages other than English</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
 </tbody> 
</table>
