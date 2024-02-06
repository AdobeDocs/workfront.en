---
product-area: documents
navigation-topic: proofing-overview
title: Document reprocessing for proofing overview
description: When you submit a document (DOCX, PDF, XLSX, AI) for proofing, Adobe Workfront reprocesses it so that it can display in the proofing viewer without the software application you used to create it.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
---
# Document reprocessing for proofing overview

When you submit a document (DOCX, PDF, XLSX, AI) for proofing, Adobe Workfront reprocesses it so that it can display in the proofing viewer without the software application you used to create it.&nbsp;

Each page of your document appears in the proofing viewer as a thumbnail image. When you click a thumbnail, you can zoom into a bitmap version of that page at 100%, 200%, and 400%. For proofs exceeding 800mm in height or width, the maximum zoom level is 200%.

The colors in your document display in sRGB with color conversion from the latest Adobe library. The proofing viewer supports any International&nbsp;Color Consortium (ICC) profiles embedded in the document.

All font text is extracted in its layer as long as you include the correct file extension when uploading the document to the system. Text included as images or curves does not display.

>[!NOTE]
>
>Workfront currently supports documents containing up to 2000 pages. This includes combined proofs. For more information, see [Create a multi-page proof](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## General tips

* Because PDF files are the most standardized and reliable, we recommend converting documents to this format&nbsp;before uploading them.
* Use the latest possible version of your software to create your original documents.
* If you are not sure which settings to use when saving or exporting your documents in the application where you created them, use the default settings.&nbsp;
* Make sure to embed all the fonts you use in a document inside it. If you use custom fonts, your document will display those fonts only on machines where they are installed. However, because custom fonts are not included in the proof system, it is not able to use custom fonts when generating the file, even when embedded.
* If possible, place all text elements in the top layers of your design. This should ensure that your text is extracted and selectable in the Text annotation tool.
* Place all of your document's images and elements inside it. If you link them from the outside sources, such as another file on your computer, they won't display in the proof you create.
* Create your document&nbsp;using the standards recommended for its type and optimize it before uploading it. This will ensure that the document will open successfully in the proofing viewer, as well as in all other applications and platforms.
* In your design software, try running "preflight" options to see if your document generates any warnings. These options are available in most applications as output preview, printing production, and so on. See your application's documentation for more information.
* Make sure color settings are consistent throughout your document.
* If your document is protected from actions such as from file copying, the proofing extraction tool may not be able to access its content.

## Process times

Normally, processing takes a few seconds per page. However, various factors can prolong this, such as network traffic/bandwidth, local connection speeds, and international connection speeds (for users outside the US). The following may also affect processing time:

* For static documents and images: page count, page dimensions, text volume, image and objects complexity (elements such as multiple vector elements, layers, transparencies).
* For videos: long durations, large dimensions, and codecs used.
* For web captures: web page loading times and page dimensions.

## Process steps

Submitted files go through some or all the following steps:

1. **Submission**. When you upload a document to the system, you do so using the New proof page or using an application programming interface (API).&nbsp;
1. **Queue**. During heavy traffic periods, Workfront may need to queue submissions to keep from overloading the system. Most proofs spend only a few seconds in a queue.&nbsp;
1. **Processing.**&nbsp;The files reach the processing machines as per the content type. We use different tools to process video proofs, web captures, static images and documents. Rich Media containers (ZIP) and Interactive web capture submissions do not require processing.
