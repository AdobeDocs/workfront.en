---
filename: subgroups
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
---




# Subgroups {#subgroups}

You can create a subgroup by adding an existing group as a member of another existing group, or you can create a new subgroup from scratch. For instructions, see `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <a href="create-view-manage-subgroups.md" class="MCXref xref" xrefformat="{para}">Create, view, and manage subgroups in the new Workfront experience</a></MadCap:conditionalText>`.


## Objects inherited by subgroups {#objects-inherited-by-subgroups}

Subgroups inherit the membership of their parent group. So, users and groups in a subgroup have the same visibility, permissions, and access to all objects as users and groups that belong to the parent group they share.

` `**Tip: **`` Sometimes, you might want to use subgroups to add multiple users to an existing group in order to give them access to an object they need.


For example, suppose that you have a group of help desk technicians and a separate group of IT directors. The help desk group has permissions to a certain Request Queue. You want to add the IT directors to the help desk group so that they also have permissions to the Request Queu. Without the subgroup functionality, you would have to add the IT directors to the help desk group manually, which could be inefficient and hard to manage. If you add the IT directors group to the help desk group as a subgroup, you accomplish this task faster with just one change.


>[!NOTE]
>
>If a user was added to both a subgroup and to its parent group separately, removing the user from one doesn't remove the user from the other. If you don't want the user to have the access allowed for the parent group, you must remove the user both from the subgroup and from the parent group.




## Levels of subgroups {#levels-of-subgroups}

As a `Workfront administrator` or a `Group Administrator`, you can create `up to 14 levels of subgroups under 1 group.` On any one of these levels, you can create an unlimited number of parallel subgroups.


## Public and private subgroups {#public-and-private-subgroups}

For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.


You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.


If you create a subgroup under a group that is public, the subgroup is also public, by default. For more information about creating a group and making it public, see [Create and manage groups](create-manage-groups.md). For more information about the access needed to edit users, see [Grant access to users](grant-access-other-users.md).


Any group you add to an existing group automatically becomes a subgroup and is no longer a main group. However, the subgroup retains its existing users, as well as any associations with projects, issues, and tasks, in addition to all project, task, and issue statuses that belong to the new parent group.
