---
title: View the Number of Licenses Allocated and Used in a Group
description: As an Adobe Workfront administrator, you can view counts of the individual types of licenses currently used in your group and its subgroups. This is useful when you need to assess whether to redistribute licenses.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
---
# View the number of licenses allocated and used in a group

As an Adobe Workfront administrator, you can view counts of the individual types of licenses currently used in your group and its subgroups. This is useful when you need to assess whether to redistribute licenses.

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

>[!IMPORTANT]
>
>A user's license is counted in a particular group only if the group is the user's Home Group.

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
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Access level configurations</td> 
   <td>You must be a group administrator of the group or a system administrator.</td>
  </tr>
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## View the number of licenses used in a group

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![Groups](assets/groups-icon.png).

1. Click the name of the group.
1. On the page that displays, in the header area near the upper-right corner, view the **Licenses in use** area to see the number of **Plan** and **Work** licenses currently being used.

   If you are viewing a top-level group and the Workfront administrator defined a maximum number of each license type for the group, these numbers are also displayed. For example, in the group below, a maximum of 10 users can have a Plan license and a 15 can have a Work license:

   ![Allocated licenses](assets/licenses-used-allocated.png)

   For information about how a Workfront administrator defines a maximum number of allocated licenses for a group, see the section [Set the maximum license count for a Home Group](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) in the article [Manage available licenses in your system](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >If the group you are looking at is a subgroup, you can view only the numbers of licenses being used, not the maximum number of licenses allocated for the group. This is because Workfront administrators do not define a maximum license count for a subgroup.
   >
   >![Used licenses in subgroup](assets/subgroup-used-licenses-only.png)
   >

1. For separate counts of each type of license currently used in the group (including Review and Request), click the text area directly below **Licenses in use:**

   ![Click to see more](assets/click-text-to-see-more.png)

   The box that displays provides the same information for all four Workfront license types: Plan, Work, Review, and Request. At the bottom of the box, you can see the total number of licenses being used by members of this group or one of its subgroups:

   ![More license information](assets/more-license-info.png)

   For Review and Request licenses, the Max column always displays Unlimited.
