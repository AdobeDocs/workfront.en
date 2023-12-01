---
content-type: api
navigation-topic: api-navigation-topic
title: Escaped characters in API Responses
description: Escaped characters in API Responses
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
---
# Escaped characters in API Responses

The syntax of some API responses may contain the escape character, `\` (backslash). An escape character indicates that the character or string of characters that immediately follow the escaped character have a special value. For example, `\t` tells the reading device that `t` should be interpreted as `tab` and not as the letter "t". A string of one or more characters following the backslash is called an escape sequence.

Hexadecimal escaped sequences require the use of valid hexadecimal digits. The following table lists the escape sequences that are encoded in Adobe Workfront API responses:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Escape Sequence</strong> </th> 
   <th><strong>Unicode Character</strong> </th> 
   <th><strong>Represents</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>Where, <em>x</em> is the hexadecimal code for numbers 0 through 7</p> </td> 
   <td>0-7</td> 
   <td>Unicode characters represented by code points 0 through 7</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>Backspace</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>Tab</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>New line</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>Vertical tab</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>Form feed</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Carriage return</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>Where, xx is the hexadecimal code for&nbsp; numbers 14 through 31</em> </p> </td> 
   <td>14 - 31</td> 
   <td>Unicode characters represented by code points 14 through 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (Forward slash)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; (Less than)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (Back slash)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>Where, <em>xxxx</em> is the hexadecimal code for any number over 127</p> </td> 
   <td>128+</td> 
   <td>Unicode characters for any code point over 127</td> 
  </tr> 
 </tbody> 
</table>
