---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Troubleshoot proof creation failures
description: The proof creation process includes both importing and proof generation. Occasionally when you are creating a proof, a file might fail to import, or the proof might fail to generate after the file is imported.
---

# Troubleshoot proof creation failures

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

The proof creation process includes both importing and proof generation. Occasionally when you are creating a proof, a file might fail to import, or the proof might fail to generate after the file is imported.

>[!NOTE]
>
>&nbsp;If the document you are attempting to proof does not match any of the criteria listed in this section, please contact Adobe Workfront&nbsp;Support for further investigation.

## Reasons for import failure

* You have created a combined proof containing over 50 files.

## Reasons for proof generation failure

* The file type is not supported.  
  For a list of supported file types, see [Supported proofing file types and size limits overview](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* The file structure is a non-standard structure for the file type.
* The file is protected by a password or has content copying disabled.

  Unlike other types of files, PDF files can be generated into proofs if your security setting for content copying is set to Allowed on the PDF.

* The page length or page count exceeds the limit.

  The maximum allowed page length is 195 inches after rasterizing; the maximum allowed page count is 1,000 pages for a single proof.

* The file is damaged or corrupted.
* The workflow deadline on a new proof version is in the past.

  This occurs when you are creating a new proof version using a quick proof method and **Automatically generate proofs when uploading documents** is selected. The new proof version attempts to take the workflow deadlines from the previously generated proof. Proof generation fails if these deadline are in the past. To remedy this, you can set the workflow deadlines on the previous version in the future, or generate a new proof version. If you generate a new version, use&nbsp;**More > New Version > Proof** and select **Workflow deadlines in the future**.

* When proofing PDF files, reasons for proof generation failure include:

   * Fonts and images are&nbsp;linked from outside sources (such as from your local file system)

     Fonts and images must be embedded in the PDF file in order to display on another computer&nbsp;or within Workfront Proof.
   
   * Your PDF file contains empty layers or transparent or overlapping fields.

     If you're not able to determine which layer or object causes this, export the design/document as an optimized PDF (this removes all the unwanted elements).

