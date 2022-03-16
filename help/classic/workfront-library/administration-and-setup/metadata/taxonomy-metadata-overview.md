---
filename: taxonomy-metadata-overview
content-type: overview
product: workfront-library
product-area: documents
navigation-topic: metadata
title: Overview of taxonomy metadata in Workfront Library
description: Taxonomy is a type of metadata used to describe and categorize the factual attributes of content uploaded to Workfront Library. For information about metadata, see Overview of metadata in Workfront Library.
---

# Overview of taxonomy metadata in Workfront Library

Taxonomy is a type of metadata used to describe and categorize the factual attributes of content uploaded to Workfront Library. For information about metadata, see [Overview of metadata in Workfront Library](../../../workfront-library/administration-and-setup/metadata/metadata-overview.md).

Users apply taxonomy when they upload an asset to Workfront Library. Users can also add or edit taxonomy metadata to shared assets to which they have Manage permissions.

Some taxonomy, such as EXIF and XMP, is embedded in the content file and can be automatically added to the content's metadata when the file is uploaded. Other taxonomy must be provided by the user during the content upload process.

As a Workfront Library administrator, you configure your organization's taxonomy by selecting the types of information users are prompted for when they upload content. For example, you can add fields to the taxonomy that require users to enter the content creator's name or the location of a photo.

Before designing your organization's taxonomy, determine the types of information your users are most likely to filter for when looking for content. You can then set up taxonomy fields that prompt users for information that support more accurate search results.&nbsp;

Some taxonomy fields can also be used as faceted filters in the Filter panel. For information on filtering, see [Filter content displayed in Workfront Library](../../../workfront-library/content-management/basics/filter-content-displayed.md).

You can configure the following types of fields in your taxonomy:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Custom data</td> 
   <td>Fields that allow you to collect information that is specific to your organization. The date, single-select, and multi-select custom data fields are also faceted filters in the Filter panel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Attribute</td> 
   <td>Pre-configured fields that capture specific attributes of a content file, for example file size and format. All attribute fields are faceted filters in the Filter panel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">EXIF </td> 
   <td>(Exchangeable Image File) Fields that identify characteristics of an image file, such as date and time of creation, copyright information, and camera settings.&nbsp;EXIF metadata is embedded on an image file by the creation device or application, such as a cell phone, word processing application, or digital camera.&nbsp;EXIF fields cannot be faceted filters on the Filter panel. For information on supported EXIF metadata types, see <a href="../../../workfront-library/administration-and-setup/metadata/taxonomy-field-types-overview.md" class="MCXref xref">Overview of taxonomy field types</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">XMP</td> 
   <td>(Extensible Metadata Platform) Fields that capture standardized metadata that can be processed and shared by a variety of software applications. XMP metadata is embedded on the content file and remains with the file even when it's downloaded by external users. XMP fields cannot be faceted filters on the Filter panel. For information on supported XMP metadata types, see <a href="../../../workfront-library/administration-and-setup/metadata/taxonomy-field-types-overview.md" class="MCXref xref">Overview of taxonomy field types</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Expiry</td> 
   <td> <p>A field that allows users to specify an expiration date for content they upload. The Expiration Date field is a faceted filter in the Filter panel. For information on adding a expiration field to your taxonomy, see <a href="../../../workfront-library/administration-and-setup/workfront-library-setup/set-up-content-expiration-in-library.md" class="MCXref xref">Set up content expiration in Workfront Library</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

With the exception of attribute fields, you can configure taxonomy fields to be either optional or required. Any attribute fields that you add to your taxonomy are automatically configured as required fields.

The fields you configure in your taxonomy display in the metadata Details panel for the content.

While users process content for uploading to Workfront Library, they can identify the taxonomy for the content. Before the content is uploaded, users must complete all required taxonomy fields. For information on filling in metadata during upload, see [Upload content to Workfront Library](../../../workfront-library/content-management/upload-new-content.md).

Users with Manage permissions to an item can change and add to its metadata. For content with multiple versions, only the metadata of the active (most current) version can be modified. After a new version of content is uploaded to Workfront Library, the metadata for the older version is locked and cannot be changed. For more information on versioning content, see [Overview of content versioning in Workfront Library](../../../workfront-library/content-management/content-versioning/content-versioning-overview.md).

Because portal users might not need to view all the taxonomy you collect on your organization's assets, you can select which taxonomy fields display on content shared with a portal. For information about specifying taxonomy fields for portal content, see [Set up a portal in Workfront Library](../../../workfront-library/administration-and-setup/workfront-library-setup/set-up-a-portal-in-library.md).

For more information on ways to manage taxonomy, see the following articles:

* [Set up taxonomy metadata for Workfront Library](../../../workfront-library/administration-and-setup/metadata/set-up-taxonomy-metadata.md) 
* [Determine the display order of taxonomy fields in Workfront Library](../../../workfront-library/administration-and-setup/metadata/determine-display-order-of-taxonomy-fields.md) 
* [Edit a taxonomy metadata field in Workfront Library](../../../workfront-library/administration-and-setup/metadata/edit-the-taxonomy.md) 
* [Delete a taxonomy field in Workfront Library](../../../workfront-library/administration-and-setup/metadata/delete-a-taxonomy-field-in-workfront-library.md)

