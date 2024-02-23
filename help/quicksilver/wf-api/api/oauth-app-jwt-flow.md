---
content-type: api
navigation-topic: api-navigation-topic
title: Using JWT flow for custom OAuth 2 applications 
description: Using JWT flow for custom OAuth 2 applications
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
---
# Configure and use your organization's custom OAuth 2 applications using JWT flow

In order to integrate with Workfront and allow your client app to communicate with Workfront on behalf of the user, you must:

* Create an OAuth2 application
* Create a Public Key Certificate
* Create a JSON Web Token (JWT)

## Create an OAuth2 Application

For instructions on creating the OAuth2 application, see [Create an OAuth2 application using server authentication (JWT flow)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [Create OAuth2 applications for Workfront integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Create a Public Key Certificate

The JWT must be signed and base-64 encoded for inclusion in the access request. The JWT libraries provide functions to perform these tasks.

The token must be signed using the private key for a digital signing certificate. If you do so, you can use the private key of any associated certificate to sign your JWT.

The algorithm used is RS256&nbsp;(RSA Signature with SHA-256). This is an asymmetric algorithm, and it uses a public/private key pair. The identity provider has a private (secret) key used to generate the signature, and the consumer of the JWT gets a public key to validate the signature.

To generate the public key, do **one** of the following.

* Open your MacOS/Linux terminal and execute the following command, then upload `certificate_pub.crt` using the **Add public key** button in the OAuth2 application setup in Workfront.

  <!-- [Copy](javascript:void(0);) --> 
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Use the **Generate a public/private keypair** button in the OAuth2 application setup in Workfront to generate the RSA.

## Create a JSON Web Token

A JSON Web Token for Service Account authentication requires a particular set of claims, and must be signed using a valid digital signing certificate. We recommend that you use one of the publicly available libraries or tools for building your JWT.

The following table contains information about fields that may be required when you are configuring the JWT token.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Required. The expiration parameter is a required parameter measuring the absolute time since 01/01/1970 GMT. You must ensure that the expiration time is later than the time of issue. After this time, the JWT is no longer valid.&nbsp;</p> <p>Note: We recommend that you have a very short lived token (a few minutes), so that it expires soon after it has been exchanged for an access token. Every time a new access token is required, one JWT is signed and exchanged. This is a more secure approach. We do not recommend longer lived tokens that are re-used to obtain access tokens as needed.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>Required. The issuer is your&nbsp;Customer ID&nbsp;from the OAuth2 app details.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Required. The subject is your&nbsp;User ID&nbsp;that created the public key in setup.</td> 
  </tr> 
 </tbody> 
</table>

## Exchange the JWT to retrieve an access token

1. Send a POST request to:

   <!-- [Copy](javascript:void(0);) --> 
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. The body of the request should contain URL-encoded parameters with your Client ID, Client Secret, and JWT:

   <!-- [Copy](javascript:void(0);) --> 
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

&nbsp;
