---
title: Manage record comments 
description: You can collaborate on Adobe Maestro records, by adding comments or replies in the Comments area of a record.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---

# Manage record comments

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> 

You can collaborate on Adobe Maestro records, by adding comments or replies in the Comments area of a record.

## Considerations about commenting on a record

* You can add comments and replies to operational records and taxonomies in Maestro, in the Comments section of a record. 

* Comments added to linked records do not display on the records you are linking from. For example, if you comment on a Maestro Product record that is linked to a Campaign record, the comment displays only on the Product record in Maestro and not on the Campaign record from which you are linking. 

* You can add comments to Maestro records created as a result of a connection between a Maestro record and an object from another application. 
   
   For example, you can comment on the Project Maestro record after you connect Workfront projects with Maestro records. For more information, see [Connect records](/help/quicksilver/maestro/records/connect-records.md). 

* Comments added to linked objects in other applications do not display in Maestro and comments added to linked objects in Maestro do not display in other applications.  
   
   For example, comments added to projects in Workfront do not display on the same project linked to a campaign in Maestro, and comments added to the project Maestro record don't display in Workfront. 

* You can tag users to bring their attention to an update. Tagged users do not receive an in-app notification or an email about your update. <!--this might change??-->
   
* You can add an update to records from the following areas of Maestro:

   * From the Details page.

   <!--* From the table view.-->

## Access requirements

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Maestro. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### Manage comments on records

{{step1-to-maestro}}

   The last accessed workspace opens by default. 
1. Choose a table view from the **View** drop-down menu.
1. Click the name of a record in the table view. 

    The record's **Details** page opens. The Comments area opens by default in the right panel. 

1. Start entering a comment in the **New comment** box. 
   
   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Navigating away from the Comments section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.

1. (Optional) To undo or redo a change, use the following shortcut keys:
      * CTRL + Z (⌘+z for Mac) to undo a change 
      * CTRL + Y (⌘+y for Mac) to redo a change 
1. (Optional) Add **@** followed by the name of a user to tag someone in the update.  
1. (Optional) Use the options in the Rich Text toolbar to format your text, add emojis, links, or images to your update, to enhance your content. For more information, see the "Use Rich Text in a Workfront update" section in the article [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![](assets/new-line-indicator-comments.png)

1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.

   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  

1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
   
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.

1. <span class="preview">(Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.</span>     

   <span class="preview">![](assets/search-box-for-comments-area.png)</span>
     
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ...** area, to reply to an existing comment, then follow steps 4-8 above. <!--(**************accurate??***********)-->  

1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.

    ![](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
  
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 

    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body tex**t: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 
1. (Optional) Click the **More** icon ![](assets/more-menu.png) in the upper-right corner of the comment, then click **Delete** to delete the comment. 

