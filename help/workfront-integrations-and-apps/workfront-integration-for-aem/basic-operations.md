

# `Workfront Tools for AEM User Guide : Basic Operations`

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p><em>Work</em> or higher</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Work</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have a license to Adobe Experience Manager</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

* You must install Workfront Tools for Adobe Experience Manager before you can use it to perform these basic operations.

  For instructions, see [Workfront Tools for AEM User Guide: Installation Guide 1.x.x](../../workfront-integrations-and-apps/workfront-integration-for-aem/installation-guide.md)

## Testing Webhooks basic operations

[https://one.workfront.com/s/article/Document-Webhooks-API-745459769](https://one.workfront.com/s/article/Document-Webhooks-API-745459769)

## Files Webhook

1. Go to `Documents`tab in the top main menu.
1. Click on `Add New` and select `From <your AEM instance>`
1. You should see `Link External Files and Folders` menu showing the content of an AEM folder in your AEM instance.
1. Click on the first item in the breadcrumb of the menu. You should now see all files and folders in /content/dam folder.
1. Browse to a folder with +1000 files inside. You should see all files listed in the menu. Do not change to “ `thumbnail` view because it will break. *Workfront* has not implemented pagination yet.
1. Select a folder and click `Link`. Open the linked folder, you should see all child folders and assets that are within that folder in AEM.

## Metadata Webhook

1. Open a linked folder that contains sub-folders and assets.
1. Verify that the folders correctly display the folder’s title.
1. Verify that the assets correctly display:

  1. Title
  1. Thumbnail
  1. Size

1. Check the json response if possible (ngrok?)

  1. If option “Access DAM through API endpoints” in Advanced tab of the cloud services configuration is unchecked, then viewLink should look like: [https://6c8828a8b3bd.ngrok.io/content/dam/workfront/broadcast_audio_projects/2020_example_program/2020/activities/test_0609-2/background-blur-test-asset.jpg](https://6c8828a8b3bd.ngrok.io/content/dam/workfront/broadcast_audio_projects/2020_example_program/2020/activities/test_0609-2/background-blur-test-asset.jpg) and downloadLink should look like: [https://6c8828a8b3bd.ngrok.io/content/dam/workfront/broadcast_audio_projects/2020_example_program/2020/activities/test_0609-2/background-blur-test-asset.jpg/jcr:content/renditions/original](https://6c8828a8b3bd.ngrok.io/content/dam/workfront/broadcast_audio_projects/2020_example_program/2020/activities/test_0609-2/background-blur-test-asset.jpg/jcr:content/renditions/original)
  1. If option “Access DAM through API endpoints” in Advanced tab of the cloud services configuration is checked, then viewLink and downloadLink should both look like: [https://6c8828a8b3bd.ngrok.io/bin/workfront-tools/view?id=d2b498a7-485c-4128-a06f-f73c893a9371](https://6c8828a8b3bd.ngrok.io/bin/workfront-tools/view?id=d2b498a7-485c-4128-a06f-f73c893a9371)

1. Verify that `View` and `Download` options work correctly with and without option `Access DAM through API endpoints` checked.

## Search Webhook

1. Go to `Documents` tab in the top main menu.
1. Click on `Add New` and select `From <your AEM instance>.`
1. You should see `Link External Files and Folders` menu showing the content of an AEM folder in your AEM instance.
1. Type a search term that will not match any file in AEM. You should see a message that specifies that no file was found.
1. Type a search term that will match some files in AEM. Current search implementation will only search for files that contain the search term in their name (not it their title). You should see the files that were found. Each file should display the titles of all folders in the path where the file is located.
1. Type a search term that will match +100 files. You should see only 100 results. Pending to verify with *Workfront* why the search is not paginating, *Workfront* webhooks will not request the second set of 100 files.

## Download Webhook

NOT IMPLEMENTED.

## Thumbnail Webhook

1. Go to “ `Documents`” tab in the top main menu.
1. Click on `Add New` and select “ `From <your AEM instance>.`
1. Browse to a folder that has assets within it. Check that the thumbnails display correctly.
1. Step back one level in the breadcrumb list, select the folder that contained the assets and link it.
1. Open the linked folder and verify that the thumbnails are displayed correctly.

## View Link

1. Verify that `Access DAM through API endpoints` in `Advanced`tab of the cloud services configuration is unchecked.
1. Upload an image into a linked folder and select the image. Click on `Open`.
1. The image should open in a new tab. Verify that the call to get the image was made directly to /content/dam… path.
1. Update `Access DAM through API endpoints` in `Advanced`tab of the cloud services configuration option to be checked.
1. Upload a new image into a linked folder and select the image. Click on `Open`.
1. The image should open in a new tab. Verify that the call to get the image was made to /bin/workfront-tools/view
1. Delete the image in AEM. Click `Open` again in *Workfront*. /bin/workfront-tools/view call should now return 404.

## Upload Init and Upload Webhooks

1. Send a document from the Documentsarea:

  1. Upload an image to *Workfront* `Documents`tab in the main navigation.
  1. Attach `Workfront Tools Document` custom form and fill in all fields.
  1. Select the document and click on `More → Send to → <your AEM instance>`. Select a folder that has `Workfront Tools` metadata schema applied and click `Save`.
  1. Verify that the asset together with the document metadata have been sent correctly.

1. Send a document from a Project:

  1. Upload an image to the `Documents`tab of a Workfront Project.
  1. Attach `Workfront Tools Document` custom form to the document and fill in all fields.
  1. Attach `Workfront Tools Project` custom form to the project and fill in all fields.
  1. Drag and drop the document into the Project’s linked folder.
  1. Verify that the asset together with the document and project metadata have been sent correctly.

1. Send a document from a Task:

  1. Upload an image to the `Documents`tab of a *Workfront* Task.
  1. Attach `Workfront Tools Document` custom form to the document and fill in all fields.
  1. Attach `Workfront Tools Task` custom form to the document and fill in all fields.
  1. Attach `Workfront Tools Project` custom form to the project and fill in all fields.
  1. Select the document and click on `More → Send to → <your AEM instance>`. Select a folder that has `Workfront Tools` metadata schema applied and click `Save`.
  1. Verify that the asset together with the document, task and project metadata have been sent correctly.

1. Send a document from an Issue:

  1. Upload an image to the `Documents` tab of a *Workfront* Issue.
  1. Attach `Workfront Tools Document` custom form to the document and fill in all fields.
  1. Attach `Workfront Tools Issue` custom form to the document and fill in all fields.
  1. Attach `Workfront Tools Project` custom form to the project and fill in all fields.
  1. Drag and drop the document into the Issue’s linked folder.
  1. Verify that the asset together with the document, issue and project metadata have been sent correctly.

## Service Info Webhook

NOT IMPLEMENTED.

## Create Folder Webhook

1. Go to `Documents`tab in the top main menu.
1. Click on `Add New` and select `From <your AEM instance>`.
1. Select a folder and click `Link`.
1. Open the linked folder and click `Add New → Folder`. Type the new folder’s name.
1. Open the created folder and create another folder within it.
1. Refresh the page in *Workfront* and verify both folders are correctly displayed.
1. Upload an asset to one of the created folders.
1. Verify in AEM that both folders have been created correctly and the asset has been uploaded.

## Delete Webhook

NOT IMPLEMENTED.

## Rename Webhook

NOT IMPLEMENTED.

## Custom Action Webhooks

NOT IMPLEMENTED.  

