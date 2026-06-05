---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Troubleshoot Adobe Cloud Drive
description: Review limitations, performance considerations, and solutions to common issues with Adobe Cloud Drive on Mac and Windows.
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
# Troubleshoot Adobe Cloud Drive

This article describes the limitations of Adobe Cloud Drive, performance considerations to keep in mind, and solutions to common issues you might encounter.

For information about working with Adobe Cloud Drive, see [Use Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Limitations

### File and folder operations

* Project folders are read-only at the top level. You can't rename, delete, or move them from Adobe Cloud Drive. To create, rename, or delete a project, use the Workfront web interface.
* File and folder operations inside a project folder are fully supported.

### File and path limits

* File names can't exceed 255 characters on any platform.
* The full file path (all folder names plus the file name) can't exceed 1024 characters. Files with paths longer than this limit don't appear in Adobe Cloud Drive, even if they're visible in the Workfront web interface.
* If you see a **Full path too long** error on a file, shorten the folder names or reduce the folder nesting depth to bring the path within the limit.

### Storage

* Files cached locally use disk space on your device.
* Cloud-only files don't use local storage.
* Remove offline access for files you no longer need. For more information, see [Remove offline access to free up space](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#remove-offline-access-to-free-up-space) in [Use Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Performance considerations

* **File size:** The time required to sync depends on the file size. Larger files generally take longer.
* **Network speed:** Faster connections provide better sync performance. Sync automatically resumes after an interruption.
* **First-time access:** Files are downloaded on demand the first time you access them. Subsequent access is faster because the file is cached locally.

## Common issues

### Adobe Cloud Drive isn't appearing

**Possible causes:**

* Adobe Cloud Drive isn't installed.
* Installation didn't complete successfully.
* Your organization isn't on a version of Workfront that supports Adobe cloud storage.

**Solutions:**

* Verify that Adobe Cloud Drive is installed. Check **Applications** (Mac) or **Programs** (Windows).
* Launch Adobe Cloud Drive manually.
* Contact your Workfront administrator to confirm that your organization is on a version of Workfront that supports Adobe cloud storage.
* Reinstall Adobe Cloud Drive if necessary. For more information, see [Install Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

### The Adobe Cloud Drive icon isn't visible in the menu bar or taskbar

**Possible causes:**

* The menu bar (Mac) or system tray (Windows) doesn't have enough space to display the icon.

**Solutions:**

* **Mac:** Hold Cmd and drag existing menu bar icons to rearrange or remove them, creating space for the Adobe Cloud Drive icon.
* **Windows:** Click the up arrow (**Show hidden icons**) in the taskbar to find the Adobe Cloud Drive icon, then drag it to the visible area.

### Projects aren't showing, or some projects are missing

**Possible causes:**

* You don't have access to any projects.
* Sync hasn't completed.
* You have a network connectivity issue.

**Solutions:**

* Verify your project access in the Workfront web interface.
* Check your network connection.
* Sign out of Adobe Cloud Drive and sign back in.

### Files aren't syncing

**Possible causes:**

* You have a network connectivity issue.
* There's a sync error on the file or folder.
* You don't have enough disk space.

**Solutions:**

* Check your internet connection.
* Verify that you have enough disk space available.
* Check the file status indicators for sync errors. For more information, see [File status indicators](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#file-status-indicators) in [Use Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).
* Restart Adobe Cloud Drive.
* Check the Adobe Cloud Drive status in the system tray (Windows) or menu bar (Mac).

### You can't open a file

**Possible causes:**

* The file is cloud-only and the download failed.
* The application required to open the file isn't installed.
* The file is corrupted.

**Solutions:**

* Check the file status indicator.
* Make sure the required application is installed.
* Right-click the file, select **Always Keep On This Device**, then try opening it again.
* Verify that the file isn't corrupted in the Workfront web interface.

### Sync is slow

**Possible causes:**

* The file is large.
* Your network connection is slow.
* Many files are syncing at the same time.

**Solutions:**

* Be patient with large files. Sync is resumable, so it picks up where it left off after an interruption.
* Check your network speed.
* Limit the number of simultaneous file operations.
* Keep large files cloud-only unless you need offline access.

### Offline files are taking too much space

**Solutions:**

* Right-click offline files and select **Free Up Space**.
* Check your disk space regularly.
* Keep large files you rarely access in cloud-only mode.

### You can't create, edit, or delete files or folders

**Possible causes:**

* You're trying to create, rename, or delete a project folder. Project folders are read-only at the top level.
* The project is read-only for you, so you can't create, edit, or delete files or folders within it.

**Solutions:**

* To create, rename, or delete a project, use the Workfront web interface.
* Ask the project owner to share the project with you with edit access.

## Get help

For license questions, project access issues, or organization-specific configuration, contact your Workfront administrator.

To share logs with Adobe support, follow the steps in [Run the Adobe log collector tool](https://helpx.adobe.com/creative-cloud/apps/troubleshoot/diagnostics-repair-tools/run-log-collector-tool.html).

## Best practices

* **Plan offline work.** Download files before you travel or work in areas with poor connectivity.
* **Monitor sync status.** Check file indicators before you close applications.
* **Follow the project's folder structure.** Organize files within project folders as the project owner intends.
* **Use descriptive file names.** Help your team members find what they need.
* **Avoid creating duplicates.** Don't make unnecessary copies of files.
