

# Group rows in a table

You can organize the information in a report by displaying it in groups defined by currency, date, percentage, text, and time

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
fields
</MadCap:conditionalText>
-->

.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to create Reports, Calendars, and Dashboards</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta program.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For more information, see [link to Beta enrollment info].
</MadCap:conditionalText>
-->

## Group rows in a table

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Reports**.
1. Click **New report**.

   Or

   Go to an existing report, click the **More Menu** icon ![](assets/more-icon.png) in the report header, then select **Edit**. 

   <!--
   <MadCap:conditionalText style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   Should this step be a separate section and just a link here?
   </MadCap:conditionalText>
   -->

1. (Conditional) To group rows on an existing table, click the **Edit** icon ![](assets/edit-icon.png) in the table header.
1. In the right panel, locate the field that you want group by and drag it to the **Group** section.

   You can use the Search box to find the group you want.

1. (Optional) Type a new name for the group.
1. Select an option to indicate how you want the grouped rows to be sorted.

   The options vary based on the type of field you are using to group your rows.

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Currency</td> 
      <td> 
       <ul> 
        <li> <p>Smallest to Biggest</p> </li> 
        <li> <p>Biggest to Smallest</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date</td> 
      <td> 
       <ul> 
        <li> <p>Oldest - Newest</p> </li> 
        <li> <p>Newest - Oldest</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percent</td> 
      <td> 
       <ul> 
        <li> <p>Smallest to Biggest</p> </li> 
        <li> <p>Biggest to Smallest</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Text</td> 
      <td> 
       <ul> 
        <li> <p>A - Z</p> </li> 
        <li> <p>Z - A</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Time</td> 
      <td> 
       <ul> 
        <li> <p>Smallest to Biggest</p> </li> 
        <li> <p>Biggest to Smallest</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) To have rows in a group collapsed by default, click the **More menu** icon ![](assets/more-icon.png) next to the group, then select **Collapse**.

   >[!NOTE]
   >
   >Each group can be set individually to display with rows collapsed or expanded. By default, all grouped rows are collapsed.

1. (Optional) To display a count in the group row, click the **More menu** icon ![](assets/more-icon-27x15.png) next to the group, then select **Display count**.
1. (Optional) To remove a group, click the **More menu** icon ![](assets/more-icon.png) next to the group, then select **Remove group**.

