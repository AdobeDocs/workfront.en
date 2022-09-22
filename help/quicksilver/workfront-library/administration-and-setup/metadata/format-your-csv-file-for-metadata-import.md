---
product-previous: workfront-library
product-area: documents
navigation-topic: metadata
title: Format your CSV file for metadata import in [!DNL Workfront Library]
description: "[!DNL Workfront Library] can consume a CSV file with up to 100,000 rows of data. While a larger file can take longer to import, Workfront recommends importing one file—if possible—because Workfront Library only processes one metadata import at a time. If you need to import multiple files, you must wait until the first file has finished before you can start another import."
feature: Workfront Library, Digital Content and Documents
exl-id: 8fd74886-8539-40f3-8e0e-f1ad016c6d37
---
# Format your CSV file for metadata import in [!DNL Workfront Library]

[!DNL Workfront Library] can consume a [!UICONTROL CSV] file with up to 100,000 rows of data. While a larger file can take longer to import, [!DNL Workfront] recommends importing one file—if possible—because [!DNL Workfront Library] only processes one metadata import at a time. If you need to import multiple files, you must wait until the first file has finished before you can start another import.

>[!NOTE]
>
>Before formatting your [!DNL CSV] file, you need to set up your metadata schema in [!DNL Workfront Library] to match the structure of your previous content tool. To learn how, see [Set up taxonomy metadata for [!UICONTROL Workfront Library]](../../../workfront-library/administration-and-setup/metadata/set-up-taxonomy-metadata.md).

## Exact match

All information (metadata tags, column headers, etc.) in the [!UICONTROL CSV] file must exactly match what is set up in [!DNL Workfront Library]. Having slight variations—including extra spaces, abbreviations, or punctuation—could result in duplicate information being added to the metadata schema or metadata not mapping correctly to the asset. However, the fields are not case sensitive, so you don't need to worry about capitalization.

For example, if you entered the tag *US* in the [!UICONTROL CSV] file but [!DNL Workfront Library] had the tag *U.S.* instead, then [!DNL Workfront Library] would create a new tag. Entering *us* in the [!UICONTROL CSV] file would correctly map to the metadata tag *US*.

## Required column headers

The [!UICONTROL CSV] file must match the same structure as the metadata schema in [!DNL Workfront Library]. You must include a column for each metadata field that you want to apply to assets listed in the CS[!UICONTROL ]V file.

The [!UICONTROL CSV] file must also include these column headers:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>filepath</p> </td> 
   <td>This column includes the filepath of the asset's location in [!DNL Workfront Library]. If you move an asset to a different folder prior to importing the metadata, you need to update the filepath to the new location. If an asset is in the [!UICONTROL My Content] area of [!DNL Workfront Library], the [!UICONTROL filepath] column must be left blank for the metadata to map properly to the asset.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>filename</p> </td> 
   <td>This column includes the filename of the asset in [!DNL Workfront Library]. The filename must include the filetype, such as <i>.pdf</i> or <i>.png</i>. [!DNL Workfront Library] does allow you to have the same filename for different assets with no repercussions from importing metadata, however, having duplicate filenames with the same filepath could result in only one of these rows mapping.</td> 
  </tr> 
 </tbody> 
</table>

