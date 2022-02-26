---
filename: add-outlook-email-as-task-to-your-work-list
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Add an Outlook email as a task to your work list
description: You can convert Outlook emails to Adobe Workfront tasks. After an email is converted, the task is available in your Work List in the Home area.
---

# Add an Outlook email as a task to your work list

You can convert Outlook emails to *Adobe Workfront* tasks. After an email is converted, the task is&nbsp;available in your Work List in the Home area.

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

## Add an Outlook email as a task to your work list

<ol> 
 <li value="1">Select the email within Outlook that you want to convert to a task.</li> 
 <li value="2">Click the&nbsp;<span class="bold"><em>Workfront</em></span>&nbsp;icon in the upper-right corner of the email message to display the <em>Workfront</em> add-in.<br>You might need to click the down-pointing arrow in the upper right of your email to access the <em>Workfront</em> icon.</li> 
 <li value="3">Click the <span class="bold">Menu</span> icon to display the list of available <em>Workfront</em> options.<br><img src="assets/o365-addin-menu-icon.png" alt="o365_addin_menu_icon.png"></li> 
 <li value="4">Click <span class="bold">Add to Work</span>.<br><img src="assets/outlook-add-to-work-menu-242x337.png" alt="outlook_add_to_work_menu.png" style="width: 242;height: 337;"></li> 
 <li value="5">Deselect the <span class="bold">Add to Project</span> field.&nbsp;</li> 
 <li value="6">(Optional) You can update the following information from the email before it is saved as a task: 
  <ul>
   <li><span class="bold">Task Name:</span> By default, the task name is the same as the email Subject. You can modify the task name as desired.</li>
   <li><span class="bold">Description:</span> By default, the description is the same as the email Body. You can modify the description&nbsp;as desired.</li>
   <li><span class="bold">Attachments:</span> Any email attachments are saved to the Documents area of the task. You can delete any attachments before saving&nbsp;the email as a task.</li>
  </ul></li> 
 <li value="7">Click <span class="bold">Add</span>.<br>The task is added to the Work List in your Home area with no commit date.</li> 
 <li value="8"> <p>(Optional) Click <span class="bold">View in <em>Workfront</em></span>&nbsp;to display the task within the&nbsp;<em>Workfront</em> application in a new tab.<br></p> </li> 
 <li value="9">(Optional) Navigate back to Outlook, and select the original email.<br>At the top of the <em>Workfront</em> add-in panel, notice the confirmation with a link that the email was added to <em>Workfront</em> as a task. The link includes the date on which it was converted.<br><img src="assets/outlook-standalone-task-added-350x123.png" alt="outlook_standalone_task_added.png" style="width: 350;height: 123;"><br></li> 
</ol>

