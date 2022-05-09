---
filename: string-functions
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: String functions in Adobe Workfront Fusion
description: You must have the following access to use the functionality in this article - EDIT ME.
---

# String functions in Adobe Workfront Fusion

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## ascii (text; [remove diacritics])

Removes all non-ascii characters from a text string.

``` ```**Examples: **``````

* ```ascii(```

  ```
  Wěošrčkřfžrýoáníté
  ```

  ```)```

  Returns: Workfront

* ```ascii(```

  ```
  ěščřž
  ```

  ```;``` [!DNL true] ```)```

  Returns: escrz

## base64 (text)

Transforms text to base64.

**Example:** <pre><span class="function">base64(</span>workfront<span class="function">)</span></pre>Returns: d29ya2Zyb250==  

## capitalize (text)

Converts the first character in a text string to uppercase.

**Example:** <pre><span class="function">capitalize(</span>workfront<span class="function">)</span></pre>Returns: Workfront  

## contains (text; search string)

Verifies whether text contains the search string.

``` ```**Examples: **``````

* ```contains(```

  ```
  Hello World<span class="function">;</span>Hello
  ```

  ```)```

  Returns: true

* ```contains(```

  ```
  Hello World<span class="function">;</span>Bye
  ```

  ```)```

  Returns: false

## decodeURL (text)

Decodes special characters in a URL to text.

**Example:** <pre><span class="function">decodeURL(</span>Automate%20your%20workflow<span class="function">)</span></pre>Returns: Automate your workflow  

## encodeURL (text)

Encodes special characters in some text to a valid URL address.

## escapeHTML (text)

Escapes all HTML tags in text.

**Example:** <pre><span class="function">escapeHTML(</span><b>Hello</b><span class="function">)</span></pre>Returns: &lt;b&gt;Hello&lt;/b&gt;  

## escapeMarkdown(text)

Escapes all Markdown tags in text.

**Example:** ```escapeMarkdown(```

```
# Header
```

```)```

Returns: &#35; Header

## indexOf (string; value; [start])

Returns the position of the first occurrence of a specified value in a string. This method returns '-1' if the value that is searched for is not there. The start value indicates where in the string the search should begin.

``` ```**Examples: **``````

* ```indexOf(```

  ```
  Workfront
  ```

  ```;```

  ```
  o
  ```

  ```)```

  Returns: 1

* ```indexOf(```

  ```
  Workfront
  ```

  ```;```

  ```
  x
  ```

  ```)```

  Returns: -1

* ```indexOf(```

  ```
  Workfront
  ```

  ```;```

  ```
  o
  ```

  ```;```

  ```
  3
  ```

  ```)```

  Returns: 6

## length (text or buffer)

Returns the length of text string (number of characters) or binary buffer (buffer size in bytes).

**Example:** <pre><span class="function">length(</span>hello<span class="function">)</span></pre>Returns: 5  

## lower (text)

Converts all alphabetical characters in a text string to lowercase.

**Example:** ```lower(```Hello ```)```

Returns: hello

## md5 (text)

Calculates the md5 hash of a string.

**Example:** ```md5(```Workfront ```)```

Returns: 1448bbbeaa7a9b8091d426999f1f666b

## replace (text;search string; replacement string)

Replaces the search string with the new string.

**Example:** <pre><span class="function">replace(</span>Hello World<span class="function">;</span>Hello<span class="function">;</span>Hi<span class="function">)</span></pre>Returns: Hi World  Regular expressions (enclosed in

```
/.../
```

) can be used as search string with a combination of flags (such as 

```
g
```

, 

```
i
```

, 

```
m
```

) appended:

**Example:**  ![](assets/replace---1-350x31.png)

All of these numbers X X X X are replaced with X  The replacement string can include the following special replacement patterns:

* 

  ```
  $&
  ```

  Inserts the matched substring.
* 

  ```
  $n
  ```

  Where n is a positive integer less than 100, inserts the nth parenthesized submatch string. This is 1-indexed.

``` ```**Examples: **``````  ![](assets/variable-value-350x63.png)

Returns: Phone number +420777111222

&nbsp;

![](assets/variable-value---2-350x55.png)

Returns: Phone number: +420777111222

>[!CAUTION]
>
>Do not use named capture groups such as >
>```>
>/ is (?<number>\d+)/
>```>
>in the replacement string argument. Doing so results in an error.

For more information on regular expressions, see [Text parser](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## sha1 (text; [encoding]; [key])

Calculates the sha1 hash of a string. If the key argument is specified, sha1 HMAC hash is returned instead. Supported encodings: "hex" (default), "base64" or "latin1."

**Example:** <pre><span class="function">sha1(</span>workfront<span class="function">)</span></pre>Returns: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f  

## sha256 (text; [encoding]; [key])

Calculates the sha256 hash of a string. If the key argument is specified, sha256 HMAC hash is returned instead. Supported encodings: "hex" (default), "base64" or "latin1".

**Example:** <pre><span class="function">sha256(</span>workfront<span class="function">)</span></pre>Returns: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc  

## sha512 (text; [output encoding]; [key]; [key encoding])

Calculates the sha512 hash of a string. If the key argument is specified, sha512 HMAC hash is returned instead.

Supported encodings:

* "hex" (default)
* "base64"
* "latin1"

Supported key encodings:

* "text" (default)
* "hex"
* "base64" or "binary"

When using "binary" key encoding, a key must be a buffer, not a string.

**Example:** <pre><span class="function">sha512(</span>workfront<span class="function">)</span></pre>Returns: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19  

## split (text; separator)

Splits a string into an array of strings by separating the string into substrings.

**Example:** <pre><span class="function">split(</span>John, George, Paul<span class="function">;</span>,<span class="function">)</span></pre>

## startcase (text)

Capitalizes the first letter of every word and lower cases all other letters.

**Example:** ```startcase(```

```
hello WORLD
```

```)```

Returns: Hello World

## stripHTML (text)

Removes all HTML tags from text.

**Example:** ```stripHTML(```

```
<b>Hello</b>
```

```)```

Returns: Hello

## substring (text; start;end)

Returns a portion of a text string between the "start" position and "end" position.

``` ```**Examples: **``````

* ```substring(```

  ```
  Hello<span class="function">;</span>0<span class="function">;</span>3
  ```

  ```)```

  Returns: Hel

* ```substring(```

  ```
  Hello<span class="function">;</span>1<span class="function">;</span>3
  ```

  ```)```

  Returns: el

## toBinary (value)

Converts any value to binary data.

You can also specify encoding as a second argument to apply binary conversions from hex or base64 to binary data.

``` ```**Examples: **``````

* ```toBinary(```

  ```
  Workfront
  ```

  ```)```

  Returns: 57 6f 72 6b 66 72 6f 6e 74

* ```toBinary(```

  ```
  V29ya2Zyb250<span class="function">;</span>
  ```

  ```
  base64
  ```

  ```)```

  Returns: 57 6f 72 6b 66 72 6f 6e 74

## toString (value)

Converts any value to a string.

## trim (text)

Removes space characters at the start or end of the text.

## upper (text)

Converts all alphabetical characters in a text string to uppercase.

**Example:** ```upper(```

```
Hello
```

```)```

Returns: HELLO