Although the [!UICONTROL keywords] column header is not required, you must include this column if you want to map [!UICONTROL keywords] to your assets. To learn about requirements for the [!UICONTROL keywords] column, see [Keyword hierarchy](#keyword-hierarchy).

## Date format

Any dates in the [!UICONTROL CSV] file must be listed in MM/DD/YYYY format. Otherwise, the metadata won't map to the asset in [!DNL Workfront Library].

## Multi-select metadata

To indicate that you want multiple tags selected from a metadata field, you must add the Pipe character to separate the tags. Adding a space to either side of the Pipe character results in spaces being added to the metadata, which could result in new tags being added to the metadata fields and assets. For example, typing "Fall 2018|Fall 2019" in a cell would select both locations in a multi-select field.

If you enter multiple tags in a column that maps to a single-select field, only the first tag maps correctly to the asset. To learn what happens when you add multiple tags to a single-select field or a multi-select field that aren't currently included as selections, see [How information updates](#how-information-updates).

>[!NOTE]
>
>If you were previously using commas to separate multiple tags within a field, you can use the [!UICONTROL SUBSTITUTE] function to quickly replace all commas with the Pipe character.

## Keyword hierarchy {#keyword-hierarchy}

>[!NOTE]
>
>If you have a metadata field titled "[!UICONTROL keywords]" within your taxonomy metadata in [!DNL Workfront Library], it will not update and you need to change the name both in [!DNL Workfront Library] and in the column header. Otherwise, this column will add any additional keywords in the keyword metadata fields to the asset(s).

Workfront Library allows you to create hierarchical keywords. Unlike the taxonomy metadata, the keyword structure does not need to be set up prior to importing the [!UICONTROL CSV] file. Instead, you can create the hierarchy by importing the file. To learn more about keywords in [!DNL Workfront Library], see [Overview of keyword metadata in [!UICONTROL Workfront Library]](../../../workfront-library/administration-and-setup/metadata/keyword-metadata-overview.md).

Any keywords that you need to add to your assets must be in a column with the column header "[!UICONTROL keywords]." The text listed in this column automatically maps to the keyword metadata in [!DNL Workfront Library]. You must indicate the keyword hierarchy within the cell, separating each level with the Greater Than Sign character. For example, "Fashion campaign>Fall>2019" is 3 levels deep with "Fashion campaign" as the root parent keyword.

If an asset has multiple keyword tags, you must separate them with the pipe character. For example, "Fashion campaign>Fall>2019|Fashion campaign>Fall>2018" is tagged with 2 keywords that have the same parent keywords at the first and second levels.

Adding a space to either side of the Pipe character or Greater Than Sign character results in spaces being added to the metadata, which could result in new tags being added to the metadata fields and assets.

To learn what happens when an asset already has keywords selected in [!DNL Workfront Library] and you add different keyword in the [!UICONTROL CSV] file, see [How information updates](#how-information-updates).

## How information updates {#how-information-updates}

If an asset already has metadata information in [!DNL Workfront Library] but the metadata listed in the [!UICONTROL CSV] file is different, the metadata for the asset updates to match the information in the [!UICONTROL CSV] file. The way this works varies for the different types of metadata fields in [!DNL Workfront Library].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Single-select fields</strong> </p> </td> 
   <td>Regardless of whether metadata exists for the asset already, the tag entered in the column of a single-select field is mapped to the asset listed and all previous selections are removed from that field. If there are multiple tags listed for a single-select metadata option, only the first tag maps to the asset. However, the additonal tags listed will be added as options if they weren't already options for that field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Multi-select fields</strong> </p> </td> 
   <td>Regardless of whether metadata exists for the asset already, the tag(s) entered in the column of a multi-select field is mapped to the asset listed and all previous selections are removed from the field. If there are tags listed that aren't already options for that field, they are added as selections.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Keyword fields</strong> </td> 
   <td> <p>Any keywords entered in this column are added to the current keyword list for the asset. All keywords previously added to the asset remain.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Blank cells</strong> </td> 
   <td> <p><span style="font-weight: normal;">Leaving a cell blank in a column does not affect an asset's current metadata selections. To remove metadata information from an asset, you must remove them manually.</span> </p> </td> 
  </tr> 
 </tbody> 
</table>

If you add a column that doesn't exactly match a metadata field in [!DNL Workfront Library], nothing in that column will map to the assets listed. To make sure that everything maps correctly, it is very important to make sure the column names, metadata field selections, and all other information listed in each row exactly matches the taxonomy in [!DNL Workfront Library]'s [!UICONTROL Setup] area. Neglecting to do so can result in creating duplicate metadata tags or metadata not mapping correctly to an asset.

To learn how to import the [!UICONTROL CSV] file, see [Use [!DNL Workfront Library]'s import tool to add metadata to content](../../../workfront-library/administration-and-setup/metadata/import-metadata-for-content.md).
