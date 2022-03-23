

# Connect to Snowflake

[Intro]

For more information on Data Access, see [Data Access overview](../../reports-and-dashboards/data-access/data-access-overview.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>*</td> 
   <td> <p>[Any, Pro, Business, Enterprise] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>[Request, Review, Work, Plan] or higher</p> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a group administrator. For more information on group administrators, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>[Specify special product information. Remove this line if the functionality is in Workfront Proper]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[Insert any access level configurations needed]</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must

* Have a Snowflake account. If you do not have an existing account, you need to sign up for a “Data Bundle” on-demand account with Snowflake.  
  For information on setting up your Snowflake account, see Snowflake's [Before You Begin](https://docs.snowflake.com/en/user-guide/setup.html) documentation.

## Connect to Snowflake

1. Go to the business intelligence tool you want to connect to Snowflake.
1. Add the data source with the following information:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Type the name you want to use for the Snowflake Connection.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type</td> 
      <td>Select <strong>Snowflake</strong> for the type.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Connection string</td> 
      <td> <p>Workfront provides the domain and schema that you will need for your Connection URL. Add these items in the appropriate place, then enter the connection string:</p> <p><code>jdbc:snowflake://&lt;domain provided&gt;.snowflakecomputing.com/?warehouse=analytics_wh&amp;db=workfront_analytics&amp;schema=&lt;schema provided&gt;</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If your BI&nbsp;tool has a built-in Snowflake connector, you can connect with JDBC.<br>If you connect using JDBC, the connection string may look like this:<br><code>jdbc:snowflake://&lt;domain provided&gt;.snowflakecomputing.com/?warehouse=analytics_wh&amp;db=workfront_analytics&amp;schema=&lt;schema provided&gt;</code><br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Username</td> 
      <td>Enter the Username provided.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Password</td> 
      <td>Enter the Password provided.</td> 
     </tr> 
    </tbody> 
   </table>

