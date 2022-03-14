---
filename: manage-items-on-views-page
product: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Manage Items on the Views Page in Workfront Proof
description: The Views page allows you to see and work with all of your proofs, files and folders in one place.
---

# Manage Items on the Views Page in Workfront Proof

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

The Views page allows you to see and work with all of your proofs, files and folders in one place.

## Displaying the Views Page

1. Click `Views` in the left sidebar.
1. From the drop-down menu (2), click the view (3) you want to see.

![Views.png](assets/views-350x297.png)

## Changing the Views Page Layout

The default Views page layout is the Thumbnail list. In this layout, you can see a miniature image of each proof, file (if possible to generate), and folders (if set), with other details included in separate columns.

1. Click the `Page Layout` icon (1), then choose the layout you want.

![Views_Page_Layout.png](assets/views-page-layout-350x140.png) 

## Changing the Views List

To change what you see in the Views list:

1. Click the  `Change view` button.  
   The name appearing on this button depends on the view you selected the last time you used it.  
   ![Views-Chnge_view_button.png](assets/views-chnge-view-button-350x205.png)

1. Click a different view in the drop-down menu:

  * `All items`: Includes all proofs, files and folders that you have permission to see. It is the default when you open the Views page. You have the option to include/exclude archived proofs in this view.
  * `Active items`: All active proofs, files and folders.
  * `Active proofs`: All active (not archived) proofs that you have permission to see.
  * `Locked proofs`: Only locked proofs.
  * `Archived proofs`: Only archived proofs (see [Archive in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/archive.md)).
  
  * `My Proofs`: Shows only proofs for which you are the owner and that are delegated to you. For more information, see&nbsp; [Designating Temporary Proof Owners in Workfront Proof](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
  
  * `Proofs awaiting decision`: Shows only proofs on which you have to make a decision&nbsp;
  * `Late proofs`: Shows only proofs for which the deadline has passed
  * `Files`: Shows only files

   In each of these views, the following columns are included

  * `Type`: Icon of the item with the icon of proof, file or folder
  * `Name`: Name of the proof, file or folder
  * `Progress`: S=Sent, O=Opened, C=Comment, D=Decision (see Progress Bar)
  * `Status`: Pending, Changes required, Approved
  * `Decisions`: Number of decisions made and number required
  * `Owner`: Name of the person who owns the proof  
    My proofs, Proofs awaiting decision and Late proofs views have an additional column called My deadline. This column displays your own deadlines on the proofs where you are explicitly added as a Reviewer/Approver.

    >[!NOTE]
    >
    >&nbsp;If you navigate away from the Views page and return to it later in the same session, your last selected view appears.

    You can also create your own views. See&nbsp; [Create and Manage Custom Views in Workfront Proof Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md) for more information.

## Filtering Items

You can filter the information listed in a view.

1. Click the `Show filters`&nbsp;icon at the right top of the page (1).  
   ![Filters.png](assets/filters-350x107.png)

1. The filter bar (2) appears and each category has a filtering drop-down menu (3) to select your preferred value. The default value for each category is All.  
1. &nbsp;The filter bar does not display in custom views you create. For those views,&nbsp;you can apply and edit filters in the Filters tab. For more information, see [Create and Manage Custom Views in Workfront Proof Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
1. To apply all chosen filters, click the Filter icon (4) at the end of the filtering bar.  
   ![Filters_2.png](assets/filters-2-350x102.png)

The Filter values you select remain in effect until you change them. If you want to see and access the full list of items again, you must change all the filter values back to the default, which is `All`.

>[!NOTE]
>
>&nbsp;If you set filtering options and then hide the filtering bar by clicking the Hide filters icon (5), the bar automatically shows again if you change views. If you hide the filtering bar while all filters are set to the default all option, the filtering bar remains hidden when changing views.

## Sorting Items

When you create a new proof (or version) or upload a new file, it appears at the top of your All items list. The oldest item appears at the bottom of the list.&nbsp;

To view the list in a different sort order:

1. Do one of the following:

  * Click one of the column headings in the list: Type, Name, Status, Decisions, or Owner.   
    For example, if you want to see the proofs/files in alphabetical order, click the Name heading once (1) to sort the list by name in ascending order (A - Z).  
    You can click the Proof name heading again (2) to reverse the order and display the proofs in descending order (Z - A).
  
  * Click the down arrow in the upper-right of the Views page to sort by the creation date (Latest or Oldest) or by Type, Name, Status, Decisions, or Owner.  
    ![Views-Sort_down_arrow.png](assets/views-sort-down-arrow-350x124.png)  
    If your column is sorted in ascending order the column header will show an upward arrow next to the column name. To reverse the order (to descending) click the relevant column header (this will show a downward arrow next to the column name).  
  
  * &nbsp;Changes that you make to the sort order of the items last only while you remain on the All items page. If you navigate away from the All items page and return to it later, the items are listed again in the default reverse chronological order.

## Viewing a Proof Summary

To view more detailed information about a proof:

1. Click the arrow to the left of the proof image.   
   The arrow points down and the Proof summary displays below the basic information about the proof. The Proof summary shows:

  * `Proof summary`: Overall status of the proof
  * `Stage`: Indicates the proof deadline and number of decisions made and required
  * `Reviewers`: Name, role and progress of each reviewer will be listed
  * `Versions`: Version of the proof being viewed and the total number of versions available
  * `Folder`: Folder in which the proof is located
  * `State`: Active, Locked, Draft, or Submitted

1. (Optional) If you have edit rights on the proof and the proof has stages, click the `More` (three dot) menu to the right of the stage to access the following options:

  * `Message all`: Send an email to all reviewers on the stage.
  * `Share`: Add new reviewers
  * `Delete stage`

1. (Optional) Click a reviewer's `More` (three dot) menu to the right of their name to do any of the following:

  * Send the reviewer a reminder message.&nbsp;
  * Edit the Reviewer's settings on the proof.   
    The Edit reviewer box that appears, you can change not only role and email alerts but also the Display Name for the Reviewer. Note that the Display Name can be changed only on the particular proof, not in the reviewer's details in the Contacts page. See [Contacts](https://support.workfront.com/hc/en-us/sections/115000920808-Contacts) for more information.
  
  * Select the reviewer to be the Primary Decision Maker on the proof.
  * Delete the reviewer from the proof.  
  * &nbsp;You can also change the Role and Email alerts for a reviewer added to the proof.

## Including and Excluding Archived Proofs

The All Items view by default displays all active and locked proofs, files and folders. It also provides the option to include or exclude archived proofs in the view.   
To include the archived proofs:

1. When you choose a view, click `Include archived proofs`.  
   ![Views-include_archived_proofs.png](assets/views-include-archived-proofs-350x188.png)  
   Archived proofs will appear with an archived icon to distinguish them from other proofs.  
   ![Views-Archived_icon.png](assets/views-archived-icon.png)

## Opening an Item From a List View

1. Do one of the following:

  * To view details about a proof, file or folder, click its name.
  * To open a proof into the proofing viewer, click `Go to Proof`.  
    For information about the proofing viewer, see [Review a proof](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## Performing Actions on Multiple Items

To select multiple items:

1. Click the checkbox above the list.  
   ![Views-select_all_items_checkbox.png](assets/views-select-all-items-checkbox-350x193.png)

1. In the extra options that appear above the Views list, do any of the following to the files you have selected:

  * Click on `Tags`&nbsp;to add a tag to these items.
  * Click on `Move to` to move the selected items to a different folder (or move the items out of the folder if you select (No folder selected).
  * Click `Share selected items`&nbsp;to share all of these items with additional reviewers.  
    ![Share_button-small.png](assets/share-button-small.png)

  * Click `Delete`&nbsp;to move the selected items to the Trash.  
    ![Trash_button.png](assets/trash-button.png)

  * Click the `More` menu for additional actions available.  
  
  * The actions will be applied only to those of the selected items that have the particular option available. For example if you select files and proofs and choose Lock, only the proofs will be locked (because you cannot lock files)

## Moving an Item to a Folder

If you have the edit rights to do so, you can move proofs, files and folders to specific folders on the Views page.&nbsp;

1. Open the folder tree in the sidebar by clicking the arrow to the left of your top-most folder.
1. Do one of the following:

  * To move one item, click and hold it, dragging and dropping it to the folder where you want to put it.
  * To move multiple items at the same time, you can select the check boxes to the left of the items, then click `Move to`&nbsp;above the list, then select the folder where you want to put them, or create a new folder for them.

