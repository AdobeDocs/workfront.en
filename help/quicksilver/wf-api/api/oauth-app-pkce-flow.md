---
content-type: api
navigation-topic: api-navigation-topic
title: Using PKCE flow for OAuth 2 applications
description: Using PKCE flow for OAuth 2 applications
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
---
# Configure and use your organization's custom OAuth 2 applications using PKCE flow

PKCE is a secure authorization flow that works well with dynamically refreshing applications such as mobile apps, but is valuable across all OAuth2 clients. Instead of a static client secret, PKCE uses a dynamically generated string, eliminating the risk of a leaked client secret.

## PKCE overview

A PKCE flow has the following steps. The steps in this section are presented for information only. To perform these procedures, see other sections in this article.

1.  The client creates the `code_challenge` by transforming the `code_verifier` using `S256` encryption.
    
1.  The client directs the browser to the OAuth2 sign-in page, along with the generated `code_challenge`. You must register your app (Client) so that OAuth2 can accept the authorization request. After registration, your app can redirect the browser to OAuth2.
    
1.  The OAuth2 Authorization Server redirects the authentication prompt to the User.
    
1.  The User authenticates using one of the configured login options, and may see a consent page listing the permissions OAuth2 will give to the application.
    
1.  OAuth2 redirects back to your application with an `authorization code`.
    
1.  Your application sends this code, along with the `code_verifier`, to OAuth2.
    
1.  OAuth2 Authorization Server transforms the `code_verifier` using the `code_challenge_method` from the initial authorization request, and checks the result against the `code_challenge`. If the value of both strings match, then the server has verified that the requests came from the same client and will issue an `access token`.
    
1.  OAuth2 returns the `access token`, and optionally a `refresh token`.
    
1.  Your application can now use these tokens to call the resource server such as an API on behalf of the user.
    
1.  The resource server validates the token before responding to the request.
    

## Configure your application

Before you can implement authorization, you need to register your app in OAuth2 by creating an app integration from Workfront.

For instructions on creating the OAuth2 application, see [Create an OAuth2 single-page web application using PKCE ](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [Create OAuth2 applications for Workfront integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## Create the Proof Key for Code Exchange

Similar to the standard Authorization Code flow, your app starts by redirecting the user's browser to your Authorization Server's `/authorize` endpoint. However, in this instance you also have to pass along a code challenge.

Your first step is to generate a code verifier and challenge.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Code verifier</td>
        <td>
          <p>Random URL-safe string with a minimum length of 43 characters</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Code challenge</td>
        <td>
          <p>Base64 URL-encoded SHA-256 hash of the code verifier</p>
        </td>
      </tr>
    </tbody>
</table>


You must add code in your client app to create the code verifier and code challenge.

The PKCE generator code creates output similar to the following:

>[!INFO]
>
>**Example:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

Your app saves the `code_verifier` for later, and sends the `code_challenge` along with the authorization request to your Authorization Server's `/authorize` URL.

## Request an authorization code

If you are using the default Custom Authorization Server, then your request URL would be similar to the following:

>[!INFO]
>
>**Example:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Note the parameters that are being passed:

*   `client_id` matches the Client ID of the OAuth2 application that you created in the when configuring the application.
    
    For instructions, see Create an OAuth2 single-page web application using PKCE in Create OAuth2 applications for Workfront integrations.
    
*   `response_type` is `code`, because the application uses the Authorization Code grant type.
    
*   `redirect_uri` is the callback location that the user agent is directed to along with the `code`. This must match one of the redirect URls that you specified when you created your OAuth2 application.
    
*   `code_challenge_method` is the hash method used to generate the challenge, which is always `S256` for Workfront Oauth2 applications that use PKCE.
    
*   `code_challenge` is the code challenge used for PKCE.
    

## Exchange the code for tokens

To exchange the authorization code for an access token, pass it to your Authorization Server's `/token` endpoint along with the `code_verifier`.

>[!INFO]
>
>**Example:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> Unlike the regular Authorization Code flow, this call doesn't require the Authorization header with the Client ID and secret. That is why this version of the Authorization Code flow is appropriate for native apps such as mobile applications or single-page application that do not have a backend.

Note the parameters that are being passed:

*   `grant_type` is `authorization_code`, because the app uses the the Authorization Code grant type.
    
*   `redirect_uri` must match the URI that was used to get the authorization code.
    
*   `code` is the authorization code that you received from the /authorize endpoint.
    
*   `code_verifier` is the PKCE code verifier that your app generated in [Create the Proof Key for Code Exchange](#Create).
    
*   `client_id` identifies your client and must match the value preregistered in OAuth2.
    

If the code is still valid, and the code verifier matches, your application receives an access token.

>[!INFO]
>
>**Example:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## Validate the access token

When your application passes a request with an access token, the resource server needs to validate it.

You can validate your access token with an API call similar to the following:

>[!INFO]
>
>**Example:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Request a refresh token

To request a refresh token, you can make a POST call to the API, similar to the following:

>[!INFO]
>
>**Example:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
