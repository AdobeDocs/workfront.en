---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: Share a Canvas Dashboard
description: You can share a Canvas dashboard with other Adobe Workfront users so that they can view or edit it.
author: Jenny
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
---
# Share a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. Parts of the feature may not be complete or work as intended during this stage. Please submit any feedback regarding your experience by following the instructions in the [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) section in the Canvas Dashboards beta overview article.<br>
>If you have feedback regarding a possible bug or technical issue, please submit a ticket to Workfront Support. For more information, see [Contact Customer Support](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Please note that this beta is not available on the following cloud providers:
>
>* Bring Your Own Key for Amazon Web Services
>* Azure
>* Google Cloud Platform 

You can share a Canvas dashboard with other Adobe Workfront users so they can view or edit it.

## Access Requirements

+++ Expand to view access requirements for the functionality in this article.
 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td> 
<p>Standard </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configurations</p></td> 
   <td><p>View access to Reports, Dashboards, and Calendars</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td><p>View permissions for the dashboard to share the dashboard</p>
   <p>Manage permissions for the dashboard to assign dashboard permissions</p>
  </td> 
  </tr>
</tbody> 
</table> 

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Considerations about sharing dashboards

* Dashboards can be shared to user, team, group, job role, or company resources.

* By default, the creator of a dashboard has Manage permissions for the dashboard. 

* System administrators and users with Manage permission can grant View or Manage access to a dashboard.

* Users with View permission to a dashboard can grant View access to a dashboard. 

* When sharing a dashboard, the resources it's shared with will inherit permissions to the reports displayed on the dashboard.

* When a dashboard is distributed through a layout template, an automatic View permission for the dashboard (and its reports) is granted to all resources assigned to the layout template.


## Share a Canvas Dashboard


{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 

1. On the **Canvas Dashboards** page, select the dashboard you want to share. 

1. In the upper-right corner of the page, click the **Share** button. The **Dashboard Sharing** dialog box appears.

1. In the **Give access to** field, begin typing the name of a specific user, team, role, group, or company you want to share the Canvas Dashboard with, then select it when it appears in the drop-down list. 

1. (Optional) To edit a resource's access to the dashboard, click **View** next to their name, then select **Manage** in the drop-down list that appears. 

    >[!NOTE]
    >
    > When users do not have the Edit permissions to a dashboard assigned through their access level, they cannot be assigned Manage permissions to a dashboard.

1. Repeat steps 5-6 for each resource you want to share the dashboard with.

1. Click the **Share** button. The recipients receive an email notification informing them that the dashboard has been shared with them, which they can now access at **Dashboards** > **Canvas Dashboards** > **Shared Dashboards**. 

    >[!NOTE]
    >
    > Individual user preferences and system exclusions for email notifications may apply. <br>
    > Notifications are only sent when shared directly with a user. Sharing to groups, roles, companies, and teams do not generate email notifications.<br>
    > Permissions inherited from a layout template will not generate an email notification about the access to the dashboard.
