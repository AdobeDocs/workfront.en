---
filename: create-or-statements-in-filters-text-mode
product-area: reporting
navigation-topic: text-mode-reporting
title: Create "OR" statements in text mode filters
description: You can include multiple statements when you create a filter in lists and reports.
---

# Create "OR" statements in text mode filters

You can include multiple statements when you create a filter in lists and reports.

For information about creating filters, see the following articles:

* [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
* [Edit a filter using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Text Mode filter operators

For information about Adobe Workfront filter operators in the standard filter interface, see [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront has 2 filter operators that connect each filter statement:

<ul> 
 <li> <p><span class="bold">AND</span>: When you join 2 filter statement by the AND&nbsp;operator you indicate that you want both filter statements to be met at the same time.</p> 
  <div> 
   <p>By default, the statements in a filter are joined by the AND&nbsp;operator.</p> 
   <p>When building an AND filter in the text mode interface, you don't need to use the AND operator. It is assumed.</p> 
   <div class="example" data-mc-autonum="<b>Example: </b>">
    <span class="autonumber"><span><b>Example: </b></span></span> 
    <p>To filter for tasks that have a Planned Completion Date of Today and a Percent Complete lower than 100% use the following text mode code:</p> 
    <div>
     <pre>plannedCompletionDate=$$TODAY</pre>
     <pre>plannedCompletionDate_Mod=eq</pre>
     <pre>percentComplete=100</pre>
     <pre>percentComplete_Mod=lt</pre> 
    </div> 
   </div> 
  </div> </li> 
 <li> <p><span class="bold">OR</span>: When you join 2 filter statements by the OR operator you indicate that you want either statement to be met.</p> 
  <div> <note type="tip">
    When changing your AND statements to OR statements, the number of the items in your report should increase.
   </note> 
   <p>When building an OR&nbsp;filter using the text mode interface, you must use the OR operator.</p> 
   <div class="example" data-mc-autonum="<b>Example: </b>">
    <span class="autonumber"><span><b>Example: </b></span></span> 
    <p>To filter for tasks that have a Planned Completion Date of Today or a Percent Complete lower than 100% use the following text mode code:</p> 
    <div>
     <pre>plannedCompletionDate=$$TODAY</pre>
     <pre>plannedCompletionDate_Mod=eq</pre>
     <pre>OR:1:percentComplete=100</pre>
     <pre>OR:1:percentComplete_Mod=lt</pre> 
    </div> 
   </div> 
  </div> </li> 
</ul>

## Text Mode syntax for OR filters

The text mode syntax for an OR filter must contain the following:

<ul> 
 <li> <p>The OR operator followed by a colon, a number, and another colon at the beginning of each filter line that refers to the object in the OR statement.&nbsp;This includes the line that references the filter field or attribute and the line that references the filter modifier.</p> <p>Follow this pattern when building an OR filter:</p> 
  <div>
   <pre><field name in camel case>=<value></pre>
   <pre><field name in camel case>_Mod=<modifier value></pre>
   <pre>OR:1:<field name in camel case>=<value></pre>
   <pre>OR:1:<field name in camel case>_Mod=<modifier value></pre> 
  </div> <note type="tip">
   The OR operator is case sensitive and it is always uppercase.
  </note> <p style="text-align: left;">You may have multiple OR statements in a filter. In this case, every OR statement receives a number, in the order you want the statements applied.</p> 
  <div class="example" data-mc-autonum="<b>Example: </b>">
   <span class="autonumber"><span><b>Example: </b></span></span> 
   <p> To filter for tasks that have a Planned Completion Date of Today OR a Percent Complete lower than 100% OR a Status of New use the following text mode code:</p> 
   <div>
    <pre>plannedCompletionDate=$$TODAY</pre>
    <pre>plannedCompletionDate_Mod=eq</pre>
    <pre>OR:1:status=NEW</pre>
    <pre>OR:1:status_Mod=in</pre>
    <pre>OR:2:percentComplete=100</pre>
    <pre>OR:2:percentComplete_Mod=lt</pre> 
   </div> 
  </div> </li> 
 <li> <p style="text-align: left;">The name of the fields or the attributes you reference in a filter must be written in camel case. For information about camel case, see <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref" xrefformat="{para}">Text mode syntax overview</a>.</p> </li> 
 <li> <p style="text-align: left;">When you refer to custom fields in an OR filter, you must insert DE: between the OR modifier syntax and the name of the custom field. You must spell the name of the custom field as it appears in the Workfront interface.</p> 
  <div class="example" data-mc-autonum="<b>Example: </b>">
   <span class="autonumber"><span><b>Example: </b></span></span> 
   <p>To filter for tasks that have a Status of New OR a Percent Complete lower than 100% OR a custom field called "Account Type" with a value of "Equal", use the following text mode code:</p> 
   <div>
    <pre>status=NEW</pre>
    <pre>status_Mod=in</pre>
    <pre>OR:1:percentComplete=100</pre>
    <pre>OR:1:percentComplete_Mod=lt</pre>
    <pre>OR:2:DE:Account Type=Capital</pre>
    <pre>OR:2:DE:Account Type_Mod=in</pre> 
   </div> 
  </div> </li> 
</ul>

