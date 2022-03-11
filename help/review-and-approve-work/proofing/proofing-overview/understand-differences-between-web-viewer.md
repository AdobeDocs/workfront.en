---
filename: understand-differences-between-web-viewer
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview
description: Adobe Workfront provides two different proofing viewers:
---

# Differences between the `Web Proofing Viewer` and the `Desktop Proofing Viewer` overview

`Adobe Workfront` provides two different `proofing` viewers:

<ul> 
 <li><span class="bold"><span>Web Proofing Viewer</span>:</span>&nbsp;Designed primarily for <span>proofing</span> static and video files. Runs in Google Chrome, Firefox, or Safari. </li> 
 <li><span class="bold"><span>Desktop Proofing Viewer</span>:</span> Designed for <span>proofing</span> interactive files as well as video and static files.&nbsp;Runs as&nbsp;a standalone application on your workstation. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md" class="MCXref xref">Understand the Desktop Proofing Viewer</a></li> <note type="note">
  If your organization cannot use the 
  <span>Desktop Proofing Viewer</span> app for security reasons, your 
  <span>Workfront administrator</span> can configure your system so that you can review interactive content, bundled in a ZIP archive file, in the 
  <span>Web Proofing Viewer</span>. For more information, see&nbsp;
  <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md" class="MCXref xref">Set up interactive content proofing in Web Proofing Viewer</a>.
 </note> 
</ul>

The following list can help you understand what Proofing Viewer you can use to proof certain types of content:

* `Interactive web content - URL`: If you create a proof for web content using a URL and you want to proof the content interactively, you must use the `Desktop Proofing Viewer`.

