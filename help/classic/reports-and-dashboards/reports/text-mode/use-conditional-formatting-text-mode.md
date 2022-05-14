---
filename: use-conditional-formatting-text-mode
product-area: reporting
navigation-topic: text-mode-reporting
title: Use conditional formatting in Text Mode
description: Use conditional formatting in Text Mode
---

# Use conditional formatting in Text Mode

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: this article might need to be split in its sections. Tony asked that numbers and dates should be in separate articles (??))</p>
-->

The standard interface builder provides a great range of flexibility when creating reporting elements to meet the needs in your organization.

You can apply conditional formatting in a view by using the standard interface.  
For more information about applying conditional formatting to a view, see [Use conditional formatting in views](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to edit views in a report</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to edit views in a report</p> <p>Manage permissions to a view to edit it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Conditional formatting in Text Mode

Text mode enables you&nbsp;to create more complex views, filters, groupings, and prompts by allowing you to use fields that are not available in the standard interface.

For a complete list of all our reportable fields, see the&nbsp; [API Explorer](../../../wf-api/general/api-explorer.md).

For more information about using text mode syntax, see [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

You can also use text mode to format views in reports and lists.&nbsp;Using conditional formatting, you can change the views of your reports by changing the font type and background of the results in&nbsp;the report, as well as icons and flags. We recommend that you always build your views using the standard interface first and switch to the text mode interface only when absolutely necessary.

>[!NOTE]
>
>&nbsp;Using CSS styling to customize&nbsp;conditional formatting is not supported. Instead, you must use the predesigned formatting options that are&nbsp;available in Adobe Workfront.

## Add conditional formatting to Views

For more information about applying conditional formatting to a view in the standard builder interface, see [Use conditional formatting in views](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

To add conditional formatting to a view in the text mode interface:

1. Go to a list of objects.
1. Expand the drop-down menu of a view to which you want to add conditional formatting.
1. Click **Customize View**.
1. Click the column in the view to which you want to apply conditional formatting.
1. Click **Switch to Text Mode**.
1. In the **Show in this column:** area, click **Click to edit text**.

1. Add the code samples provided in [Format Views using Text Mode](#format-views-using-text-mode) at the bottom of the text in the column you selected.
1. Click **Save**, then click **Save View**.

## Format Views using Text Mode {#format-views-using-text-mode}

You can add the following components to a column in a view to conditionally format it in text mode:

* [Column settings](#column-settings) 
* [Column rules](#column-rules) 
* [Conditionally format a valueexpression](#conditionally-format-a-valueexpression)

### Column settings {#column-settings}

You must be familiar with the text mode interface before you can add conditional formatting to your views.

You can customize the following elements of a column when using conditional formatting in a view:

* [Column headers](#column-headers) 
* [Format dates](#format-dates) 
* [Format numbers](#format-numbers)

#### Column headers {#column-headers}

To change the displayed column header, add&nbsp;the following code to your column:
<pre>displayname=&nbsp;[Name of column]</pre>For example, to name a column Project Owner, the text code would look like:
<pre>displayname=Project Owner</pre>

#### Format dates {#format-dates}

Dates can be configured to display in a variety of formats.

For more information, see [Format dates in text mode reports](../../../reports-and-dashboards/reports/text-mode/format-dates-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above)</p>
-->
<p>To establish a date format, you must modify the <code>valueformat</code> line of the text mode code in the column.</p>
<pre>valueformat=&nbsp;[new date format]</pre>
<p>For example, if you wanted the Projected Completion Date to be displayed as MM/DD/YY the code would look like:</p>
<pre>valueformat=atDate<br>valuefield=projectedCompletionDate&nbsp;</pre>
<p>If you wanted to show the Planned Completion Date as <em>Mth, DD, Year</em>, the code would look like:</p>
<pre>valueformat=mediumAtdate<br>valuefield=plannedCompletionDate</pre>
<p>You can format dates using the following <code>valueformat</code>&nbsp;text mode values:</p>
<table>
<col>
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Format</strong> </th>
<th scope="col">Example&nbsp;</th>
<th scope="col"><em><strong>valueformat=</strong></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>atDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY Time</td>
<td>10/11/18 12:00pm</td>
<td><pre>longAtDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>shortAtDate</pre> </td>
</tr>
<tr>
<td>Mth, DD, YR</td>
<td>Oct, 11, 2018</td>
<td><pre>mediumAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR</td>
<td>Mon, Oct, 11, 2018</td>
<td><pre>partialAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR Time</td>
<td>Mon, Oct, 11, 2018 12:00 pm</td>
<td><pre>fullAtDate</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

#### Format numbers {#format-numbers}

You can format numeric values to display information that best suits your reporting needs.

For more information, see [Format numbers, currency and percentage values in text mode reports](../../../reports-and-dashboards/reports/text-mode/format-numbers-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To modify the format of a numeric value, you must edit the&nbsp;<strong>valueformat</strong>&nbsp;line of your column.</p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above) </p>
-->
<p>For example, if you wanted to display the Budget column as $1000, the value format line would look like:</p>
<pre>valueformat=currencyStringCurrencyRounded<br>valuefield=budget</pre>
<p>You can format numbers&nbsp;using the following values for the&nbsp;<code>valueformat</code>&nbsp;line of your column:</p>
<table border="2" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Example</strong> </th>
<th scope="col"><em><code>valueformat=</code></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>1234</td>
<td><pre>doubleAsString</pre> or <pre>int</pre></td>
</tr>
<tr>
<td>1,234</td>
<td><pre>doubleAsInt</pre> </td>
</tr>
<tr>
<td>$1,234</td>
<td><pre>currencyStringCurrencyRounded</pre> </td>
</tr>
<tr>
<td>1234.56</td>
<td><pre>doubleAsDouble</pre> </td>
</tr>
<tr>
<td>$1,234.56</td>
<td><pre>currencyStringCurrency</pre> </td>
</tr>
<tr>
<td>12%</td>
<td><pre>doubleAsPercentRounded</pre> </td>
</tr>
<tr>
<td>12.34%</td>
<td><pre>doubleAsPercent</pre> </td>
</tr>
<tr>
<td>(1,234.56)</td>
<td><pre>doubleAsFinancial</pre> </td>
</tr>
<tr>
<td>(1,234)</td>
<td><pre>doubleAsFiancialRounded</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

### Column rules {#column-rules}

Column rules allow for the addition of images, color, formatting, and text overrides within a view. Column rules can be established independently or can contain multiple conditions for a column.

* [Conditional formatting](#conditional-formatting) 
* [Multiple conditional formats](#multiple-conditional-formats) 
* [Apply text](#apply-text) 
* [Apply row formats](#apply-row-formats) 
* [Apply images](#apply-images)

#### Conditional formatting {#conditional-formatting}

A specific text mode statement must be applied when incorporating color or formatting text.

>[!NOTE]
>
>Conditional formatting may not be supported in merged columns.  
>For more information on merging columns with Text Mode, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

Insert the following code in any column where you want to add conditional formatting to:
<pre>styledef.case.0.comparison.leftmethod=&nbsp;[field name]<br>styledef.case.0.comparison.lefttext= [field name]<br>styledef.case.0.comparison.righttext= [field value]<br>styledef.case.0.comparison.operator=&nbsp;[qualifier]<br>styledef.case.0.comparison.operatortype= [data type]<br>styledef.case.0.comparison.icon=false<br>styledef.case.0.comparison.truetext=&nbsp;<br>styledef.case.0.comparison.trueproperty.0.name= [format option]&nbsp;<br>styledef.case.0.comparison.trueproperty.0.value= [format style]</pre>

>[!NOTE]
>
>The >
>```>
>styledef.case.0.comparison.icon
>```>
>line is always false unless working with icons.
>
>The >
>```>
>styledef.case.0.comparison.truetext
>```>
>line is always left blank until working with overwriting text.
>
>The >
>```>
>styledef.case.0.comparison.righttext
>```>
>line is blank when the qualifier is notblank.

For example, if we wanted to show the Company Name in green text on a project report, you can use the following&nbsp;code:
<pre>styledef.case.0.comparison.leftmethod=company:name<br>styledef.case.0.comparison.lefttext=company:name&nbsp;<br>styledef.case.0.comparison.righttext=&nbsp;<br>styledef.case.0.comparison.operator=notblank<br>styledef.case.0.comparison.operatortype=string<br>styledef.case.0.comparison.icon=false<br>styledef.case.0.comparison.truetext=<br>styledef.case.0.comparison.trueproperty.0.name=textcolor<br>styledef.case.0.comparison.trueproperty.0.value=03a219</pre>

>[!NOTE]
>
>* While this&nbsp;statement could be&nbsp;applied to a Company Name column, it could also be applied to any other column on the report. Green text would only be displayed if the project had a Company associated with it. Remember the [field name], [value], and [qualifier] drive whether or not the conditioning ultimately displays on the column.
>* When working with qualifiers, we recommended using >
>  ```>
>  cicontains
>  ```>
>  rather than >
>  ```>
>  equal
>  ```>
>  . By default, >
>  ```>
>  equal
>  ```>
>  looks for ID numbers. Using the >
>  ```>
>  cicontains
>  ```>
>  qualifier, you can access items by their name.
>

![](assets/screen-shot-2013-08-15-at-2.53.51-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-2.54.08-pm-350x185.png)

Whether Text Color, Alignment, Font Style, or Background Color are applied to a text mode, the same statement (shown above) is used.

The following lines must be modified to reflect the corresponding formatting needed for the column:
<pre>styledef.case.0.comparison.trueproperty.0.name= [format option]<br>styledef.case.0.comparison.trueproperty.0.value= [format style]</pre>Use the following tables to identify which lines need to be modified and what values you should specify&nbsp;to define the format style of your column:

| **Text Color** |**Line: textcolor=** |
|---|---|
| Black |<pre>000000</pre> |
| Dark Blue |<pre>0c6aca</pre> |
| Teal |<pre>1b878c</pre> |
| Green |<pre>03a219</pre> |
| Purple |<pre>6408c4</pre> |
| Grey |<pre>767676</pre> |
| Red |<pre>d30519</pre> |
| Yellow |<pre>e19503</pre> |

| **Alignment** |**Line: align=** |
|---|---|
| Left alignment |<pre>left</pre> |
| Right alignment |<pre>right</pre> |
| Center Alignment |<pre>center</pre> |

| Font |Line:&nbsp;***fontstyle=*** |
|---|---|
| Bold |<pre>bold</pre> |
| Italic |<pre>italic</pre> |

| **Background Color** |**Line: bgcolor=** |
|---|---|
| Teal |<pre>dcf6f7</pre> |
| Green |<pre>def6e2</pre> |
| Grey |<pre>e8e8e8</pre> |
| Blue |<pre>e8f1ff</pre> |
| Purple |<pre>e9def4</pre> |
| Red |<pre>eac6c9</pre> |
| Yellow |<pre>feecc8</pre> |
| White |<pre>ffffff</pre> |

#### Multiple conditional formats {#multiple-conditional-formats}

You can apply more than one formatting style to a statement. The core statement would remain unchanged and any additional formatting expressions would be added to the statement.

For example, using the earlier statement to include Company Name in green bolded text. The statement would be written using the following code:
<pre>styledef.case.0.comparison.leftmethod=company:name<br>styledef.case.0.comparison.lefttext=company:name<br>styledef.case.0.comparison.righttext=<br>styledef.case.0.comparison.operator=notblank<br>styledef.case.0.comparison.operatortype=string<br>styledef.case.0.comparison.icon=false<br>styledef.case.0.comparison.truetext=&nbsp;<br>styledef.case.0.comparison.trueproperty.0.name=textcolor<br>styledef.case.0.comparison.trueproperty.0.value=03a219<br>styledef.case.0.comparison.trueproperty.1.name=fontstyle<br>styledef.case.0.comparison.trueproperty.1.value=bold</pre>

>[!NOTE]
>
>When including more than one conditional formatting expression, it is necessary to numerically identify each expression in the statement. Notice that expression 0 and expression 1 have been identified.

![](assets/screen-shot-2013-08-15-at-3.18.45-pm-350x198.png)

#### Apply text {#apply-text}

If you want to replace the default values that populate in a column with a value of your choosing, it is possible when applying text&nbsp;to the column.

For example, on a project report, set the Planned Start Date column value to not display the planned start date for the project, but rather the text 'Not Today.' Use the following code for the Planned Start Date column:
<pre>case.0.comparison.leftmethod=plannedStartDate<br>case.0.comparison.lefttext=plannedStartDate&nbsp;<br>case.0.comparison.righttext=2013-04-10T10:45:00:000&nbsp;<br>case.0.comparison.operator=ne&nbsp;<br>case.0.comparison.operatortype=date&nbsp;<br>case.0.comparison.icon=false&nbsp;<br>case.0.comparison.truetext=not today<br>styledef.case.0.comparison.leftmethod=plannedStartDate<br>styledef.case.0.comparison.lefttext=plannedStartDate&nbsp;<br>styledef.case.0.comparison.righttext=2013-04-10T10:45:00:000&nbsp;<br>styledef.case.0.comparison.operator=ne&nbsp;<br>styledef.case.0.comparison.operatortype=date&nbsp;<br>styledef.case.0.comparison.icon=false&nbsp;<br>styledef.case.0.comparison.truetext=not today</pre>

>[!NOTE]
>
>The lines that start with >
>```>
>case.0.
>```>
>&nbsp;use case comparisons to identifying the use of text. The lines that start with **styledef.case.0.**&nbsp;are early conditional formatting statements where we identify the use of text through the >
>```>
>truetext
>```>
>expression. Make sure to set >
>```>
>truetext
>```>
>to a value, rather than leaving it blank.

![](assets/screen-shot-2013-08-15-at-3.22.02-pm-350x196.png)

![](assets/screen-shot-2013-08-15-at-3.22.16-pm-350x151.png)

#### Apply row formats {#apply-row-formats}

If you would like to apply a condition to the entire row, use the following code&nbsp;with your column code:
<pre>styledef.case.0.comparison.icon=false</pre><pre>styledef.case.0.comparison.isrowcase=true</pre><pre>styledef.case.0.comparison.leftmethod= [field name]</pre><pre>styledef.case.0.comparison.lefttext= [field name]</pre><pre>styledef.case.0.comparison.operator= [qualifier]</pre><pre>styledef.case.0.comparison.operatortype= [data type]</pre><pre>styledef.case.0.comparison.righttext= [field value]</pre><pre>styledef.case.0.comparison.trueproperty.0.name= [format option]</pre><pre>styledef.case.0.comparison.trueproperty.0.value= [format style]</pre><pre>styledef.case.0.comparison.truetext=</pre><pre>row.0.styledef.applyallcases=true</pre><pre>row.0.styledef.case.0.comparison.icon=false</pre><pre>row.0.styledef.case.0.comparison.isrowcase=true</pre><pre>row.0.styledef.case.0.comparison.leftmethod= [field name]</pre><pre>row.0.styledef.case.0.comparison.lefttext= [field name]</pre><pre>row.0.styledef.case.0.comparison.operator= [qualifier]</pre><pre>row.0.styledef.case.0.comparison.operatortype= [data type]</pre><pre>row.0.styledef.case.0.comparison.righttext= [field value]</pre><pre>row.0.styledef.case.0.comparison.trueproperty.0.name= [format option]</pre><pre>row.0.styledef.case.0.comparison.trueproperty.0.value= [format style]</pre><pre>row.0.styledef.case.0.comparison.truetext=</pre>

#### Apply images {#apply-images}

Similarly to formatting with text, images can be used to display information in reports. Workfront has a number of built-in images to convey visual information in a report setting. To use images in the conditional formatting setting the following statement is needed:
<pre>image.case.0.comparison.leftmethod= [field name]<br>image.case.0.comparison.lefttext= [field name]<br>image.case.0.comparison.righttext= [field value]<br>image.case.0.comparison.operator= [qualifier]<br>image.case.0.comparison.operatortype= [data type]<br>image.case.0.comparison.icon=true<br>image.case.0.comparison.truetext=</pre>For example, on a project report, you want to build a column where you would show a frown face for every Planned Completion Date that does&nbsp;not equal to today's date. Use the following text mode code to add the icon to your column:
<pre>image.case.0.comparison.leftmethod=plannedCompletionDate<br>image.case.0.comparison.lefttext=plannedCompletionDate<br>image.case.0.comparison.righttext=2013-04-10T13:00:00:000&nbsp;<br>image.case.0.comparison.operator=ne&nbsp;<br>image.case.0.comparison.operatortype=date<br>image.case.0.comparison.icon=true<br>image.case.0.comparison.truetext=/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif</pre>

>[!NOTE]
>
>Notice that the statement uses the >
>```>
>icon=true
>```>
>expression. This statement is also different from other conditional formatting statements in that it does not use the >
>```>
>style.def
>```>
>format, but rather a unique image format.

![](assets/screen-shot-2013-08-15-at-3.35.08-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-3.35.22-pm-1-350x167.png)

To use the images available, apply the following code and values:

| **Icon** |**Line: image.case.0.comparison.truetext=** |
|---|---|
| Frown Face&nbsp; ![](assets/face-sad.png)|=`/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif` |
| Happy Face&nbsp; ![](assets/face-happy.png)|=`/interface/images/v4_redux/icons/casebuilder/emoticon_smile.gif&nbsp;` |
| Blue Flag&nbsp; ![](assets/flag-blue-large.png)|=`/interface/images/v4_redux/icons/casebuilder/flag_blue.gif&nbsp;` |
| Green Flag&nbsp; ![](assets/flag-green-large.png)|=`/interface/images/v4_redux/icons/casebuilder/flag_green.gif` |
| Red Flag&nbsp; ![](assets/flag-red-style2.png)|=`/interface/images/v4_redux/icons/casebuilder/flag_red.gif` |
| Yellow Flag&nbsp; ![](assets/flag-yellow-style2.png)|=`/interface/images/v4_redux/icons/casebuilder/flag_yellow.gif` |
| Black Circle&nbsp; ![](assets/dot-black.png)|=`/interface/images/v4_redux/icons/casebuilder/light_black.gif&nbsp;` |
| Blue Circle&nbsp; ![](assets/dot-blue.png)|=`/interface/images/v4_redux/icons/casebuilder/light_blue.gif&nbsp;` |
| Grey Circle&nbsp; ![](assets/dot-gray.png)|=`/interface/images/v4_redux/icons/casebuilder/light_grey.gif&nbsp;` |
| Green Circle&nbsp; ![](assets/dot-green.png)|=`/interface/images/v4_redux/icons/casebuilder/light_green.gif&nbsp;` |
| Orange Circle&nbsp; ![](assets/dot-orange.png)|=`/interface/images/v4_redux/icons/casebuilder/light_orange.gif&nbsp;` |
| Pink Circle&nbsp; ![](assets/dot-pink.png)|=`/interface/images/v4_redux/icons/casebuilder/light_pink.gif&nbsp;` |
| Purple Circle&nbsp; ![](assets/dot-purple.png)|=`/interface/images/v4_redux/icons/casebuilder/light_purple.gif&nbsp;` |
| Red Circle&nbsp; ![](assets/dot-red.png)|=`/interface/images/v4_redux/icons/casebuilder/light_red.gif` |
| White Circle&nbsp; ![](assets/dot-white.png)|=`/interface/images/v4_redux/icons/casebuilder/light_white.gif&nbsp;` |
| Yellow Circle&nbsp; ![](assets/dot-yellow.png)|=`/interface/images/v4_redux/icons/casebuilder/light_yellow.gif` |

### Conditionally format a 

```
valueexpression
```

{#conditionally-format-a-valueexpression}

To display a calculated value in a column, you can replace the 

```
valuefield
```

line of code in the column with a 

```
valueexpression
```

. A calculated value allows you to display a new value for an objects based on the calculation between two existing fields on that same object.  
For more information about how to format the 

```
valueexpression line
```

, see [Text mode syntax overview](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

You cannot conditionally format a column which contains a 

```
valueexpression
```

line of code.  
Instead, you can add a Calculated Custom Field to a Custom Form and associate it with the objects you are displaying in the report. Then, you can conditionally format the columns displaying this field.

For more information about Calculated Custom Fields, see [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Add an aggregator value in a Text Mode column

We recommend that you build the column in the builder interface first, add the aggregator value there, and then edit the column in Text Mode.

Consider the following when adding aggregators to a column in Text Mode:

* The values in the column must have a format that can be summarized.&nbsp;For example, they must have one of the following formats:

   * Number
   * Date
   * Currency

* You can add an aggregator to a column that displays a calculation. The aggregated value displays in the grouping of the view or report. For more information, see [Grouping: display the result of aggregating multiple calculated values in a grouping](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
* The lines of code for the definition of the column must be identical to the lines of code introducing the aggregator and preceded by "aggregator."&nbsp;For example, if you have a column where you display Planned Hours on a project, the text mode of the main lines of the column is:
  <pre>valuefield=workRequired<br>valueformat=compound</pre>When you want to aggregate the value of all the lines in the grouping of the view, we can add the following code to add the aggregator values:

  ```
  aggregator.valuefield=workRequired
  ```

  (the 

  ```
  aggregator.valuefield
  ```

  line must be the same as the 

  ```
  valuefield
  ```

  that describes the column)

  ```
  aggregator.valueformat=compound
  ```

  (the 

  ```
  aggregator.valueformat
  ```

  line must have the same value as the 

  ```
  valueformat
  ```

  that describes the column)

  ```
  aggregator.function=SUM
  ```

  (this is a mandatory line that indicates how you want to aggregate the column, in this case, you want to add all the individual Planned Hours into one number in the grouping line)

  ```
  aggregator.displayformat=minutesAsHoursString
  ```

  (because hours are stored in Workfront in minutes, we want to indicate the 

  ```
  displayformat
  ```

  for hours when they are stored in minutes)

