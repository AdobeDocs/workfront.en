---
product-previous: workfront-library
product-area: documents
navigation-topic: metadata
title: Set up taxonomy metadata for Workfront Library
description: As a Workfront Library administrator, you can set up your organization's taxonomy to gather the information your users search for and to track content. For more information about the different types of taxonomy you can collect, see Overview of taxonomy metadata in Workfront Library.
feature: Workfront Library, Digital Content and Documents
exl-id: 7f9249eb-af41-41d3-9498-1580e70aa03f
---
# Set up taxonomy metadata for Workfront Library

As a Workfront Library administrator, you can set up your organization's taxonomy to gather the information your users search for and to track content. For more information about the different types of taxonomy you can collect, see [Overview of taxonomy metadata in Workfront Library](../../../workfront-library/administration-and-setup/metadata/taxonomy-metadata-overview.md).

1. In Workfront, click the **Main Menu** icon ![](assets/main-menu-icon.png), then select **Library** to open Workfront Library in a new browser tab.
1. In the upper-left corner of Workfront Library, click the **Menu** icon ![](assets/library-menu-icon.png).
1. In the left panel, click **Setup** > **Taxonomy**.
1. Click **Add Field**, then select the type of field you want to add to your taxonomy.

   You can choose from the following field types:

   * Custom
   * Attribute
   * EXIF
   * XMP

## Custom

Use custom taxonomy to gather information tailored to your organization, such as campaign, department, or location.

1. In the **Field Type** drop-down list, select the type of field you want to configure.

   You can choose from the following field types:

   | Date |Allows users to manually enter a date or select a date from a date picker |
   |---|---|
   | Multi-select |Lists multiple options in a picklist from which users can choose several options |
   | Single-select |Lists multiple options in a picklist from which users can choose one option |
   | Text field |Allows users to freely enter text |

   {style="table-layout:auto"}


   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   up to X characters of [FOLLOW&nbsp;UP&nbsp;WITH&nbsp;CLINT]
   </MadCap:conditionalText>
   -->

1. (Conditional) If you are configuring a multi- or single-select custom field, enter the **Value** and press **Enter**. You can list up to 100 different values in the picklist with names. These names can be up to 50 characters.
1. (Optional) To require users to complete this field when entering metadata, enable&nbsp;**Required Field**.
1. Click **Save**.

   The custom field is added to the taxonomy.

## Attribute

The metadata for attribute fields is derived from the device or application used to create the content.

1. In the **Name**&nbsp;drop-down menu, choose the attribute you want to add to the taxonomy.

   You can choose from the following attributes:

   * File Extension
   * Size
   * Modified Date
   * Created Date

1. Click **Save**.

### EXIF

Although some asset files contain large amounts of EXIF metadata, you can configure your taxonomy to collect only the EXIF metadata you need.&nbsp;If at a later date you decide to collect additional EXIF metadata, simply add the appropriate EXIF field to your taxonomy. Workfront Library then updates the EXIF metadata for all content embedded with the appropriate EXIF metadata.

To learn about the EXIF metadata that Workfront Library supports, see [Overview of taxonomy field types](../../../workfront-library/administration-and-setup/metadata/taxonomy-field-types-overview.md).

1. In the **EXIF Field** box, begin typing the EXIF tag you want to capture and select the tag when it displays in the drop-down list.
1. In the **Custom Label** box, enter a unique name for the field.  
   The field name becomes the label that displays in the Details panel for content.
1. Click **Save**.

### XMP

You can configure XMP taxonomy fields to embed specific types of metadata to content when it is uploaded to Workfront Library.

To learn about the XMP metadata that Workfront Library supports, see [Overview of taxonomy field types](../../../workfront-library/administration-and-setup/metadata/taxonomy-field-types-overview.md).

1. In the **XMP Field**&nbsp;box, begin typing the XMP tag you want to capture in the taxonomy and select the tag when it displays in the drop-down list.

   <!--
   <note type="note">
   If your organization has not yet uploaded content to Workfront Library, no options display in the XMP Field drop-down list. After you upload some content files with XMP data, Workfront Library begins to recognize the type of XMP data your organization uses and lists the applicable XMP tags in the XMP Field drop-down list.
   </note>
   -->

1. In the **Custom Label** box, enter a label for the field.

   The field name becomes the label that displays in the Details panel for content. 

1. Click **Save**.