* `Interactive web content - ZIP file`: If you create a proof for web content using a ZIP file, you can use either the `Web Proofing Viewer` (with some limitations) or the `Desktop Proofing Viewer`. For information about the limitations involved in using the `Web Proofing Viewer` for interactive content, see [Set up interactive content proofing in Web Proofing Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

* `Static and video content`: If you create a proof containing static content, you can use either the `Web Proofing Viewer` or the `Desktop Proofing Viewer`.

## Static `proofs`

| `Feature`  | ` `Web Proofing Viewer``  | ` `Desktop Proofing Viewer``  |
|---|---|---|
| Open static `proofs` |✓ |✓&#42; |
| Single, magazine, and continuous views |✓ |✓&#42; |
| Panning |✓ |✓&#42; |
| Zooming |✓ | ✓&#42; |
| Rotate |✓ | ✓&#42; |
| Measurement tool |✓ (set a custom-sized area) | ✓&#42; |
| Thumbnail view |✓ | ✓&#42; |
| Static `proof` navigator |✓ | ✓&#42; |
| Document search |✓ | ✓&#42; |
| Post comment on multiple pages |✓&nbsp;(available on all views) | ✓&#42; (available on all views) |
| Advanced static `proof` shortcuts |✓&nbsp;(for more information, see [Keyboard shortcuts in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |✓&#42;(for more information, see [Keyboard shortcuts in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |

&#42; This functionality works only if your `Workfront administrator` has configured the `Desktop Proofing Viewer` as the default viewer for all `proofs`.

## Video `proofs`

| `Feature`  | ` `Web Proofing Viewer``  | ` `Desktop Proofing Viewer``  |
|---|---|---|
| Open video `proofs` |✓ |✓&#42; |
| Buffering |✓ |✓&#42; |
| Review using time |✓ |✓&#42; |
| Review using frames or timecode |✓ |✓&#42; |
| Review faster or slower |✓ |✓&#42; |
| Volume regulation |✓ | ✓&#42;&nbsp; |
| full-screen mode |✓ | ✓&#42;&nbsp; |
| Range comments |✓ | ✓&#42;&nbsp; |
| Loop video `proofs` (videos finish and start automatically) |✓ | ✓&#42;&nbsp; |
| Advanced video shortcuts |✓&nbsp;(for more information, see [Keyboard shortcuts in the proofing viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;&nbsp; |

&#42; This functionality works only if the `Desktop Proofing Viewer` is configured as the default viewer for all `proofs`.

##

## Interactive `proofs`

| `Feature`  | ` `Web Proofing Viewer``  | ` `Desktop Proofing Viewer``  |
|---|---|---|
| Open interactive `proofs` created from content bundled in a ZIP file |✓ |✓ (recommended) |
| Open an interactive `proof` created from a URL |Not supported |✓ |
| View interactive `proofs` (created from content bundled in a ZIP file) in various screen sizes |✓ |✓ |
| View interactive `proofs` (created from content bundled in a ZIP file) for various devices |Not supported |✓ |
| Review unsecured (HTTP) sites |Not supported |✓ |
| Review iFrame-protected sites (sites that are protected from being viewed within an iFrame) |Not supported |✓ |

## Comments

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Feature</th> 
   <th><span>Web Proofing Viewer</span> </th> 
   <th><span>Desktop Proofing Viewer</span> </th> 
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
   <td>✓ Static <span>proofs</span> only</td> 
   <td>✓ Static <span>proofs</span> only</td> 
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
   <td>✓ <!--
     ?check this
    --></td> 
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

| Feature | `Web Proofing Viewer`  | `Desktop Proofing Viewer`  |
|---|---|---|
| Make decisions |✓ |✓ |
| Customize decisions |✓ |✓ |

## Compare `proofs`

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Feature</th> 
   <th><span>Web Proofing Viewer</span> </th> 
   <th><span>Desktop Proofing Viewer</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Compare different versions of <span>proofs</span></td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>Compare separate <span>proofs</span></td> 
   <td>&nbsp;✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## `Proof` operations

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Feature</th> 
   <th><span>Web Proofing Viewer</span> </th> 
   <th><span>Desktop Proofing Viewer</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Change the <span>proof</span> version&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;✓ </td> 
  </tr> 
  <tr> 
   <td>Create a new version</td> 
   <td> <p>Available only in <span>Workfront Proof</span>(planned for the future when <span>proofing</span> within <span>Workfront</span>)<br></p> </td> 
   <td>Available only in <span>Workfront Proof</span>(planned for the future when <span>proofing</span> within <span>Workfront</span>)</td> 
  </tr> 
  <tr> 
   <td>Review <span>proof</span> details&nbsp;</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Review <span>proof</span> workflows</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Edit workflow stages</td> 
   <td>Not supported</td> 
   <td>Not supported</td> 
  </tr> 
  <tr> 
   <td>Share <span>proofs</span></td> 
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
   <td>Lock and unlock <span>proofs</span> and stages</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Print <span>proof</span> summary</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Delete <span>proofs</span></td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Manage <span>proofs</span> from the same folder</td> 
   <td><font size="2">Available only in <span>Workfront Proof</span></font> </td> 
   <td><font size="2">Available only in <span>Workfront Proof</span></font> </td> 
  </tr> 
  <tr> 
   <td>Branding (custom logos)</td> 
   <td>✓</td> 
   <td>&nbsp;✓<br>(<span>Workfront</span> Logo on launch page) </td> 
  </tr> 
  <tr> 
   <td>Custom links&nbsp;(<span>Workfront Proof</span> only)</td> 
   <td>Not supported</td> 
   <td> Not supported&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Basecamp integrations&nbsp;(<span>Workfront Proof</span> only)&nbsp;</td> 
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

| `Feature`  | ` `Web Proofing Viewer``  | ` `Desktop Proofing Viewer``  |
|---|---|---|
| Embedded code |Planned for future for static and native video `proofs` |Not supported&nbsp; |

## Translations

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Feature</span>&nbsp;</th> 
   <th><span class="bold"><span>Web Proofing Viewer</span></span> </th> 
   <th><span class="bold"><span>Desktop Proofing Viewer</span></span> </th> 
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

