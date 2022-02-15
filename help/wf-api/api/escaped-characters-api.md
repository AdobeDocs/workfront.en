---
filename: escaped-characters-api
content-type: api
navigation-topic: api-navigation-topic
---



# Escaped characters in API Responses {#escaped-characters-in-api-responses}

The syntax of some API responses may contain the escape character, "\" (backslash). An escape character indicates that the character or string of characters that immediately follow the escaped character have a special value. For example, \t tells the reading device that "t" should be interpreted as "tab" and not as the letter t. A string of one or more characters following the backslash is called an escape sequence.&nbsp;


Hexadecimal escaped sequences require the use of valid hexadecimal digits. The following table lists the escape sequences that are encoded in *`Adobe Workfront`* API responses:

<table style="width: 587px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Escape Sequence</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Unicode Character</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"><span class="bold">Represents</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>\u000<em>x</em></p> <p>Where, <em>x</em> is the hexadecimal code for numbers 0 through 7</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">0-7</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Unicode characters represented by code points 0 through 7</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">\b</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">8</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Backspace</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">\t</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">9</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Tab</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">\n</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">10</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">New line</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">\u000b</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">11</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Vertical tab</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">\f</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">12</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Form feed</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">\r</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">13</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Carriage return</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>\u00<em>xx</em></p> <p><em>Where, xx is the hexadecimal code for&nbsp; numbers 14 through 31</em> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">14 - 31</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Unicode characters represented by code points 14 through 31</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>\/</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">47</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">/ (Forward slash)</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>\u003c</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">60</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&lt; (Less than)</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>\\</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">92</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">\ (Back slash)</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>\u<em>xxxx</em></p> <p>Where, <em>xxxx</em> is the hexadecimal code for any number over 127</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">128+</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Unicode characters for any code point over 127</td> 
  </tr> 
 </tbody> 
</table>

