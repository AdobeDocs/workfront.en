---
filename: config-time-logged-hrs-days
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configure whether time is logged in hours or days
description: As a user with a Planner license, you can configure whether you log time in Adobe Workfront in hours or days. System administrators can configure this setting for individual users or for multiple users in their organization. By default, users log time in hours. For information about how to log time in Workfront, see Log time.
---

# Configure whether time is logged in hours or days

As a user with a Planner license, you can configure&nbsp;whether you log time in *Adobe Workfront* in hours or days. System administrators can configure this setting for individual users or for multiple users in their organization. By default, users log time in hours. For information about how to&nbsp;log time in *Workfront*, see [Log time](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>We recommend logging time in the same way, either hours or days, across the organization to ensure reporting accuracy.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>Planners can configure time for themselves. Only a <em>Workfront administrator</em> can configure time for other users.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Planners can configure time for themselves. Only a <em>Workfront administrator</em> can configure time for other users.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

<ol> 
 <li value="1">Do either of the following, depending on your objective and your access level in the system: 
  <ul>
   <li><span class="bold">Planner user configuring time logging for yourself:</span> <draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Click the Main Menu icon. Click your user avatar, then click the 
      <span class="bold">More</span> icon next to your name and select 
      <span class="bold">Edit</span>.
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the Main Menu icon. Click your user avatar, then click the 
     <span class="bold">More</span> icon next to your name and select 
     <span class="bold">Edit</span>.
    </MadCap:conditionalText></li>
   <li><span class="bold">System administrator configuring time logging for others:</span> Begin editing one or more user accounts, as described in <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</li>
  </ul></li> 
 <li value="2"> <p>In the resulting dialog box, in the <span class="bold">Resource Planning</span> section, locate the <span class="bold">Log Time in</span> option.</p> <p> <img src="assets/new-timesheet-log-hours-350x249.png" style="width: 350;height: 249;"> </p> </li> 
 <li value="3">(Conditional) If you are a system administrator editing multiple users simultaneously, select <span class="bold">Log Time in</span>.</li> 
 <li value="4">Select from the following options for logging time: <br>
  <table cellspacing="0">
   <col>
   <col>
   <tbody>
    <tr>
     <td role="rowheader"><span class="bold">Hours:</span></td>
     <td>Users specify hours when logging time in <em>Workfront</em>.</td>
    </tr>
    <tr>
     <td role="rowheader"><span class="bold">Days:</span></td>
     <td> Users specify days when logging time in <em>Workfront</em>.</td>
    </tr>
   </tbody>
  </table></li> 
 <li value="5"> <p>(Conditional) If you selected to log time in days, in the <span class="bold">Equivalent Hours for Full Workday</span> field, type the number of hours that equal a full day. One day on a user's timesheet is the equivalent of the number of hours you enter here.</p> <p>Consider the following when configuring this setting: </p> 
  <ul> 
   <li>This option is not available when configuring to log time in hours.</li> 
   <li>This option is used only for the purpose of logging time. This option is not related to the <span class="bold">Schedule</span> option that is also available when editing a user. The <span class="bold">Schedule</span> option is used when calculating timelines and in other areas of <em>Workfront</em>. (For more information about using the <span class="bold">Schedule</span> option, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.)&nbsp;</li> 
  </ul> </li> 
 <li value="6">Click <span class="bold">Save Changes</span>.</li> 
</ol>

