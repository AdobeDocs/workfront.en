---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Use Adobe Cloud Drive
description: Work with your Adobe cloud storage projects directly from Finder or File Explorer using Adobe Cloud Drive. Open and edit files in any application, work offline, and resolve conflicts.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Use Adobe Cloud Drive

After you install Adobe Cloud Drive, you can work with your Adobe cloud storage projects directly from Finder or File Explorer. You can open and edit files in any application, work offline, and let Adobe Cloud Drive sync your changes to the cloud.

For information about installing Adobe Cloud Drive, see [Install Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront version</td> 
   <td>Workflow Ultimate, with Adobe cloud storage enabled</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>
      <p>View access to a project to see it in Adobe Cloud Drive</p>
      <p>Edit access to a project to add, edit, or delete files in it</p>
   </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Access your projects

1. Open Finder (Mac) or File Explorer (Windows).
1. Navigate to **Adobe Cloud Drive**.
1. Browse the list of projects you have access to in Workfront. Open any project folder to view its files and subfolders.

   >[!NOTE]
   >
   >* Project folders are read-only at the top level. You can't rename, delete, or move project folders themselves.
   >* You can work with files and folders inside a project folder — open, edit, create, delete, and so on.
   >* Legacy Workfront projects don't appear in Adobe Cloud Drive. Only projects stored in Adobe cloud storage are available.

## File status indicators

Adobe Cloud Drive uses visual indicators to show file synchronization status. The icons differ between Windows and Mac.

### File status indicators on Windows

| Icon | Status | File meaning | Folder meaning |
| --- | --- | --- | --- |
| ![Online only icon](assets/acd-windows-online-only.png) | Online only | File is synced but only available online. | All files inside are available online. |
| ![Syncing icon](assets/acd-windows-syncing.png) | Syncing | Latest updates to the file are syncing to the local cache or to Adobe cloud storage. | At least one file in the folder is syncing. |
| ![Available offline icon](assets/acd-windows-available-offline.png) | Available offline | File is synced and available offline. | At least one file in the folder is available offline. |
| ![Pinned icon](assets/acd-windows-pinned.png) | Pinned (Always Keep on Device) | File is synced and always kept offline. Adobe Cloud Drive doesn't purge pinned content automatically. | All files in the folder are in local cache and available offline. |
| ![Read only icon](assets/acd-windows-read-only.png) | Read only | File is read only. | Folder is read only. |
| ![Sync error icon](assets/acd-windows-sync-error.png) | Sync error | File can't be synced. Hover over the icon for details. | Folder can't be synced. Hover over the icon for details. |
| ![Sync excluded icon](assets/acd-windows-sync-excluded.png) | Sync excluded | File can't be synced due to unsupported type or name. | Folder can't be synced due to unsupported name. |

### File status indicators on Mac

| Icon | Status | File meaning | Folder meaning |
| --- | --- | --- | --- |
| (No icon) | Available offline | File is synced and available offline. | All files are available offline. |
| ![Online only icon](assets/acd-mac-online-only.png) | Online only | File is synced and available online only. | At least one file in the folder is online only. |
| ![Syncing icon](assets/acd-mac-syncing.png) | Syncing | Latest updates to the file are syncing to the local cache or to Adobe cloud storage. | Folder content is syncing. |
| ![Sync error icon](assets/acd-windows-sync-error.png) | Sync error | File can't update or sync. Hover over the icon for details. | Folder can't update or sync. Hover over the icon for details. |
| ![Sync excluded icon](assets/acd-windows-sync-excluded.png) | Sync excluded | File is excluded from sync. | Folder is excluded from sync. |
| ![Read only icon](assets/acd-mac-read-only.png) | Read only | File is read only. | Folder is read only. |
| ![Pinned icon](assets/acd-windows-pinned.png) | Pinned (Always Keep on Device) | File is pinned to be available offline. Adobe Cloud Drive doesn't purge pinned content automatically. | Folder is pinned to be available offline. |

### Error tooltips

When a sync error or issue occurs, hover over the file or folder icon to see a tooltip describing the issue.

| Error category | Tooltip | Meaning |
|---|---|---|
| Sync excluded | Unsupported file type | The file type isn't supported by Adobe Cloud Drive. |
| Sync excluded | Unsupported file name | The file name isn't supported by Adobe Cloud Drive. |
| Sync excluded | Parent project deleted | The parent Workfront project has been deleted. |
| Sync suspended | File content not supported | The file content can't be synced (for example, a security issue was detected). |
| Sync suspended | Invalid characters in file name | The file name contains invalid characters. |
| Sync suspended | Full path too long | The file path exceeds the maximum length allowed. |
| Sync suspended | No write permission | Your write access to this file or project has been revoked. |
| Sync error | Authentication issue | There's a problem with your sign-in credentials. |
| Sync error | Cloud storage unavailable | Adobe cloud services are temporarily unavailable. |
| Sync error | Cloud storage full | Your cloud storage quota is full. |
| Sync error | Local disk full | Your local disk doesn't have enough free space. |
| Sync error | No internet connection | Your device isn't connected to the internet. |
| Sync error | Unexpected error | An unexpected error occurred during sync. |
| Sync error | Account blocked | Your account has been blocked by the service. |

>[!NOTE]
>
>System-level errors — such as disconnected, authentication failure, network unavailable, local disk full, or cloud storage full — are shown in the system tray (Windows) or menu bar (Mac), not on individual files.

### Sync Exclusion List

Adobe Cloud Drive excludes certain system-generated, temporary, and lock files from synchronization. The following file types and patterns are excluded:

| Category | File types / patterns | Description |
|---|---|---|
| System files | `.DS_Store`, `Thumbs.db` | Operating system metadata and thumbnail cache files. |
| System and virtual memory files | `*.sys` (for example, `hiberfil.sys`, `pagefile.sys`, `swapfile.sys`) | Large system files used for virtual memory, hibernation, or other operating system functions. |
| macOS indexing files | `.Spotlight-V100`, `.fseventsd` | macOS Spotlight indexing and file system event tracking files. |
| Temporary and backup files | `*.tmp`, `*.swp`, `*~`, `*.bak` | Temporary, transient, or backup files generated by applications. |

## Open a file

1. In Adobe Cloud Drive, navigate to the file.
1. Double-click the file.

   The file opens in its default application.

Adobe Cloud Drive supports any file type that an installed application on your computer can open, including:

* Adobe Creative Cloud formats (PSD, AI, INDD, PRPROJ, AEP, and so on)
* Microsoft Office documents (DOCX, XLSX, PPTX)
* Images (JPG, PNG, GIF, and so on)
* Video files (MP4, MOV, and so on)

>[!NOTE]
>
>Cloud Document formats (PSDC, AIDC, and so on) open as their standard equivalents (PSD, AI, and so on) when you access them through Adobe Cloud Drive.

## Edit and save a file

1. Open a file from Adobe Cloud Drive.
1. Make your changes in the application.
1. Save the file by selecting **File** > **Save**, or by pressing Ctrl+S (Windows) or Cmd+S (Mac).

   Your changes sync automatically to Adobe cloud storage.

>[!IMPORTANT]
>
>Save files using **File** > **Save** or the keyboard shortcut. Avoid using **Save As** to create copies, because it generates duplicate files in the drive.

## Create or add a new file

You can create a new file directly in a project, or add an existing file from your local storage.

### Create a new file from an application

1. Open the application you want to use to create the file.
1. Create the file as you normally would.
1. When you save, choose a location inside an Adobe Cloud Drive project folder.

   The file appears in Adobe Cloud Drive and syncs to Adobe cloud storage.

### Add an existing file to a project

1. In Finder (Mac) or File Explorer (Windows), open the project folder in Adobe Cloud Drive.
1. Drag or copy files from your local storage into the project folder.

   The files sync automatically to Adobe cloud storage.

## Make files and folders available offline

When a file or folder is available offline, you can open and edit it without an internet connection. Offline files use local disk space.

### Keep a file or folder on your device

1. Right-click the file or folder in Adobe Cloud Drive.
1. Select **Always Keep On This Device**.

   The file or folder downloads to your local cache, and you can work with it even when you're offline.

### Remove offline access to free up space

1. Right-click the offline file or folder.
1. Select **Free Up Space**.

   The file or folder remains in cloud storage, but it's removed from your local cache.

>[!NOTE]
>
>Offline files and folders use local disk space. Remove offline access for files and folders you no longer need to free up space.

## Copy a file to local storage

You can copy a file out of Adobe Cloud Drive to your local drive. The original remains in Adobe Cloud Drive, and the copy becomes an independent local file.

1. Right-click the file in Adobe Cloud Drive.
1. Select **Copy**, then paste the file into the location on your local drive where you want it.

   The file copies to the destination. The original remains in Adobe Cloud Drive.

>[!NOTE]
>
>Files copied to your local storage are independent copies. Changes you make to a local copy don't sync back to Adobe cloud storage.

<!-- Courtney check me: New sections below (Upload to Cloud through Open in Workfront) added for Adobe Cloud Drive v1.2.0, per helpxNewFeature.pdf from Pulkit Goel. Verify content, placement, and heading order. -->

## Upload files to the cloud (Direct Upload) {#direct-upload}

<!-- Courtney check me: Source PDF calls this "Upload to Cloud (Direct Upload)". Confirm heading wording. -->

Direct Upload sends files and folders from your computer directly to Adobe cloud storage, without first copying them into the Adobe Cloud Drive folder.

### Upload files or folders

1. Right-click a file or folder in Finder (Mac) or File Explorer (Windows).
1. Select **Upload to Cloud**.
1. In the destination picker, select a location within one of the projects in Adobe Cloud Drive, then click **Upload Here**.
1. Monitor progress in the **Direct Upload** section of the Sync Activity window.

### Things to know about Direct Upload

* Direct Upload copies the item to the cloud. The original item remains in its current location.
* You can select multiple items to upload at once.
* The Direct Upload section lists individual files only, up to a maximum of 500. Folders are uploaded together with their contents and aren't listed as separate entries.
* You can upload items from your user home directory or from any attached external drive. Other cloud storage locations, such as iCloud Drive or `~/Library/CloudStorage`, aren't supported.
* You must be signed in with an entitled Adobe account. You don't need an internet connection to start an upload. Without a connection, uploads remain queued.
* Pausing sync cancels uploads that are in progress. Queued uploads resume automatically when you resume sync.
* If you quit Adobe Cloud Drive during an upload, in-progress uploads are marked as cancelled. Queued uploads resume automatically when you restart the app.
* Hidden files and folders, symbolic links, and aliases aren't supported.
* Adobe Cloud Drive controls how many uploads run at the same time. The remaining uploads stay queued until a slot becomes available.
* A live count of uploads, including failed uploads, is displayed, for example "3 files uploading." When all uploads complete successfully, the count changes to a summary such as "3 files uploaded." Select **Dismiss** to remove it.

<!-- Courtney check me: "Pausing sync cancels uploads in progress" and the quit behavior are from the PDF. Confirm with dev that both are intended. -->

### Upload status

<!-- Courtney check me: Icons extracted from the PDF (48x48 px, low resolution) and named by table order. Verify each icon matches its status and ask Pulkit's team for higher-resolution originals. Add alt text review too. -->

| Icon | Status | Description | Available actions |
| --- | --- | --- | --- |
| ![Queued icon](assets/acd-upload-status-queued.png) | Queued | The upload is waiting to start. | **Cancel** cancels this item. |
| ![Uploading icon](assets/acd-upload-status-uploading.png) | Uploading | The upload is in progress. | **Cancel** cancels this item. |
| ![Completed icon](assets/acd-upload-status-completed.png) | Completed | The upload finished successfully. | **Open in Workfront** opens the asset in the Workfront web interface. |
| ![Failed icon](assets/acd-upload-status-failed.png) | Failed | The upload couldn't be completed. | **Show source file** reveals the original file. **Retry** retries the upload. Retry is available only for certain failures. |
| ![Cancelled icon](assets/acd-upload-status-cancelled.png) | Cancelled | The upload was stopped, either by you or by the system. | None. Cancelled uploads aren't retried. You must start a new upload. |

To see the reason for a failure, hover over the failed item.

### Manage the upload list

Each action is available only when it applies.

* **Cancel all uploads:** Available when uploads are queued or in progress. Cancels all of them.
* **Retry failed uploads:** Available when failed uploads that can be retried exist. Retries all of them. Uploads that can't be retried remain unchanged.
* **Clear:** Available when no uploads are queued or in progress. Removes all completed, failed, and cancelled items. Local files and content already uploaded aren't affected.
* **Automatic clearing:** Completed, failed, and cancelled items are removed automatically 24 hours after their last update. Queued and in-progress items are never removed automatically.

## Pause and resume sync {#pause-resume-sync}

You can pause Adobe Cloud Drive when you don't want it to upload or download files, for example on a slow or metered internet connection. While sync is paused, your changes aren't sent to the cloud, and changes from the cloud aren't downloaded to your computer. Sync stays paused until you resume it.

### Pause sync

1. Click the Adobe Cloud Drive icon in the system tray (Windows) or the menu bar (Mac).
1. Click the **Menu** icon (≡) in the top-right corner of the Adobe Cloud Drive window.
1. Select **Pause sync**.

   >[!TIP]
   >
   >With the Adobe Cloud Drive window open, you can also press Ctrl+P (Windows) or Command+P (Mac).

   The Adobe Cloud Drive window shows **Sync is paused** and the message **Files will not sync until you resume**. When you hover over the Adobe Cloud Drive icon, it shows **Adobe Cloud Drive (Paused)**.

>[!NOTE]
>
>Pause sync is available only when you're signed in and Adobe Cloud Drive is connected.

### Resume sync

1. Click the Adobe Cloud Drive icon in the system tray (Windows) or the menu bar (Mac).
1. Do one of the following:

   * Click **Resume**.
   * Click the **Menu** icon (≡), then select **Resume sync**. With the window open, you can also press Ctrl+R (Windows) or Command+R (Mac).

   Adobe Cloud Drive starts syncing again, including any changes you made while sync was paused.

## View and manage version history {#version-history}

You can use Version History in Adobe Cloud Drive to browse saved cloud versions of a supported file, view version details and thumbnails, and revert to an earlier version. You can also edit a version's name and description if you have the required permissions.

### View version history

1. Navigate to your Adobe Cloud Drive folder in Finder or File Explorer.
1. Select a supported file.
1. Right-click the file and select **Version History**.
1. Select a version to view its available details and thumbnail.

   If the file has no previous versions, **No earlier versions** is displayed. Thumbnails might not be available for every file or version.

### Edit version information

1. Open Version History for the file.
1. Select the version you want to update.
1. Open the version's options menu and select **Edit version info**.
1. Enter a **Version name** or **Description**.
1. Select **Save**.

   The updated information is saved and appears when you reopen Version History.

### Revert to an earlier version

1. Open Version History for the file.
1. Select the version you want to restore.
1. Select **Revert to this version**, if available.
1. Wait for synchronization to complete.
1. Reopen the file to verify that the content of the selected version is now current.

## Manage local storage {#manage-local-storage}

You can use Manage Local Storage in Adobe Cloud Drive to monitor local disk usage, set a storage limit, and view files marked as **Always on this device**.

<!-- Courtney check me: PDF says "Always on this device" here but this article uses "Always Keep On This Device" for the right-click option. Confirm which label the UI shows in each place. -->

### View local storage usage

1. Select the Adobe Cloud Drive icon and open its options menu.
1. Select **Manage Local Storage**.
1. Review the current storage usage and the list of files marked as **Always on this device**.
1. Sort the file list by **Name** or **Size** to find specific files.

### Change the local storage limit

1. Open **Manage Local Storage** from the Adobe Cloud Drive options menu.
1. Enter the desired storage limit.
1. Select **Save** to apply the change.

>[!NOTE]
>
>Make sure sufficient free disk space is available on your device when you set the storage limit.

## View sync activity {#sync-activity}

Sync Activity shows recent activity between the Adobe Cloud Drive folder on your computer and Adobe cloud storage. Use it to monitor uploads and downloads, review completed changes, and identify items that couldn't sync.

### View sync activity

1. Select the Adobe Cloud Drive icon in the menu bar (Mac) or system tray (Windows).
1. Expand the sync activity section using the arrow beside its status summary.
1. Review the listed items and their status indicators. Hover over a status indicator to see transfer progress, the completed operation, or an error message.
1. Select the more-actions menu beside an item to see the actions available for that item.

### Things to know about Sync Activity

* Normal sync tracks changes made through the Adobe Cloud Drive folder, including uploads, downloads, creates, renames, moves, and deletions.
* The normal sync list contains up to 500 recent entries. New or updated entries appear at the top. Older entries might be removed as the list reaches its limit.
* An entry can initially display **Preparing...** while its name or metadata is being resolved.
* The summary displays the number of items currently syncing. **Sync complete** means no items are currently active. Inspect the list for failed or excluded items rather than treating this summary as confirmation that every item succeeded.
* Files and folders excluded from sync can appear with an error that explains the unsupported name, unsupported type, or other exclusion reason.
* Activity is cleared when you sign out. The list is an activity view, not a permanent audit history.

### Sync status

<!-- Courtney check me: The PDF has two sync status tables (page 7 with 4 statuses, page 8 with 3 statuses and icons). I used the page 8 icons with the page 7 descriptions where they overlap. Confirm and decide whether to keep both tables. -->

| Icon | Status | Description | Available actions |
| --- | --- | --- | --- |
| Waiting indicator | Waiting to sync | The item is waiting for its operation to begin. | **Show in Finder** (Mac) or **Show in Explorer** (Windows), where applicable. |
| ![Uploading icon](assets/acd-sync-status-uploading.png) | Uploading / Downloading | File content is transferring. Hover over the indicator to see the transfer direction and percentage when available. At 100%, the tooltip might show **Finalizing...** until processing completes. | **Show in Finder** or **Show in Explorer**, where applicable. |
| ![Completed icon](assets/acd-sync-status-completed.png) | Synced / completed operation | The operation completed. The tooltip can identify Uploaded, Downloaded, Created, Renamed, Renamed on cloud, Moved, Deleted, or Deleted on cloud. | **Show in Finder** or **Show in Explorer** for non-deleted items. **Open in Workfront** for eligible completed, non-deleted items. |
| ![Failed icon](assets/acd-sync-status-failed.png) | Sync failed / excluded | The item couldn't sync or is excluded from sync. Hover over the indicator for the reason. | **Show in Finder** or **Show in Explorer**, where applicable. Resolve the reported issue before expecting the item to sync. |

Deleted items can't be revealed locally or opened in Workfront from their activity entry.

### Manage the activity list

| Action | Description |
| --- | --- |
| Expand or collapse | Use the arrow beside the sync summary to show or hide individual entries. |
| Show in Finder / Show in Explorer | Locate a non-deleted item in the Adobe Cloud Drive folder. |
| Open in Workfront | Open an eligible completed item in Workfront in your browser. This action isn't available for active, failed, or deleted normal-sync entries. |
| Clear | Available when no normal-sync items are active. Clears finished entries, including failed entries, from the activity view. Clearing history doesn't delete local files or cloud content and doesn't resolve a sync failure. |
| Dismiss | After you clear a completed batch, a synced-items summary might be shown. Select its close button to dismiss the summary. |

>[!NOTE]
>
>Normal-sync rows don't provide the per-item **Retry** or **Cancel** actions used by Direct Upload. For information about Direct Upload, see [Upload files and folders to the cloud (Direct Upload)](#direct-upload).

## Open an item in Workfront {#open-in-workfront}

Open in Workfront takes you from an item in Adobe Cloud Drive to its corresponding location in Workfront in your browser. Use it to continue working with the cloud item in Workfront without searching for it manually.

### Open an item from Finder or File Explorer

1. Open the Adobe Cloud Drive folder in Finder (Mac) or File Explorer (Windows).
1. Select a single file or folder associated with a Workfront item.
1. Right-click the item and select **Open in Workfront**.

   Your browser opens the corresponding Workfront location. If prompted, sign in with an account that has access to that item.

### Open an item from Sync Activity

1. Select the Adobe Cloud Drive icon in the menu bar (Mac) or system tray (Windows).
1. Expand the sync activity section.
1. For an eligible completed, non-deleted item, open the more-actions menu and select **Open in Workfront**.
1. For a file uploaded through Direct Upload, use the same action on its completed entry in the **Direct Upload** section.

### Things to know about Open in Workfront

* Select only one item at a time. Opening multiple selected items in Workfront isn't supported.
* In File Explorer, the command is hidden for items outside the Adobe Cloud Drive folder and for the drive root itself. It's disabled when multiple items are selected.
* An item must have a corresponding Workfront location. Some folders or other items might not have a Workfront mapping, even if they're visible in Adobe Cloud Drive.
* A new local item that hasn't finished uploading might not yet have a Workfront link. Wait for the upload to complete before you try again.
* In normal Sync Activity, the action is offered only for eligible completed entries. It isn't offered for active, failed, or deleted entries.
* In Direct Upload, the action is offered for completed uploads, not for queued, uploading, failed, or cancelled entries.
* You must be signed in to Adobe Cloud Drive. Workfront might also ask you to sign in separately in the browser, and your Workfront permissions still apply.
* You need an internet connection to retrieve an uncached link and to access Workfront. A previously resolved link doesn't provide offline access to Workfront.
* This action opens Workfront in a browser. It doesn't open the file in its desktop application, upload another copy, or change its local offline availability.

### Open in Workfront availability

| Item or state | Open in Workfront behavior | What to do |
| --- | --- | --- |
| Single eligible item in Adobe Cloud Drive | Opens the corresponding Workfront location. | Select **Open in Workfront**. |
| Multiple selected items | Opening multiple items isn't supported. File Explorer disables the command. | Select a single item. |
| New item still uploading | The Workfront link might not yet be available. | Wait for the upload to complete, then try again. |
| Completed normal-sync entry | Available when the item is eligible and hasn't been deleted. | Use the entry's more-actions menu. |
| Completed Direct Upload entry | Available after the upload finishes. | Use the entry's more-actions menu. |
| Item without a Workfront mapping | A message indicates that the item isn't available in Workfront. | Check the item directly in Workfront or choose another supported item. |
| Deleted normal-sync entry | The action isn't available. | Use Workfront directly if you need to investigate the deleted item. |

## Sign out of Adobe Cloud Drive

If you sign out of Adobe Cloud Drive, the drive remains visible in Finder or File Explorer. However, any changes you make inside the drive while signed out, and any changes that hadn't synced before sign-out, don't sync to the cloud.

What happens next depends on which account you sign back in with.

### Sign back in with the same account

Adobe Cloud Drive preserves the local mounted folder when you sign out. If you sign back in with the same credentials:

* Adobe Cloud Drive reuses the existing mount automatically.
* Any unsynced changes you made before sign-out are retained, and they sync once the connection is restored.
* No action is required from you.

### Sign in with a different account

If you sign in with a different Adobe account after signing out:

* The current mounted folder is automatically renamed and backed up. The backup folder name uses this format: `Adobe Cloud Drive <usermail>_<short_guid> (backup yyyy-MM-dd HH-mm-ss)`.
* Adobe Cloud Drive mapped to the new account becomes available in Finder or File Explorer as usual.
* You can manually recover any unsynced work from the backup folder before you remove it.

>[!NOTE]
>
>Backup folders are saved in `~/Library/CloudStorage` on Mac and `C:\Users\<user>\` on Windows. If you switch accounts multiple times, multiple timestamped backup folders are created. Review and clean up backups periodically to free up disk space.

## Resolve file conflicts

Conflicts can occur in any of the following situations:

* Multiple users edit or delete the same file at the same time.
* A file is modified while another user has it open.
* Network interruptions cause sync issues.

### How Adobe Cloud Drive resolves conflicts

Adobe Cloud Drive uses a duplication strategy for conflicts:

* **No file locking.** Multiple users can edit files at the same time.
* **Automatic duplication.** When Adobe Cloud Drive detects a conflict, it preserves both versions.
* **Clear naming.** Conflict files include the username and timestamp in this format: `filename (Conflicted copy from username on date_time).extension`. For example: `hero-banner (Conflicted copy from John on 2026-02-10_16-06-44).psd`.

### Resolve a conflict manually

1. Identify the conflict file. Conflict files have "Conflicted copy" in the filename.
1. Review both versions to determine which one is correct.
1. Keep the correct version and delete the other version.
1. Give the retained file a suitable name.

>[!TIP]
>
>To minimize conflicts:
>
>* Check sync status before editing files.
>* Communicate with team members about who is editing which files.
>* Save frequently so changes sync promptly.
>* Close files when you finish editing.
