---
filename: create-complex-text-mode-filters-using-exists-statements
product-area: reporting
navigation-topic: text-mode-reporting
title: Create complex Text Mode filters using EXISTS statements
description: Important: This article requires a thorough understanding of the Adobe Workfront API and of the text mode reporting interface. For information about the Workfront API, see API basics. For information about using text mode, see Text Mode overview.
---

# Create complex Text Mode filters using EXISTS statements

>[!IMPORTANT]
>
>This article requires a thorough understanding of the *Adobe Workfront* API and of the text mode reporting interface. For information about the *Workfront* API, see [API basics](../../../wf-api/general/api-basics.md).   
>For information about using text mode, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Overview of object relationships in *Workfront*

All objects are linked to other objects in the *Workfront* database.

Understanding the hierarchy and interdependency of objects helps you find out what objects can be referenced in reports.

For information about what objects are in *Workfront* and about their hierarchy and interdependency, see [Understand objects in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

When building filters, you can reference other objects that are connected to the object of the filter within up to 2 levels of relationship using the standard reporting interface.

For example, you can reference the Portfolio ID in an issue filter to display only issues on projects associated with a certain portfolio using the standard interface. In this case, the portfolio is 2 levels away from issues.

However, you cannot reference the Portfolio Owner in an issue filter using the standard interface to display only issues from projects associated with portfolios where the owner is a specific user. You must use text mode to access the Portfolio Owner Name field which is three levels away from issues.

![issue_to_portfolio_owner_sraight_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

For a complete list of objects in *Workfront*, see the [API Explorer](../../../wf-api/general/api-explorer.md).

For information about how to navigate the API Explorer and find objects, see [Using the API Explorer](../../../wf-api/general/using-api-explorer.md).

When building filters, you must build complex statements in the text-mode interface to reference these types of objects.

For information about building complex filters, see the [Overview of Complex Text-Mode Filters that Use EXISTS Statements](#exists-filters) section.

## Overview of complex text mode filters that use EXISTS statements

Consider the following when creating filters that span multiple levels in the object hierarchy or filter for missing objects:

* You must create complex filters when you want to reference objects not directly connected to the filter object.
* You must use an EXISTS statement to do the following:

  * Create filters that span multiple levels.
  * Create filters that look for objects that are missing.  
    For example, when building a user report, you can filter for users who have not logged time for a certain period of time.

Consider the following rules when using EXISTS statements in a filter:

* There are three objects that you could reference in an EXISTS filter:

  * The object of the filter (Original Object).
  * The object whose field you want to reference (Target Object).
  * The object that connects the Original and the Target Objects, in case they are not directly connected to one another (Linking Object).

* Filters that use EXISTS contain two separate statements linked by an equal sign:

  * The statement before the equal sign refers to the object you are referring to (the Linking or the Target Object).
  * The statement after the equal sign refers to the object you are referring from (the Original Object).

* You must use the object code of the Linking Object to connect your statements.  
  You can find the object code of all objects in the API Explorer.  
  For information about the API Explorer, see the [API Explorer](https://one.workfront.com/s/api-explorer).

* When a Linking Object is missing because the Original and the Target Objects are connected to each other directly, you can use the Object Code of the Target Object instead of the Linking Object.  
* You can refer to multiple fields (Target Fields) on the same object (Target Object) in which case you must connect the lines that are referring to the fields by AND.  
  For an example of filtering for more than one field that belongs to the Target Object, see the [Example 4: Filter by multiple fields: tasks by Portfolio Owner Name and Portfolio Alignment Scorecard ID](#example-4) section in this article.

* The only modifier supported for an EXISTS statement is NOTEXISTS.

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
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to edit filters in a report</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to edit filters in a report</p> <p>Manage permissions to a filter to edit it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create complex text mode filters that span multiple levels in the object hierarchy

You can build a filter that references objects across multiple levels of the object hierarchy in which the filter object exists. For example, you can build an issue filter for issues that are on projects that are not associated with a certain Portfolio Owner.

You must always use an EXISTS statement and the text mode interface to build this filter.

For examples of filters, see the [Example 1: Filter for issues by Portfolio Owner Name](#example-1) section in this article.

To create a filter that spans over multiple levels in the object hierarchy:

<ol> 
 <li value="1">Identify the object of your filter. We refer to this object as the Original Object.<br>For example, Issue.</li> 
 <li value="2">Identify the field that you want to filter by. We refer to this object as the Target Field that belongs to a Target Object.<br>For example, the ownerID field (Target Field) which belongs to Portfolio (Target Object).</li> 
 <li value="3"> <p>(Conditional) If the Original Object (Issue) and the Target Field (ownerID) are not directly connected to each other, you must find a third object, a Linking Object (Project) that connects them. The Linking Object must have at least one field that is referenced from the Fields or References tabs of the Original Object (Linking Field displayed on the Original Object) and it must also have a Linking Field to the Target Object displayed in the Fields or References tabs of the Linking Object. The Linking Field to the Target Object which displays on the Linking Object (or the Linking Field displayed on the Linking Object) must match the Target Field.<br>For example, (Project) ID (Linking Field displayed on the Original Object) is referenced from Issues (Original Object). (Portfolio) ownerID (Linking Field to the Target Object) is displayed in the Fields tab of the Project (Linking Object). Portfolio ownerID is also a field on the Target Object (Portfolio). The Linking Field on the Linking Object matches the Target Field.<br><img src="assets/portfolio-id-in-the-project-api-object-350x88.png" alt="portfolio_id_in_the_project_api_object.PNG" style="width: 350;height: 88;"><br></p> </li> 
 <li value="4">Using the API Explorer, identify the <span class="bold">Object Code</span> of the Linking Object (Project).<br>For example, the Object Code for Project is PROJ.<br><img src="assets/project-objcode-in-the-api-350x84.png" alt="project_objCode_in_the_API.PNG" style="width: 350;height: 84;"></li> 
 <li value="5">Create a filter for the Original Object.<br>For example, create an Issue filter.<br>For information about creating filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</li> 
 <li value="6">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="7">Paste the following formula example to the text mode interface of the new filter and replace the suggested text with the correct objects and fields:<br><pre>EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field></pre><p>For an example using the fields we have identified above, see the <a href="#example-1" class="MCXref xref">Example 1: Filter for issues by Portfolio Owner Name</a> section in this article.</p></li> 
 <li value="8"> <p>Click <span class="bold">Save Filter</span>.</p> </li> 
</ol>

## Create complex text mode filters for missing objects

You can build a filter that references objects that are missing. For example, you can build a user filter that shows which users have not logged hours in *Workfront*.

You must always use an *EXISTS* statement and the text mode interface to build this filter.

For examples of filters for missing objects, see the following sections in this article:

* [Example 2: Filter for missing objects: custom fields that do not appear in any custom forms](#example-2) 
* [Example 3: Filter for missing objects: users who did not log time for a certain period of time](#example-3)

To create a filter that references missing objects:

<ol> 
 <li value="1">Identify the object of your filter. We refer to this object as the Original Object.<br>For example, Parameter or Custom Field.</li> 
 <li value="2">Identify the field that you want to filter by. We refer to this object as the Target Field that belongs to a Target Object.<br>For example, the categoryID field (Target Field) which belongs to Category (Target Object).</li> 
 <li value="3">Because the Original Object (Parameter) and the Target Field (categoryID) are not directly connected to each other, you must find a third object, a Linking Object (a Category Parameter) that connects them. The Linking Object must have at least one field that is referenced from the Fields or References tabs of the Original Object (Linking Field displayed on the Original Object) and it must also have a Linking Field to the Target Object displayed in the Fields or References tabs of the Linking Object. The Linking Field to the Target Object which displays on the Linking Object (or the Linking Field displayed on the Linking Object) must match the Target Field.<br>For example, the ID of the Category Parameter (Linking Field displayed on the Original Object) is referenced from Parameter(Original Object). parameterID (Linking Field to the Target Object) is displayed in the Fields tab of the Category Parameter (Linking Object). The Linking Field to the Target Object which displays on the Linking Object matches the Target Field.</li> 
 <li value="4">Using the API Explorer, identify the <span class="bold">Object Code</span> of the Linking Object (Category Parameter).<br>For example, the Object Code for Category Parameter is CTGYPA.<br><img src="assets/category-parameter-objcode-in-api-350x79.png" alt="category_parameter_objcode_in_api.PNG" style="width: 350;height: 79;"></li> 
 <li value="5">Create a filter for the Original Object.<br>For example, create a Parameter filter.<br>For information about creating filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</li> 
 <li value="6">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="7">(Conditional) If you are filtering for objects that are missing, paste the following formula example to the text mode interface of the new filter and replace the suggested text with the correct objects and fields: <p><code>EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br></code><code>EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS</code></p><p>For an example of reporting on Custom Fields that are not associated with Custom Forms, see the <a href="#example-2" class="MCXref xref">Example 2: Filter for missing objects: custom fields that do not appear in any custom forms</a> section in this article.</p></li> 
 <li value="8"> <p>Click <span class="bold">Save Filter</span>.</p> </li> 
</ol>

## Examples of text mode filters that span multiple levels in the object hierarchy

* [Example 1: Filter for issues by Portfolio Owner Name](#example-1) 
* [Example 2: Filter for missing objects: custom fields that do not appear in any custom forms](#example-2) 
* [Example 3: Filter for missing objects: users who did not log time for a certain period of time](#example-3) 
* [Example 4: Filter by multiple fields: tasks by Portfolio Owner Name and Portfolio Alignment Scorecard ID](#example-4)

### Example 1: Filter for issues by Portfolio Owner Name

Using the text mode interface, you can build a filter for a list of issues to display only issues that are on projects associated with a portfolio whose owner is a specific user.

To filter issues by the Portfolio Owner Name:

<ol> 
 <li value="1">Create an Issue filter.<br>For information about creating filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</li> 
 <li value="2">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="3">Refer to the following generic code:<br><code>EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br></code><code>EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field></code></li> 
 <li value="4">Paste the following code in the <span class="bold">Set Filter Rules for your Report</span> area to replace the generic code above:<br><pre>EXISTS:A:$$OBJCODE=PROJ<br>EXISTS:A:ID=FIELD:projectID<br>EXISTS:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221</pre> <note type="note">  
   <ul> 
    <li>The Original Object is the object of the report: Issue</li> 
    <li>The Target Object is Portfolio.</li> 
    <li>The Linking Object is Project.</li> 
    <li>The Target Field and the Linking Field to the Target Object referenced from the Linking Object is ownerID.</li> 
    <li>The Object code of the Linking Object here is PROJ.</li> 
    <li>The Linking Field displayed on the Original Object is projectID and the Linking Field is ID.</li> 
   </ul> 
  </note></li> 
 <li value="5">Replace the value of the Target Field (ownerID) in the last statement with a User ID from your environment.</li> 
 <li value="6">Click <span class="bold">Save Filter</span>.</li> 
</ol>

### Example 2: Filter for missing objects: custom fields that do not appear in any custom forms

Using the text mode interface, you can build a filter to view Custom Fields (Parameters) that are not associated with Custom Forms (Categories). This filter links Parameters to Categories, which are connected through another object, Category Parameter. Because the two fields are not directly connected to one another and because you are filtering for missing information you must use an EXISTS statement.

>[!IMPORTANT]
>
>A Parameter is a field as it exists in the Field Library referenced in a Custom Form. A Category Parameter is the version of a field that appears on a specific form. For example, if the same field appears on 5 forms there will be 1 Parameter and 5 Category Parameters in the *Workfront* Database.

To filter for Custom Fields that are not associated with a Custom Form:

<ol> 
 <li value="1">Create a Parameter or a Custom Field filter.<br>For information about creating filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</li> 
 <li value="2">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="3">Refer to the following generic code:<br><code>EXISTS:A:$$OBJCODE=<Object code of the Linking Object></code><br><code>EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS</code></li> 
 <li value="4">Paste the following code in the <span class="bold">Set Filter Rules for your Report</span> area to replace the generic code above:<br><pre>EXISTS:A:$$OBJCODE=CTGYPA<br>EXISTS:A:parameterID=FIELD:ID<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS</pre> <note type="note">  
   <ul> 
    <li>The Original Object is the object of the report: Parameter.</li> 
    <li>The Target Object is Category.</li> 
    <li>The Linking Object is Category Parameter.</li> 
    <li>The Object code of the Linking Object is CTGYPA.</li> 
    <li>The Linking Field to the Target Object is parameterID because parameterID exists in both the Linking Object Table and Target Object Table.</li> 
    <li>The Linking Field displayed on the Original Object is ID (of the Category Parameter).</li> 
   </ul> 
  </note></li> 
 <li value="5">Click <span class="bold">Save Filter</span>.</li> 
</ol>

### Example 3: Filter for missing objects: users who did not log time for a certain period of time

Using the text mode interface, you can build a filter to view Users who did not log time for a certain time period. This filter links Users to Hours, which are connected to one another directly. However, you must use an EXISTS statement and the text mode interface to be able to filter for missing information.information.

To filter for users who did not log time during last week:

<ol> 
 <li value="1">Create a User filter.<br>For information about creating filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</li> 
 <li value="2">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="3">Refer to the following generic code:<br><code>EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br></code><code>EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS</code></li> 
 <li value="4">Paste the following code in the <span class="bold">Set Filter Rules for your Report</span> area to replace the generic code above:<br><p><code>EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS</code></p> <note type="note">  
   <ul> 
    <li>The Original Object is the object of the report: User.</li> 
    <li>The Target Object is Hour.</li> 
    <li>You do not need a Linking Object in this example because Users and Hours are directly connected in the <em>Workfront</em> database.</li> 
    <li>Because there is no Linking Object, you must use the Object Code of the Target Object: HOUR.</li> 
    <li>The Linking Field to the Target Object is ownerID (which displays on the Original Object; the Linking Object is missing).</li> 
    <li>The Linking Field displayed on the Original Object is ID (of the Hour) (which displays on the Target Object; the Linking Object is missing.)</li> 
    <li>The EXISTS:A:entryDate statement refers to fields that define the Target Object (Hour) and uses the same syntax as in a regular filter statement. This ensures that you display only those users who did not log time for a specific period of time, in this case, the previous week.</li> 
    <li>The NOTEXISTS modifier indicates that we are looking for items (Hours) that do not exist for the object of the report (Users).</li> 
   </ul> 
  </note></li> 
 <li value="5">Click <span class="bold">Save Filter</span>.</li> 
</ol>

### Example 4: Filter by multiple fields: tasks by Portfolio Owner Name and Portfolio Alignment Scorecard ID

Using the text mode interface, you can build a filter that refers to more than one field on the Target Object. In this case, the filter statements that are referring to the Target Fields must be connected by AND.

For example, you can filter a list of tasks to display only tasks that meet the following criteria:

* They are on a project associated with a portfolio whose owner is a specific user.
* They are on a project associated with a portfolio whose projects are not associated with a specific alignment scorecard.

To filter tasks by the Portfolio Owner Name and Portfolio Alignment Scorecard ID:

<ol> 
 <li value="1">Create a Task filter.<br>For information about creating filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</li> 
 <li value="2">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="3">Paste the following code in the <span class="bold">Set Filter Rules for your Report</span> area:<br><pre>EXISTS:A:$$OBJCODE=PROJ<br>EXISTS:A:ID=FIELD:projectID<br>EXISTS:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f<br>AND:A:EXISTS:A:$$EXISTSMOD=NOTEXISTS<br>AND:A:EXISTS:A:$$OBJCODE=PROJ<br>AND:A:EXISTS:A:ID=FIELD:projectID<br>AND:A:EXISTS:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad</pre> <note type="note">  
   <ul> 
    <li>The Original Object is the object of the filter: Task.</li> 
    <li>The Target Object is Portfolio.</li> 
    <li>The first Target Field is ownerID.</li> 
    <li>The second Target Field is Alignment Scorecard ID.</li> 
    <li>The Linking Object is Project.</li> 
    <li>The Object Code of the Linking Object is PROJ.</li> 
    <li>The Linking Field to the Target Object is the ID (of the Portfolio).</li> 
    <li>The Linking Field displayed on the Original Object is projectID.</li> 
    <li>Replace the ownerID with a User ID from your environment.</li> 
   </ul> 
  </note></li> 
 <li value="4">Click <span class="bold">Save Filter</span>.</li> 
</ol>

