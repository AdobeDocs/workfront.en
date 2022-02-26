

# Connect to Snowflake

[Intro]

For more information on *Data Access*, see [Data Access overview](../../reports-and-dashboards/data-access/data-access-overview.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><em>Adobe Workfront</em> plan</a>*</td> 
   <td> <p><em>[Any, Pro, Business, Enterprise]</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p><em>[Request, Review, Work, Plan]</em> or higher</p> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>[Specify special product information. Remove this line if the functionality is in Workfront Proper]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[Insert any access level configurations needed]</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level.<br>For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

Before you begin, you must

* Have a Snowflake account. If you do not have an existing account, you need to sign up for a “Data Bundle” on-demand account with Snowflake.  
  For information on setting up your Snowflake account, see Snowflake's [Before You Begin](https://docs.snowflake.com/en/user-guide/setup.html) documentation.

## Connect to Snowflake

<ol> 
 <li value="1"> <p>Go to the business intelligence tool you want to connect to Snowflake.</p> </li> 
 <li value="2"> <p>Add the data source with the following information:</p> 
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
     <td>Select <span class="bold">Snowflake</span> for the type.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Connection string</td> 
     <td> <p><em>Workfront</em> provides the domain and schema that you will need for your Connection URL. Add these items in the appropriate place, then enter the connection string:</p> <p><code>jdbc:snowflake://<domain provided>.snowflakecomputing.com/?warehouse=analytics_wh&db=workfront_analytics&schema=<schema provided></code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If your BI&nbsp;tool has a built-in Snowflake connector, you can connect with JDBC.<br>If you connect using JDBC, the connection string may look like this:<br><code>jdbc:snowflake://<domain provided>.snowflakecomputing.com/?warehouse=analytics_wh&db=workfront_analytics&schema=<schema provided></code><br></p> </td> 
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
  </table> </li> 
</ol>

