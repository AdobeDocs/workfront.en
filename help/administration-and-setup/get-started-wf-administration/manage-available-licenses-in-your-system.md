---
filename: manage-available-licenses-in-your-system
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Manage available licenses in your system
description: As an Adobe Workfront administrator, you can access information about your Workfront account, including the number of licenses purchased for your organization, as well as the number of those licenses currently in use.
---

# Manage available licenses in your system

As an Adobe Workfront administrator, you can access information about your Workfront account, including the number of licenses purchased for your organization, as well as the number of those licenses currently in use.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## View your organization’s licenses

The number of used licenses in use updates automatically as you assign access levels to users you add to Workfront. For more information, see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

To view license information in your system:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>At the bottom of the left panel, click <span class="bold">System</span> > <span class="bold">Licenses</span>.</p> <p>For more information about the licenses listed on this page, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> <note type="note">
    Proof licenses are available only to customers who have purchased the paid Workfront Proof add-on in addition to their Workfront license. For information about this add-on, see 
   <a href="../../workfront-proof/workfront-proof.md" class="MCXref xref">Workfront Proof</a>.
  </note> </li> 
 <li value="3">(Conditional) If you see the message <span class="bold">To set a maximum, you must add a Home Group</span>, add a Home Groups in your system as explained in the section <a href="#managing-the-group-list" class="MCXref xref">Add or remove a Home Group to the Licenses page</a> in this article.</li> 
</ol>

## Viewing information about licenses for Workfront addons

In the screen shot below, `5 of 10 Proof licenses` indicates that this organization has the paid Workfront Proof add-on and is currently using 5 of the 10 Workfront Proof licenses they purchased.

![](assets/license-count-paid-add-on-350x233.png)

If your organization has purchased Workfront Goals, the license information for this product also displays here. In this case, you can view the following information: The total number of Workfront Goals licenses that your company has purchased The number of Workfront Goals licenses associated with users. This is the number of users to whom to have granted at least View access to Goals in their access level. For information about Workfront Goals, see Adobe Workfront Goals overview. For information about access to Workfront Goals, see Grant access to Adobe Workfront Goals Note: Workfront allows you to assign more Workfront Goals licenses that you have purchased. However, when you assign more licenses than what your Workfront Goals contract allows, a Workfront account manager will contact you to let you know that you have exceeded your contractual number. 

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn’t have any paid add-on products, nothing displays here.
-->

` `**Tip: **`` Users without administrative access can use a Group report to view license count. In the Report tab, create a new group report and add the following columns:

* License Type Limit: Worker Limit
* License Type Limit: Planner Limit&nbsp;

To learn more about creating a report, see [Create a custom report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Add or remove a Home Group to the Licenses page

A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)

Each user can be assigned to only one Home Group. Workfront provides a group-oriented license count by calculating how many licenses are allocated and currently used in each Home Group.

If you see the message `To set a maximum, you must add a Home Group` on the Licenses page, you need to add at least one Home Group to the Licenses page.

>[!IMPORTANT]
>
>* To effectively manage licenses with home groups, we recommend setting up specific Home Groups for business units before updating the max license count. For more information, see [Home Groups overview](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* You can add only top-level groups as Home Groups, not subgroups. If a user has a subgroup assigned as their Home Group, their license is added to the license count for the top-level group above that subgroup.
>

To add or remove a Home Group to the Licenses page:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">At the bottom of the left panel, click <span class="bold">System</span> > <span class="bold">Licenses</span>.</li> 
 <li value="3">Click <span class="bold">Manage Group List</span>.</li> 
 <li value="4"> Start typing the top-level group’s name in the <span class="bold">Home Groups</span> box.</li> 
 <li value="5"> <p>To add the group, click its name when it appears.</p> <p>Or</p> <p>To remove the group, click the X icon to the right of its name.</p> </li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

As a Workfront administrator, you can set maximum license counts for the Home Groups to prevent a business unit from using Workfront licenses purchased for other business units. For instructions, see [Set the maximum license count for a Home Group](#set) in this article.

## Set the maximum license count for a Home Group

As a Workfront administrator, you can set maximum license counts for the top-level Home Groups in your system. This allows you to prevent a business unit from using Workfront licenses purchased for other business units within your organization.

By default, the max license count is set to N/A, which means there is no limit.
group administrators can view the number of licenses allocated and used in a Home Group they manage. For more information, see View the number of licenses allocated and used in a group in the new Adobe Workfront experience. 

To set the maximum license count for a Home group:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">At the bottom of the left panel, click <span class="bold">System</span> > <span class="bold">Licenses</span>.</li> 
 <li value="3">Locate the Home Group in the list.</li> 
 <li value="4">In the <span class="bold">Max</span> column of the group, click the value that you want to set a maximum for.</li> 
 <li value="5"> <p>Type the maximum number, then press Enter.</p> <p> <img src="assets/screen4-350x152.png" alt="Screen4.png" style="width: 350;height: 152;"> </p> <note type="note">
    To set a group's maximum license value back to the default, do not type 0. Instead, delete the number in the box. Setting the maximum license value to 0 indicates that there are no licenses allocated to that group.
  </note> </li> 
</ol>

