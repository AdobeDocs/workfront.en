---
product-area: resource-management
navigation-topic: resource-planning
title: Share the Resource Planner User View with a Link
description: Adobe Workfront can generate a unique URL for the User View of the Resource Planner which you can embed into a dashboard as an External Page, or open it separately in a new browser tab. This is helpful when sharing the Resource Planner information with users who might not have direct access to the Resourcing area.
author: Lisa
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
TQID: https://experienceleague.adobe.com/C6VONkwVFolewhXNwvuYv4WWMx6Ee5v6w9vEgFPgUow
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource Management
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
    internal-label: Resource Planner
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Share the Resource Planner user view with a link

Adobe Workfront can generate a unique URL for the User View of the Resource Planner which you can embed into a dashboard as an External Page, or open it separately in a new browser tab. This is helpful when sharing the Resource Planner information with users who might not have direct access to the Resourcing area.

![User view with link](assets/rp-user-view-with-link-highlight-350x49.png)

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>View or higher access to Resource Management, Projects, and Users</p> <p>View access to Financial Data that includes access to View Cost Rates and View General Finance, to view cost information</p></td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td> <p>View or higher permissions to the projects you want to display in the Resource Planner</p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

Consider the following when generating the unique URL for the User View of the Resource Planner:

* You can obtain a unique URL only for the User View. The option to generate the URL does not exist in the Project or Role Views. 
* You can share the URL with other users, including Work, Contributor, and Review licensed users.   
  They must have access to view other users in order to view the information in the Resource Planner from the URL that you share with them. 
* The following information is saved when you share the URL with other users:

   * The type of time periods (week, month, quarter).
   * The filters that you apply.
   * The type of display (Hours or FTE).

To obtain a unique URL in the User View of the Resource Planner and share it with other users:

{{step1-to-resourcing}}

1. Select **View by User**.
1. (Optional) Select the timeframe by which you want to view the information in the Resource Planner. Select from the following:

   * Week
   * Month
   * Quarter

1. (Optional) Select whether you want to view the information by **FTE** or **Hours**.  
   ![Select FTE or Hours](assets/rp-hours-or-fte-in-user-view.png)

1. (Optional) Apply filters to the Resource Planner.  
   For information about applying filters, see [Filter information in the Resource Planner](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

1. Click the **hyperlink** icon.  
   ![Hyperlink icon and URL](assets/rp-generate-url-from-link-icon.png)

1. Click **Copy URL**.  
   This copies the unique URL of the Resource Planner in the User View to your clipboard. 

1. (Optional) Do one of the following:

   * Paste the URL into another application to send it to another user.  
     The user must be logged in to Workfront to view the Resource Planner in the User view.
   * Open a new browser tab or window and paste the link you copied, then click Enter on your keyboard to open the Resource Planner in a new tab or window. 
   * Do the following:   
   
     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. Go to **Reporting**>**Dashboards**>**New Dashboard**>**Add External Page.**
      
      1. Paste the link you copied to your clipboard in the **URL** field.
      1. Click **Save**, then **Save + Close**.  
         This will embed the URL into the dashboard and the User view of the Resource Planner displays in a separate dashboard.

1. (Optional) If you embedded the URL into a dashboard, consider adding it to a layout template or sharing it with other users who might not have access to the Resource Management area.  
   For information about adding dashboards to a layout template, see [Create and manage layout templates](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) .   
   For information about sharing dashboards, see [Share a dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) .   
   When viewing the shared URL, users can see the information with the settings that you originally applied to the Resource Planner. They must be logged in to Workfront to view the shared URL.  
   ![Sample dashboard with Resource Planner displayed](assets/user-view-dashoard-from-unique-url-350x85.png)
