---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configure whether time is logged in hours or days
description: As a user with a Plan license, you can configure whether you log time in Adobe Workfront in hours or days. System administrators can configure this setting for individual users or for multiple users in their organization. By default, users log time in hours.
author: Lisa
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
TQID: https://experienceleague.adobe.com/2rLb--26SLkI7t0tpdShzxdVxhCLJEdzWYGBO8DOJSE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Configure whether time is logged in hours or days

As a user with a Standard or Plan license, you can configure whether you log time in Adobe Workfront in hours or days. System administrators can configure this setting for individual users or for multiple users in their organization. By default, users log time in hours. For information about how to log time in Workfront, see [Log time](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>We recommend logging time in the same way, either hours or days, across the organization to ensure reporting accuracy.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td><p>Standard and Plan users can configure time for themselves. Only a Workfront administrator can configure time for other users.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

1. Do either of the following, depending on your objective and your access level in the system:

   * **Standard or Plan user configuring time logging for yourself:** Click your profile picture in the top navigation area, then click **[!UICONTROL Workfront Profile]**. Then, click the **More** icon next to your name and select **Edit**.
   
   * **System administrator configuring time logging for others:** Begin editing one or more user accounts, as described in [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. In the user profile dialog box, in the **Resource Planning** section, locate the **Log time in** option.

   ![Log time in options](assets/user-profile-log-time-options.png)

1. Select from the following options for logging time: 

   | Option |Description |
   |---|---|
   | **Hours** | Users specify hours when logging time in Workfront. |
   | **Days** | Users specify days when logging time in Workfront. |

1. (Conditional) If you selected to log time in days, in the **Equivalent Hours for Full Workday** field, type the number of hours that equal a full day. One day on a user's timesheet is the equivalent of the number of hours you enter here.

   Consider the following when configuring this setting:

   * This option is not available when configuring to log time in hours.
   * This option is used only for the purpose of logging time. This option is not related to the **Schedule** option that is also available when editing a user. The **Schedule** option is used when calculating timelines and in other areas of Workfront. (For more information about using the **Schedule** option, see [Create a schedule](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)&nbsp;

1. Click **Save Changes**.
