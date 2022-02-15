---
filename: modify-email-notification-settings-user-profiles
user-type: administrator
product-area: system-administration
keywords: modify,email,notification,settings,bulk,bulk-edit,configure,multiple,users
navigation-topic: emails-administration
---



# Modify email notification settings in users’ profiles {#modify-email-notification-settings-in-users-profiles}

If you are an *`Adobe Workfront administrator`* or you have a Planner access level allowing you to edit other users' settings, you can configure the notification settings for multiple users at one time. This includes specifying whether users receive notifications as events happen, or in one daily digest email, as described in [Adobe Workfront notifications](wf-notifications.md). For information about the access level needed to edit users, see [Grant access to users](grant-access-other-users.md).


When you configure notification settings in bulk, you can change only the settings that the selected users have in common.


You can also configure email notifications for one user at a time. For more information, see [Activate or deactivate your own event notifications](activate-or-deactivate-your-own-event-notifications.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your *`Workfront administrator`*.


## Modify the email notification settings of multiple users in bulk {#modify-the-email-notification-settings-of-multiple-users-in-bulk}




1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Users</span>. Select the users, then click  <span class="bold">Edit</span>.</MadCap:conditionalText>` 
1. In the `Edit Person` box that appears, click `Notifications`.

1.  Expand a category to view notification settings related to that category.  



   If there is at least one user selected where the notifications do not match the notifications of the other selected users, the category check box for that notification contains a horizontal line ![](assets/straight-line-instead-of-checkmark.jpg) instead of a check mark.  


1.  Click any notifications that you want the users to receive either daily or instantly, or clear any that you want them to stop receiving.   



   For the `Communication` category, you can select individual notifications for instant delivery only. You must select all of the notifications to be delivered in a daily digest.


   When you modify a notification setting, the label `Edited` appears for that notification setting, to let you know that that notification setting has been modified.

1.   If you selected notifications to be sent as a daily digest, select the time of the day you want the digest delivered at the top of the `Notifications` section in the `Email Daily Digest after` menu.


   After you select a delivery time, the `Email Daily Digest after` box displays with an orange frame to indicate that the time of the delivery has been edited.


   The daily digest includes events that meet the criteria of the notifications 24 hours prior to the selected time. Users receive one daily digest email for each notification type.


   The daily digest may arrive after the time you select, depending on how many emails are queued for delivery in the system. The time listed is your local time as specified in your browser settings.



