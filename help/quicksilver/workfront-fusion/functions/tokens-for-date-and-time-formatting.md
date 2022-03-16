---
filename: tokens-for-date-and-time-formatting
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Tokens for date and time formatting
description: You must have the following access to use the functionality in this article:
---

# Tokens for date and time formatting

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Year, month, and day tokens

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Token </th> 
   <th>Output </th> 
   <th> <p>Description</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>YY </code> </td> 
   <td><code>70 71 ... 29 30</code> </td> 
   <td> <p> 2 digit year</p> </td> 
  </tr> 
  <tr> 
   <td><code>YYYY </code> </td> 
   <td><code>1970 1971 ... 2029 2030 </code> </td> 
   <td> <p>4 digit year</p> </td> 
  </tr> 
  <tr> 
   <td><code>Y</code> </td> 
   <td><code>1970 1971 ... 9999 +10000 +10001</code> </td> 
   <td> <p> Year with any number of digits and sign</p> </td> 
  </tr> 
  <tr> 
   <td><code>Q</code> </td> 
   <td><code>1 2 3 4 </code> </td> 
   <td> <p> Quarter of year</p> </td> 
  </tr> 
  <tr> 
   <td><code>Qo</code> </td> 
   <td><![CDATA[	]]><code>1st 2nd 3rd 4th </code></td> 
   <td> <p>Quarter of year with ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>M</code> </td> 
   <td><![CDATA[	]]><code>1 2 ... 11 12</code><![CDATA[	]]></td> 
   <td> <p>Month number</p> </td> 
  </tr> 
  <tr> 
   <td><code>Mo </code> </td> 
   <td><code>1st 2nd ... 11th 12th</code> </td> 
   <td> <p> Month with ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>MM</code> </td> 
   <td><code>01 02 ... 11 12 </code> </td> 
   <td> <p> Month number with leading zero</p> </td> 
  </tr> 
  <tr> 
   <td><code>MMM</code> </td> 
   <td><![CDATA[	]]><code>Jan Feb ... Nov Dec</code></td> 
   <td> <p> Month abbreviation</p> </td> 
  </tr> 
  <tr> 
   <td><code>MMMM</code> </td> 
   <td><code> January February ... November December</code> </td> 
   <td> <p> Month name</p> </td> 
  </tr> 
  <tr> 
   <td><code>D</code> </td> 
   <td><![CDATA[	]]><code>1 2 ... 30 31 </code></td> 
   <td> <p>Day of month</p> </td> 
  </tr> 
  <tr> 
   <td><code>Do</code> </td> 
   <td><![CDATA[	]]><code>1st 2nd ... 30th 31st</code></td> 
   <td> <p> Day of month with ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>DD</code> </td> 
   <td><![CDATA[	]]><code>01 02 ... 30 31</code></td> 
   <td> <p> Day of month with leading zero</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDD</code> </td> 
   <td><![CDATA[	]]><code>1 2 ... 364 365 </code></td> 
   <td> <p>Day of year</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDDo</code> </td> 
   <td><code>1st 2nd ... 364th 365th</code> </td> 
   <td> <p> Day of year with ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDDD </code> </td> 
   <td><code>001 002 ... 364 365</code> </td> 
   <td> <p> Day of year with leading zero</p> </td> 
  </tr> 
 </tbody> 
</table>

