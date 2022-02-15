---
filename: home-groups
title: Home Groups
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
---




# Home Groups {#home-groups}

A Home Group is assigned in the user's profile. All users are required to have a Home Group. A user can belong to more than one group, but they can have only one Home Group. For more information about Groups, see [Groups](groups.md).


Although any existing group in the system can be assigned as a user's Home Group, we recommend creating and assigning new groups that represent larger organizational units.


When establishing Home Groups, consider how your organization divides your `Workfront` users. Here are a few suggestions to determine what type of groups should be used as a Home Group:



* Groups that represent departments, such as IT or Marketing
* Groups governed by different budgets
* Groups located in different areas or regions
* Groups made up of multiple teams that belong to the same cost center




>[!NOTE]
>
>If you need to reorganize your Home Groups into organizational units, you need to>
>
>
>1. Create the new group, as explained in [Create and manage groups](create-manage-groups.md).
>1. Reassign the new group as the user's Home Group, as explained in [Edit a user's profile](edit-a-users-profile.md).
>
>





## Layout Template management {#layout-template-management}

When you assign a Layout Template to a group, all users that have the group assigned as their Home Group can see the settings specified in the Layout Template.


If a Layout Template is assigned to a Home Group, it is only visible to users assigned&nbsp;to that Home Group.


For more information, see [Create and manage Layout Templates](create-and-manage-layout-templates.md) in [Create and manage Layout Templates](create-and-manage-layout-templates.md).


## License management {#license-management}

Because users can be assigned only one Home Group, this makes them easy to use for controlling license counts.&nbsp;


`Workfront administrator`s have the option to set maximum license counts for the Home Groups.


Setting a max license count allows system administrators to prevent a business unit from using `Workfront` licenses purchased for other business units.


For more information, see the article&nbsp; [Manage available licenses in your system](manage-available-licenses-in-your-system.html.md).
