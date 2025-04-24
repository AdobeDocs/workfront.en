---
title: Manage Record Comments
description: You can collaborate on Adobe Workfront Planning records, by adding comments or replies in the right panel of a record. You can also view other changes made to the record and recorded by the system in this area.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
---
# Manage record comments

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can collaborate on Adobe Workfront Planning records, by adding comments or replies in the right panel of a record. You can also view other changes made to the record and recorded by the system in this area.

The right panel of a record displays the following sections:

* **Comments**: Displays comments and replies users add to records.
* **History**: Displays system-recorded changes that users  make to the record fields. For more information, see [History section overview](/help/quicksilver/planning/records/history-section-overview.md).

## Access requirements

+++ Expand to view access requirements.. 

You must have the following access to perform the steps in this article:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Contributor or higher license</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace <span class="preview">and record type</span> </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

<!--replace the layout template info in the table with this at release: 

<div class="preview">
<p> Users with a Light or Contributor license must be assigned a layout template that includes the Planning option  in the following areas:</p>
   <ul><li>Main Menu</li>
   <li>Left panel of projects, portfolios, and programs</li>
   <li>Landing page</li>
   <li>Pins</li></ul>
   <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Create and manage layout templates</a>.</p>
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div>
   <p><b>NOTE</b></p>
   <p>In the Production environment, all users including the System administrators must be assigned to a layout template that includes the Planning areas.</p>

--> 

## Considerations about commenting on a record

* You can add comments and replies to records in Workfront Planning, in the Comments section of a record. 

* Comments added to linked records do not display on the records you are linking from. For example, if you comment on a Workfront Planning Product record that is linked to a Campaign record, the comment displays only on the Product record in Workfront Planning and not on the Campaign record from which you are linking. 

* You can add comments to Workfront Planning records created as a result of a connection between a record and an object from another application. 
   
   For example, you can comment on the Project Workfront Planning record after you connect Workfront projects with Workfront Planning records. For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

* Comments added to linked objects in other applications do not display in Workfront Planning and comments added to linked objects in Workfront Planning do not display in other applications.  
   
   For example, comments added to projects in Workfront do not display on the same project linked to a campaign in Workfront Planning, and comments added to the project Workfront Planning record don't display in Workfront. 

* You can tag users to bring their attention to an update. Tagged users do not receive an in-app notification or an email about your update. <!--this might change??-->

* You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   
   >[!NOTE]
   >
   >   Only users from customers who have onboarded with the Adobe Unified Experience receive both an in-app notification and an email notification. To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      
* You can add an update to records and review the history of changes from the following areas of Workfront Planning:

   * From the record details page. 
   * From a view, in the record details box.

### Manage comments on records

{{step1-to-planning}}

1. Click the card of a workspace. 

    The workspace opens and the record types display on cards. 

1. Click a record type card.
    The record type page opens and all records of that type display. 
     
1. Choose a table view from the **View** drop-down menu.
1. Click the name of a record in the table view. 

    The record's **Details** page opens. The Comments area opens by default in the right panel. 

1. (Conditional) If the right panel does not open by default, click the **Show Comments** ![Show comments icon](assets/show-comments-icon.png) icon in the upper-right corner to open the Comments section. 

1. Start entering a comment in the **New comment** box. 
   
   ![Empty comment box on record](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Navigating away from the Comments section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. <!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. (Optional) To undo or redo a change, use the following shortcut keys:
      * CTRL + Z (⌘+z for Mac) to undo a change 
      * CTRL + Y (⌘+y for Mac) to redo a change 
1. (Optional and conditional) If your Workfront instance is part of the Adobe Unified Experience, add **@** followed by the name of a user to tag someone in the update. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article.

1. (Optional) Use the options in the Rich Text toolbar to format your text, add emojis, or links to your update, to enhance your content. 

   >[!TIP]
   >
   >You cannot add images to a record comment.


1. Continue adding comments to the record. 

   For more information about updating objects, including Workfront Planning records, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Delete** to delete the comment. 
1. (Optional) Click the **Hide Comments** icon ![Hide comments icon](assets/hide-comments-icon.png) to close the right panel. 

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![New line indicator in comments](assets/new-line-indicator-comments.png)
1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.
   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  
1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.
1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     
   ![Search box for comments](assets/search-box-for-comments-area.png)
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ...** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.
   ![New comments banner on record](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 
    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

## History section overview

You can review the changes made to the record in the History section of the right panel of a record. 

For more information, see [History section overview](/help/quicksilver/planning/records/history-section-overview.md).
