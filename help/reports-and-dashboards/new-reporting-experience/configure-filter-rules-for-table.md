

# Configure filter rules in Reporting Canvas

After you add a table to a report, you can set up filter rules to limit the information that displays in the table. With the right access, you can also modify a table in an existing report at any time.

<!--
[insert more in-depth info here on filters rules, and/or, modifiers, etc.]
-->

There are 3 components in a filter rule:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Field</td> 
   <td> <p>The field that contains the information that you want to filter for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operator</td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Value</td> 
   <td> <p>The information that you want to filter for.</p> </td> 
  </tr> 
 </tbody> 
</table>

` `**Example: **`` If you wanted to limit results in your report to only display projects that are owned by Jane Doe, you could create a filter rule with the field "Project Owner," the operator "Equal To," and the value "Jane Doe."

Or you could display only projects that have an assigned project owner, which would have the field "Project Owner" and the operator "Is Not Blank."

If you want your report to display results for both of these filter rules, you would add the link/connective AND.

[Insert image?]

##  

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
   <td> <p>Edit access to create reports, calendars, and dashboards</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> Object permissions Manage access to the report For information on requesting additional access, see Request access to objects in Adobe Workfront. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta program.

<!--
For more information, see [link to Beta enrollment info].
-->

## Configure filter rules for a table

<ol> 
 <li value="1"> <p>Go to an existing report, click the <span class="bold">More Menu</span> icon <img src="assets/more-icon.png"> in the report header, then select <span class="bold">Edit</span>.</p> </li> 
 <li value="2"> <p>Locate the table in the report, then click the <b>Edit</b> icon <img src="assets/edit-icon.png"> in the table header.</p> <note type="tip">
   If a table has not been configured yet, an Edit button displays instead.
   <br style="font-weight: bold;">
   <!--
    [insert image of table header]
   -->
  </note> </li> 
 <li value="3"> <p>In the right panel, locate the field that you want to filter by.</p> 
  <ol> 
   <li value="1"> <p>(Optional) Enter text in the <span class="bold">Search</span> box.</p> <!--
     Up to X fields display.
    --> </li> 
   <li value="2">(Conditional) If you don't see the field that you want, click <span class="bold">More fields</span> to display more options.<br><span class="bold">[insert screenshot here]</span></li> 
  </ol> </li> 
 <li value="4"> <p>Select the field, then drag it to the Filter section.</p> <p>A filter rule displays.</p> </li> 
 <li value="5"> <p>Select the modifier that you want from the drop-down menu:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Equal To</span> </td> 
     <td> <p>This only returns an exact match of the searched value.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Not Equal To</span> </td> 
     <td> <p>This only returns results that are not exact match of the searched value.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Is Blank</span> </td> 
     <td> <p>The field exists for the object but the field has not yet been given a value.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Is Not Blank</span> </td> 
     <td> <p>The field you are filtering for exists and has been given a value.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Is Less Than</span> </td> 
     <td> <p>This searches for all results with a value less than what is entered, not including the entered value.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Is Less Than Or Equal To</span> </td> 
     <td> <p>This searches for all results with a value less than or equal to the entered value.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Is Greater Than</span> </td> 
     <td> <p>This searches for all results with a value greater than the value entered, not including the entered value.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Is Greater Than Or Equal To</span> </td> 
     <td> <p>This searches for all results with values greater than or equal to the entered value.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Between</span> </td> 
     <td> <p>Provides 2 required field values and searches for all results within range of both fields including the entered values.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Contains</span> </td> 
     <td> <p>This searches for the specified text throughout an entire text string.</p> <p>For example, using "Contains Inf" captures anything with "Inf" or "inf" in it, such as the word "Infinity".</p> <note type="note">
       Adobe Workfront searches for the exact word or phrase that you are specifying for each filter statement. For example, if you are searching for any project that contains the phrase "new project" in the name, Workfront does not display projects that have just "new" or just "project", or "new main project" in the name. The filter finds only projects with the exact phrase "new project" in the name.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Does Not Contain</span> </td> 
     <td> <p>This filters for items that are missing the value specified.</p> <p>For example, "does not contain inf" captures anything with without "Inf" or "inf" in the name.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>Enter the last value to complete the filter rule.</p> <note type="note">
   Values entered are not case sensitive. For example, using "Contains Inf" captures anything with "Inf" or "inf" in it, such as the word "Infinity".
   <br>
  </note> </li> 
 <li value="7"> <p>(Optional) To add another filter rule, drag the field to the <span class="bold">Drop to add another rule</span> drop area in the Filters section, then repeat Steps 5-6.</p> </li> 
 <li value="8"> <p>(Conditional) If you want to add a filter rule set, do the following:</p> 
  <ol> 
   <li value="1"> <p>Drag the field that you want to add to the <b>Add a rule set</b> drop area.</p> <p>&nbsp;</p> </li> 
   <li value="2"> <p>Drag the next field for your filter rule set to the <span class="bold">Drop to add another rule</span> drop area.</p> <p>&nbsp;</p> </li> 
  </ol> </li> 
 <li value="9"> <p>(Conditional) If you have filter rule sets or multiple filter rules, select the operator drop-down, then select <b>AND</b> or <b>OR</b>.</p> <p> <img src="assets/operator-drop-down.png"> </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"> <p>AND</p> </td> 
     <td> <p>When you join filter rules or rule sets with the AND operator, you indicate that you want all rules at the same level to be met.</p> <p>By default, the statements in a filter are joined by the AND operator.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>&nbsp;</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>OR</p> </td> 
     <td> <p>When you join filter rules or rule set with the OR operator you indicate that you want at least one rule—or rule set—at that level to be met.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>&nbsp;</p> </td> 
    </tr> 
   </tbody> 
  </table> <note type="important">
   If you have an AND operator selected, all filter criteria must apply for a result to display in the report.
   <br>depending on the level of the operator
   <br>AND operators and OR operators at the same level—connecting rule sets or connecting filters within a rule set—always match. If you change one of them, all operators at the same level update.
  </note> </li> 
</ol>

## Configure filter rules for a page filter

This is coming, One of the 3 dimmed options in the right panel when you edit. Will get rid of need for prompts.

<ol> 
 <li value="1"> <p>Go to an existing report, click the <span class="bold">More Menu</span> icon <img src="assets/more-icon.png"> in the report header, then select <span class="bold">Edit</span>.</p> </li> <!--
 --> 
</ol>

