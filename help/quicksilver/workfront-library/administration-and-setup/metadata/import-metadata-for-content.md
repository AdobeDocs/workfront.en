---
product-previous: workfront-library
product-area: documents
navigation-topic: metadata
title: Use [!DNL Workfront Library]'s import tool to add metadata to content
description: If you're new to [!DNL Workfront Library] and have just uploaded hundreds or thousands of assets, there's no need to manually add metadata to each asset individually. A [!DNL Workfront Library] Administrator can easily import metadata to these assets using a CSV file. To learn more about metadata, see Overview of metadata in [!DNL Workfront Library].
feature: Workfront Library, Digital Content and Documents
exl-id: fd1652b6-6053-43e9-9d6d-6ede5b8bbcc9
---
# Use [!DNL Workfront Library]'s import tool to add metadata to content

If you're new to [!DNL Workfront Library] and have just uploaded hundreds or thousands of assets, there's no need to manually add metadata to each asset individually. A [!DNL Workfront Library] Administrator can easily import metadata to these assets using a [!UICONTROL CSV] file. To learn more about metadata, see [Overview of metadata in [!DNL Workfront Library]](../../../workfront-library/administration-and-setup/metadata/metadata-overview.md).

>[!NOTE]
>
>Depending on the amount of assets you have, there are 3 options available for adding assets to [!DNL Workfront Library]: >
>* Direct upload (recommended if you have less than 50 GB of assets)
>* [!DNL AWS S3] bucket exchange
>* [!DNL AWS Snowball]
>
>If you are a [!UICONTROL Workfront DAM] customer, you can transfer the metadata through this process. To learn more about any of these options, contact [!DNL Workfront]'s Professional Services department.

Before you can add the metadata to your uploaded assets, you must set up your metadata schema in [!DNL Workfront Library] and format your [!UICONTROL CSV] file to meet all requirements. Failure to include the appropriate metadata schema or properly format your [!UICONTROL CSV] file could result in metadata not mapping correctly to your assets.

To learn how to complete these requirements, see:

* [Set up taxonomy metadata for [!DNL Workfront Library]](../../../workfront-library/administration-and-setup/metadata/set-up-taxonomy-metadata.md)
* [Format your [!UICONTROL CSV] file for metadata import in [!DNL Workfront Library]](../../../workfront-library/administration-and-setup/metadata/format-your-csv-file-for-metadata-import.md)

After completing the actions above, you can import the file.

1. In [!DNL Workfront], click the [!UICONTROL Workfront Library] **icon** in the top-right corner of the screen.
1. In [!DNL Workfront Library], click the **[!UICONTROL Menu]** icon, then go to [!UICONTROL Setup] > [!UICONTROL Metadata] > [!UICONTROL Import].

   ![](assets/import-area.png)

   >[!NOTE]
   >
   >Because you can only import one [!UICONTROL CSV] file at a time, [!DNL Workfront] recommends importing only one [!UICONTROL CSV] file if you have less than 100,000 rows of metadata.

1. If your [!UICONTROL CSV] file is properly formatted, click **[!UICONTROL Choose CSV]**, then double-click the file in your computer to upload it. The import begins and you are unable to import additional files until it completes.

   If a row in the [!UICONTROL CSV] file fails to map to an asset in [!DNL Workfront Library], a link appears allowing you to download a report detailing the filenames and filepath of rows that did not import. You may need to manually update the metadata for these assets.

   ![](assets/download-error-report-350x256.png)