## Week year, week, and weekday tokens

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Token </th> 
   <th>Output </th> 
   <th> <p>Description</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>d</code> </td> 
   <td><code>0 1 ... 5 6 </code> </td> 
   <td> <p> Day of week</p> </td> 
  </tr> 
  <tr> 
   <td><code>do</code> </td> 
   <td><code>0th 1st ... 5th 6th </code> </td> 
   <td> <p> Day of week with ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>dd </code> </td> 
   <td><code>Su Mo ... Fr Sa </code> </td> 
   <td> <p>Day abbreviation</p> </td> 
  </tr> 
  <tr> 
   <td><code>ddd</code> </td> 
   <td><code>Sun Mon ... Fri Sat </code> </td> 
   <td> <p> Day abbreviation</p> </td> 
  </tr> 
  <tr> 
   <td><code>dddd </code> </td> 
   <td><code>Sunday Monday ... Friday Saturday</code> </td> 
   <td> <p> Day name</p> </td> 
  </tr> 
  <tr> 
   <td><code>E</code> </td> 
   <td><code>1 2 ... 6 7 </code> </td> 
   <td> <p> Day of week (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>w </code> </td> 
   <td><code>1 2 ... 52 53 </code> </td> 
   <td> <p>Week of year</p> </td> 
  </tr> 
  <tr> 
   <td><code>wo </code> </td> 
   <td><code>1st 2nd ... 52nd 53rd</code> </td> 
   <td> <p> Week of year with ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>ww </code> </td> 
   <td><code>01 02 ... 52 53 </code> </td> 
   <td> <p>Week of year with leading zero</p> </td> 
  </tr> 
  <tr> 
   <td><code>W</code><![CDATA[	]]></td> 
   <td><code>1 2 ... 52 53 </code> </td> 
   <td> <p>Week of year (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>Wo</code> </td> 
   <td><code>1st 2nd ... 52nd 53rd </code> </td> 
   <td> <p> Week of year with ordinal (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>WW</code> </td> 
   <td><code>01 02 ... 52 53 </code> </td> 
   <td> <p> Week of year with leading zero (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>gg</code><![CDATA[	]]></td> 
   <td><code>70 71 ... 29 30 </code> </td> 
   <td> <p>Week year</p> </td> 
  </tr> 
  <tr> 
   <td><code>gggg </code> </td> 
   <td><code>1970 1971 ... 2029 2030</code> </td> 
   <td> <p> Week year</p> </td> 
  </tr> 
  <tr> 
   <td><code>GG </code> </td> 
   <td><code>70 71 ... 29 30 </code> </td> 
   <td> <p>Week year (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>GGGG </code> </td> 
   <td><code>1970 1971 ... 2029 2030</code> </td> 
   <td> <p> Week year (ISO)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Hour, minute, second, millisecond, and offset tokens

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Token </p> </th> 
   <th>Output </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>H</code> </td> 
   <td><![CDATA[	]]><code>0 1 ... 22 23</code><![CDATA[	]]></td> 
   <td> <p>24 hour time</p> </td> 
  </tr> 
  <tr> 
   <td><code>HH</code> </td> 
   <td><![CDATA[	]]><code>00 01 ... 22 23</code></td> 
   <td> <p> 24 hour time with leading zero</p> </td> 
  </tr> 
  <tr> 
   <td><code>h</code> </td> 
   <td><![CDATA[	]]><code>1 2 ... 11 12</code></td> 
   <td> <p> 12 hour time</p> </td> 
  </tr> 
  <tr> 
   <td><code>hh </code> </td> 
   <td><code>01 02 ... 11 12</code> </td> 
   <td> <p> 12 hour time with leading zero</p> </td> 
  </tr> 
  <tr> 
   <td><code>k</code> </td> 
   <td><![CDATA[	]]><code>1 2 ... 23 24</code></td> 
   <td> <p> 24 hour time</p> </td> 
  </tr> 
  <tr> 
   <td><code>kk</code><![CDATA[	]]></td> 
   <td><code>01 02 ... 23 24</code> </td> 
   <td> <p> 24 hour time with leading zero</p> </td> 
  </tr> 
  <tr> 
   <td><code>A</code><![CDATA[	]]></td> 
   <td><code>AM PM </code> </td> 
   <td> <p>Post or ante meridiem (upper case)</p> </td> 
  </tr> 
  <tr> 
   <td><code>a</code> </td> 
   <td><code>am pm </code> </td> 
   <td> <p> Post or ante meridiem (lower case)</p> </td> 
  </tr> 
  <tr> 
   <td><code>m</code> </td> 
   <td><code> 0 1 ... 58 59</code> </td> 
   <td> <p> Minutes</p> </td> 
  </tr> 
  <tr> 
   <td><code>mm</code> </td> 
   <td><code>00 01 ... 58 59</code> </td> 
   <td> <p> Minutes with leading zero</p> </td> 
  </tr> 
  <tr> 
   <td><code>s</code> </td> 
   <td><code>0 1 ... 58 59</code> </td> 
   <td> <p> Seconds</p> </td> 
  </tr> 
  <tr> 
   <td><code>ss</code> </td> 
   <td><![CDATA[	]]><code>00 01 ... 58 59</code><![CDATA[	]]></td> 
   <td> <p>Seconds with leading zero</p> </td> 
  </tr> 
  <tr> 
   <td><code>S</code> </td> 
   <td><code>0 1 ... 8 9 </code> </td> 
   <td> <p> Fractional seconds</p> </td> 
  </tr> 
  <tr> 
   <td><code>SS</code> </td> 
   <td><code>00 01 ... 98 99</code> </td> 
   <td> <p> Fractional seconds with leading zero</p> </td> 
  </tr> 
  <tr> 
   <td><code>SSS</code> </td> 
   <td><code>000 001 ... 998 999</code> </td> 
   <td> <p> Fractional seconds with two leading zeros</p> </td> 
  </tr> 
  <tr> 
   <td><code>SSSS ... SSSSSSSSS</code> </td> 
   <td><code>000[0..] 001[0..] ... 998[0..] 999[0..] </code> </td> 
   <td> <p> Fractional seconds</p> </td> 
  </tr> 
  <tr> 
   <td><code>Z</code> </td> 
   <td><![CDATA[	]]><code>-07:00 -06:00 ... +06:00 +07:00 </code></td> 
   <td> <p>Time zone</p> </td> 
  </tr> 
  <tr> 
   <td><code>ZZ</code> </td> 
   <td><![CDATA[	]]><code>-0700 -0600 ... +0600 +0700 </code></td> 
   <td> <p>Time zone</p> </td> 
  </tr> 
  <tr> 
   <td><code>X</code> </td> 
   <td><code>1360013296</code> </td> 
   <td> <p> Unix Timestamp</p> </td> 
  </tr> 
  <tr> 
   <td><code>x</code> </td> 
   <td><![CDATA[	]]><code>1360013296123</code></td> 
   <td> <p> Unix Millisecond Timestamp</p> </td> 
  </tr> 
 </tbody> 
</table>

