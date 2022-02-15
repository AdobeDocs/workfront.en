---
filename: sycn-box-folder
product: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
---



# Sync Box Folders With *`Workfront Proof`* {#sync-box-folders-with-workfront-proof}



>[!IMPORTANT] {type="important"}
>
>This article refers to functionality in the standalone product *`Workfront Proof`*. For information on proofing inside *`Adobe Workfront`*, see [Proofing](_proofing.md).


You can synchronize a Box folder with a folder in *`Workfront Proof`*. Every change you make to your files in the Box folder will be reflected in *`Workfront Proof`* (so uploading a new file, adding a new version, renaming of a file, etc).


For more information about folders, see [Manage Folders and their Contents in Workfront Proof](manage-folders-and-contents.md).


>[!NOTE]
>
>Only users with profiles of Managers or higher are able to sync folders. The Box user who uploads the file to a folder synced with *`Workfront Proof`*, will be made the owner of the *`proof`* created in *`Workfront Proof`* (if they are a user within the same *`Workfront Proof`* account). If the Box user is a user in a different *`Workfront Proof`* account or does not have an account with *`Workfront Proof`*, the person who created the sync between the folders will become the owner of the *`proof`*. For more information, see *"Editing User Profiles and Permissions."*


To synchronize a Box folder with a folder in *`Workfront Proof`*:



1.  `<li value="1">In your Box account, go to the All Files and Folders page.</li>` `<li value="2">Click the <span class="bold">More options</span> menu next to the folder you want to sync with <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> (1).</li>` `<li value="3">Select <span class="bold">More Actions</span> (2).</li>` `<li value="4">Click <span class="bold">Sync with <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span></span> (3).</li>` `<li value="5">In the Sync folder box that appears (if you are logged into <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span>), do one of the following:  <ul>  <li>Click a <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> folder name to sync it with the corresponding folder in Box (4).</li>  <li>Click <span class="bold">New folder</span> to create a new folder in <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> (5).<br><img src="assets/folder-sync-2-350x231.jpg" alt="folder_sync_2.jpg" style="width: 350;height: 231;">If you chose to create a new folder, you are prompted to provide details about the new folder.</li> </ul></li>` `<li value="6">Click <span class="bold">Save</span>.<br>The Folder details page for the synced folder opens in <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span>. This page contains information about the folder. <br>This page also lets you pause and disable the sync. If you pause the sync, the folder will no longer be updated with the changes from Box, but the sync can be resumed at any time. Disabling the sync means that the connection between the folders is broken and the sync would need to be re-established from the Box account.<br>The Folder details page contains the following information and functions in relation to your folder in Box:  <ul>  <li><span class="bold">Pause syncing</span>: The <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> folder will no longer be updated with the changes from Box. Sync can be resumed at any time (1).</li>  <li><span class="bold">Disable folder sync</span>: Connection between folders is lost, and the sync will have to be setup again from the Box account (2).<br></li><note type="note">   &nbsp;Only the user who started the folder sync can disable or pause it. For more information, see&nbsp;   <a href="manage-folders-and-contents.md" class="MCXref xref">Manage Folders and their Contents in Workfront Proof</a>.  </note>  <li><span class="bold">Go to Box folder</span>: If you shared the folder URL (in the Box folder options), this option will become available and will take you straight to the Box folder (3).</li>  <li><span class="bold">Folder sync details</span>: This section contains information about the Box folder (4).</li>  <li><span class="bold">Box folder link</span>: URL to the Box folder (5).</li>  <li><span class="bold">Activity:</span> Shows you the activity logs of the <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> folder, here you can check who started the folder sync (6).</li>  <p><img src="assets/folder-details--1--350x324.jpg" alt="folder_details__1_.jpg" style="width: 350;height: 324;"></p> </ul></li>` 





>[!NOTE]
>
>
>
>
>* You can also sync the Box folder from the Folder options menu. 
>* If you have your own branded *`Workfront Proof`* login page, you will be taken to that page instead of the standard *`Workfront Proof`* login page. See the articles under [Branding](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) if you need more information. 
>
>* If you have enabled the Single Sign-On (SSO) functionality in your *`Workfront Proof`* account, you will be taken to the SSO login page and asked to enter your SSO login credentials, but only if you are are using the same email address for your Box account and *`Workfront Proof`*. If you need more information, see [Single Sign-On in Workfront Proof](single-sign-on-overview.md).
>
>* If you are not using the same email address for both your Box account and your *`Workfront Proof`* account, you will always be taken to the standard *`Workfront Proof`* login page. 
>
>
>



