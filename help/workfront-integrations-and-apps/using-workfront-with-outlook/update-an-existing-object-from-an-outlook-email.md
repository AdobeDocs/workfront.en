---
filename: update-an-existing-object-from-an-outlook-email
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Update an existing object from an Outlook email
description: You can update an existing project, task, or issue with information from an Outlook email.
---

# Update an existing object from an Outlook email

You can update an existing project, task, or issue with information from an Outlook email.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Work, Plan</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>[Insert any access level configurations needed] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: Edit access to Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: Edit access to Documents
      </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[Insert any access level configurations needed] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: Edit access to Documents
     </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed and specify the object] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: View access or higher on Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: View access or higher on Documents
      </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[Insert permissions needed and specify the object] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: View access or higher on Documents
     </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

Your *Workfront administrator* must enable Outlook for Office with *Workfront* before you can use this integration.

## Update an existing object from an Outlook email

<ol> 
 <li value="1">In Outlook, select the email that contains the information that you want to include in an <em>Adobe Workfront</em>&nbsp;update.&nbsp;</li> 
 <li value="2">Click the&nbsp;<span class="bold"><em>Workfront</em></span>&nbsp;icon in the upper-right corner of the email message to ndisplay the <em>Workfront</em> add-in.<br>You might need to click the down-pointing arrow in the upper right of your email to access the <em>Workfront</em> icon.</li> 
 <li value="3">Click the <span class="bold">Menu</span> icon to display the list of available <em>Workfront</em> options.<br><img src="assets/o365-addin-menu-icon.png" alt="o365_addin_menu_icon.png"></li> 
 <li value="4">Click <span class="bold">Update in <em>Workfront</em></span>.<br><img src="assets/outlook-update-in-workfront-menu-253x345.png" alt="outlook_Update_in_workfront_menu.png" style="width: 253;height: 345;"><br>You can update the following information from the email before it is saved as a task: 
  <ul>
   <li><span class="bold">Type</span>: Select the type of object you are updating. You can select <span class="bold">Project</span>, <span class="bold">Task</span>, or <span class="bold">Issue</span>. The object you select determines the results that display in the <span class="bold">Name</span> field below. If you are unsure of the type of object, select <span class="bold">All</span> to search for projects, tasks, and issues simultaneously.</li>
   <li><span class="bold">Name</span>: Begin&nbsp;typing the name of the project, task, or issue that you want to update. Click the name when it appears in the drop-down list.</li>
   <li><span class="bold">Update</span>: By default, the update is the same as the email Body. You can modify the update as desired.<br>This update is displayed as the update status in <em>Workfront</em>.</li>
   <li><span class="bold">Attachments</span>: Any email attachments are saved to the Documents area of the task. You can delete any attachments before submitting the update.</li>
  </ul></li> 
 <li value="5"> (Optional) Click&nbsp;<span class="bold">Include Others</span>, begin typing the name of users who you want to include in the update, then click the name when it appears in the drop-down list. <br>Repeat this process to include additional users, then click <span class="bold">Done</span>.<br>By default, the user you are replying to receives a notification regardless of whether you include them.<br><img src="assets/o365-addin-includeothers.png" alt="o365_addin_includeothers.png"><br></li> 
 <li value="6"> (Optional)&nbsp;Click the <span class="bold">Lock</span> icon to restrict this update to users within your company. When the update is locked, users outside your company cannot see the update. 
  <ul>
   <li><span class="bold">Unlocked:</span> Any user with access to the project, task, or issue where the update resides can view the update.<br>By default, the update is unlocked.<br><img src="assets/o365-addin-unlock.png" alt="o365_addin_unlock.png"></li>
   <li><span class="bold">Locked:</span> Only users within your company can view the update.<br><img src="assets/o365-addin-lock.png" alt="o365_addin_lock.png"><br></li>
  </ul></li> 
 <li value="7"> Click <span class="bold">Update</span>. </li> 
 <li value="8"> (Optional) Click <span class="bold">View in <em>Workfront</em></span> to view the updated item with the <em>Workfront</em> integration within Outlook. </li> 
</ol>

