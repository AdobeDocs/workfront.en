---
filename: get-oath-token-webhooks
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Get OAuth2 Tokens
description: Returns the OAuth2 refresh token and access token for an authenticated user. This is invoked once when the the user provisions a Document Provider. Subsequent calls are made to get an updated access token.
---

# Get OAuth2 Tokens

## Getting OAuth2 Tokens (needed OAuth2 authentication only)

Returns the OAuth2 refresh token and access token for an authenticated user. This is invoked once when the the user provisions a Document Provider. Subsequent calls are made to get an updated access token.

## URL

HTTP Request POST /any/url

The URL is configurable and corresponds to the Token Endpoint URL value on the custom integration Setup page.

## Query

## Parameters

<table cellspacing="15">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Name</th>
   <th>Required</th>
   <th>Description</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>yes</td>
   <td><p>Values include “authorization_code” or “refresh_token”. The value specified indicates which of the two parameters will be passed to this API call: code or refresh_token.</p></td>
  </tr>
  <tr>
   <td>code</td>
   <td>depends</td>
   <td><p>The authorization code sent to Adobe Workfront just after the user clicks the “Grant” button. This is only required when the grant type is “authorization_code”. The authorization code should be short lived, generally expiring in 10 minutes or less.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>depends</td>
   <td><p>This is only required when making subsequent calls to retrieve a new access_token, given that the previous access_token as expired. When sending this value set the grant_type parameter to “refresh_token”.</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>yes</td>
   <td>The Client ID configured in Workfront for this custom integration.</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>yes</td>
   <td>&nbsp;The Client Secret configured in Workfront for this custom integration.</td>
  </tr>
 </tbody>
</table>

&nbsp;

## Response

<table cellspacing="15">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Name</th>
   <th>Type&nbsp;</th>
   <th>Description</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token&nbsp;</td>
   <td>String</td>
   <td><p>A token used to make authorized API calls on the user’s behalf. This should expire to prevent unauthorized API calls.</p></td>
  </tr>
  <tr>
   <td>refresh_token&nbsp;</td>
   <td>String</td>
   <td><p>A long-lived token used to retrieve a new access_token by calling this API method.</p></td>
  </tr>
  <tr>
   <td>expires_in&nbsp;</td>
   <td>long</td>
   <td><p>(optional) The time (in seconds) before the access_token expires, generally 3,600.</p></td>
  </tr>
 </tbody>
</table>

Example
<pre>POST /oauth2/token<br>grant_type=authorization_code<br>code=d9ac7asdf6asdf579d7a8<br>client_id=123456<br>client_secret=6asdf7a7a9a4af</pre>

## Response

<pre>{<br>access_token:"ad8af5ad5ads759",<br>refresh_token:"9a0h5d87d808ads",<br>expires_id:3600<br>}</pre>