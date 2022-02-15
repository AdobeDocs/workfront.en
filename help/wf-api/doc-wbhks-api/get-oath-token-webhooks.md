---
filename: get-oath-token-webhooks
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Get OAuth2 Tokens {#get-oauth-tokens}



## Getting OAuth2 Tokens (needed OAuth2 authentication only) {#getting-oauth-tokens-needed-oauth-authentication-only}

Returns the OAuth2 refresh token and access token for an authenticated user. This is invoked once when the the user provisions a Document Provider. Subsequent calls are made to get an updated access token.


## URL {#url}

HTTP Request POST /any/url


The URL is configurable and corresponds to the Token Endpoint URL value on the custom integration Setup page.


## Query {#query}



## Parameters {#parameters}


<table style="height: 356px;width: 700px;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1">
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1">
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1">
 <thead>
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1">
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Name</th>
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Required</th>
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Description</th>
  </tr>
 </thead>
 <tbody>
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">grant_type</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">yes</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"><p>Values include “authorization_code” or “refresh_token”. The value specified indicates which of the two parameters will be passed to this API call: code or refresh_token.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">code</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">depends</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"><p>The authorization code sent to <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> just after the user clicks the “Grant” button. This is only required when the grant type is “authorization_code”. The authorization code should be short lived, generally expiring in 10 minutes or less.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">refresh_token</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">depends</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"><p>This is only required when making subsequent calls to retrieve a new access_token, given that the previous access_token as expired. When sending this value set the grant_type parameter to “refresh_token”.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">client_id</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">yes</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">The Client ID configured in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for this custom integration.</td>
  </tr>
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">client_secret</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">yes</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">&nbsp;The Client Secret configured in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for this custom integration.</td>
  </tr>
 </tbody>
</table>

&nbsp;

## Response {#response}



<table style="height: 128px;width: 688;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1">
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1">
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1">
 <thead>
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1">
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Name</th>
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Type&nbsp;</th>
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Description</th>
  </tr>
 </thead>
 <tbody>
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">access_token&nbsp;</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">String</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"><p>A token used to make authorized API calls on the user’s behalf. This should expire to prevent unauthorized API calls.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">refresh_token&nbsp;</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">String</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"><p>A long-lived token used to retrieve a new access_token by calling this API method.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">expires_in&nbsp;</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">long</td>
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"><p>(optional) The time (in seconds) before the access_token expires, generally 3,600.</p></td>
  </tr>
 </tbody>
</table>

Example
`<pre>POST /oauth2/token<br>grant_type=authorization_code<br>code=d9ac7asdf6asdf579d7a8<br>client_id=123456<br>client_secret=6asdf7a7a9a4af</pre>`

## Response {#response-1}

`<pre>{<br>access_token:"ad8af5ad5ads759",<br>refresh_token:"9a0h5d87d808ads",<br>expires_id:3600<br>}</pre>` 