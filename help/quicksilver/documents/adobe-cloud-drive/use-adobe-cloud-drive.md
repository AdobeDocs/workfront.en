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
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any package with Adobe cloud storage</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Workfront v2</p></td> 
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

| Status | File meaning | Folder meaning |
|---|---|---|
| Online only | File is synced but only available online. | All files inside are available online. |
| Syncing | File is uploading or downloading. | At least one file in the folder is syncing. |
| Available offline | File is synced and available offline. | At least one file in the folder is available offline. |
| Pinned (Always Keep on Device) | File is synced and always kept offline. Adobe Cloud Drive doesn't purge pinned content automatically. | All files in the folder are downloaded and available offline. |
| Read only | File is read only. | Folder is read only. |
| Sync error | File can't be synced. Hover over the icon for details. | Folder can't be synced. Hover over the icon for details. |
| Sync excluded | File can't be synced due to unsupported type or name. | Folder can't be synced due to unsupported name. |

### File status indicators on Mac

| Status | File meaning | Folder meaning |
|---|---|---|
| Available offline (no icon) | File is synced and available offline. | All files are downloaded and available offline. |
| Online only | File is synced and available online only. | At least one file in the folder is online only. |
| Syncing | File is uploading or downloading. | Folder content is uploading or downloading. |
| Sync error | File can't update or sync. Hover over the icon for details. | Folder can't update or sync. Hover over the icon for details. |
| Sync excluded | File is excluded from sync. | Folder is excluded from sync. |
| Read only | File is read only. | Folder is read only. |
| Pinned (Always Keep on Device) | File is pinned to be available offline. Adobe Cloud Drive doesn't purge pinned content automatically. | Folder is pinned to be available offline. |

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
* **Clear naming.** Conflict files include the username and timestamp in this format: `filename (Conflicted copy from username on date_time).extension`. For example: `abc (Conflicted copy from John on 2026-02-10_16-06-44).txt`.

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
