

# HTTP modules

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
The HTTP app provides various modules for communication based on Hypertext Transfer Protocol (HTTP) protocol. HTTP is the foundation of data communication for the World Wide Web. You can use the modules to download web pages and files, call webhooks and API endpoints, and so on.

The right choice of the module depends on the authentication/authorization mechanism the resource you want to access employs:

* Make a request - universal module primarily intended for resources not employing any type of authentication/authorization
* Make a Basic Auth request - for resources employing HTTP Basic authentication (BA)
* Make a OAuth 2.0 request - for resources employing OAuth 2.0 authorization protocol
* Make a Client Certificate Auth request - for resources employing authorization protocol that requires a client-side certificate.

## Make a request

HTTP > Make a request module is a universal module that enables you to configure an HTTP request and submit it to a server. The received HTTP response is then contained in the output bundle.

>[!NOTE]
>
>To make sure your JSON is valid, you may use one of the available online services (e.g. [https://jsonlint.com/](https://jsonlint.com/)) or employ JSON > Create JSON module to create the JSON dynamically and take care of all the necessary escaping>
><!-->
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(see our tutorial>
><a href="make-an-http-request-with-an-api-key.md" class="MCXref xref" xrefformat="{para}">Use JSON Generator to create a JSON Data Structure and make an HTTP request using an API Key (SendGrid example)</a> for detailed explanation)>
></MadCap:conditionalText>>
>-->
>. Mixing JSON pieces with expressions and items directly in the Request content field is not recommended as it can result in invalid JSON.

## Make a OAuth 2.0 request

In order to make an HTTP(S)request to servers that require a OAuth 2.0 authorization, you first need to create a OAuth connection.

### Creating a connection

1. Create a OAuth client in the target service with which you want Workfront Fusion to communicate with. This option will mostly likely be found in the Developer section of the given service. When creating the client, you will be asked to specify a so called 

   ```
   Redirect URL
   ```

   (sometimes called as 

   ```
   Callback URL
   ```

   ). Always enter 

   ```
   https://app.workfrontfusion.com/oauth/cb/oauth2
   ```

   in this field.

   Once you have created the client, the given service will display two keys 

   ```
   Client ID
   ```

   and 

   ```
   Client Secret
   ```

   . Some services call these 

   ```
   App Key
   ```

   and 

   ```
   App Secret
   ```

   . Make sure you write down these keys, you will be asked to provide them when creating the connection in Workfront Fusion.

1. Find the 

   ```
   Authorize URI
   ```

   and 

   ```
   Token URI
   ```

   in the API documentation of the given service (if the service uses Implicit flow, you will need only 

   ```
   Authorize URI
   ```

   ). These are URL addresses through which Workfront Fusion communicates with the target service. The addresses serve for OAuth authorization.

   Examples of Yahoo addresses:

   * Authorize URI:    
   
     ```   
     https://api.login.yahoo.com/oauth2/request_auth
     ```   
   
   * Token URI:    
   
     ```   
     https://api.login.yahoo.com/oauth2/get_token
     ```

1. If the target service uses scopes (access rights), check how the service separates individual scopes and make sure you set the separator in the advanced settings accordingly. If the separator is not set correctly, Workfront Fusion will fail to create the connection and you will receive an invalid scope error.
1. Once you have completed the steps above, you can start to create the OAuth connection in Workfront Fusion. Add the OAuth 2.0 HTTP(S) request and response processing module to your scenario and in the Connection section click on the Add button.

   Screenshot

## Advanced information

* [Standard authorization parameters](#standard-authorization-parameters) 
* [Requesting Access tokens - standard parameters](#requesting-access-tokens-standard-parameters) 
* [Requesting Refresh tokens - standard parameters](#requesting-refresh-tokens-standard-parameters) 
* [Authorized request made to a service](#authorized-request-made-to-a-service)

### Standard authorization parameters {#standard-authorization-parameters}

* response_type: 

  ```
  code
  ```

  for Authorization Code flow and 

  ```
  token
  ```

  for Implicit flow

* redirect_uri: 

  ```
  https://app.workfrontfusion.com/oauth/cb/oauth2
  ```

* client_id: The Client ID you entered when creating the account

### Requesting Access tokens - standard parameters {#requesting-access-tokens-standard-parameters}

* grant_type: 

  ```
  authorization_code
  ```

* redirect_uri: 

  ```
  https://app.workfrontfusion.com/oauth/cb/oauth2
  ```

* client_id: The Client ID you entered when creating the account
* client_secret: The Client Secret you entered when creating the account
* code: The code returned by authorization request

### Requesting Refresh tokens - standard parameters {#requesting-refresh-tokens-standard-parameters}

* grant_type: 

  ```
  refresh_token
  ```

* refresh_token: The Refresh token obtained together with the Access token
* client_id: The Client ID you entered when creating the account
* client_secret: The Client Secret you entered when creating the account

### Authorized request made to a service {#authorized-request-made-to-a-service}

After the connection is established, the module uses by default the bearer token which is sent in the request header field. The bearer token has the following format: 

```
Authorization: Bearer <access token>
```

When creating a connection, it is possible to adjust where the token shall be located, whether in the header in the 

```
Authorization
```

parameter or in the URL in the query string.

## HTTP message body type and when to use it.

HTTP Message Body is the data bytes transmitted in an HTTP transaction message immediately following the headers if there are any to be used.

* [Raw](#raw) 
* [Multipart/Form-Data](#multipart-form-data) 
* [Application/form-urlencoded](#application-form-urlencoded)

### Raw {#raw}

Screenshot

The Raw body type is generally suitable for most HTTP body requests even is situations where developer documentation does not specify data to send, with the following field option of specifying content type as a form of parsing data.

Screenshot

Despite the content type selected, data is entered in any format that is stipulated or required by the developer documentation.

### Multipart/Form-Data {#multipart-form-data}

Multipart/form-data is an HTTP multipart request that HTTP clients construct to send files and data over to an HTTP module. It is commonly used to upload files to your desired server.

Screenshot

You will notice that when you select application form the input method changes and this entails that from the developer documentation you will have the relevant fields required, same also applies to Multipart/form-data whereby in order to receive files encoded with 

```
multipart/form-data
```

, it is necessary to configure a data structure with a 

```
collection
```

type field that contains the nested fields 

```
name
```

, 

```
mime
```

and 

```
data
```

. So as you can see the way the information is received is different.

### Application/form-urlencoded {#application-form-urlencoded}

This body type is to POST data using 

```
application/x-www-form-urlencoded
```

Screenshot

For 

```
application/x-www-form-urlencoded
```

, the body of the HTTP message sent to the server is essentially one giant query string -- name/value pairs are separated by the ampersand (

```
&
```

), and names are separated by the fields name and value for easy use to you and replacing the equals symbol (=) used in coding. However, after you have configured the above it will look like the example shown below:
<pre>MyVariableOne=ValueOne&MyVariableTwo=ValueTwo</pre>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="Tutorial"></a>Tutorials</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">How to connect Workfront Fusion with any web service using OAuth2 authorization<!--
<MadCap:conditionalText style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
- drafted out until I fix that article
</MadCap:conditionalText>
--></p>
-->

## Generating JSON Web Tokens (JWT)

It is possible to generate a JWT token with the help of built-in functions:

Header:

Screenshot

Code for copy&paste:
<pre>{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}</pre>Payload:

Screenshot

Code for copy&paste:
<pre>{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}</pre>Token:

Screenshot

Code for copy&paste:
<pre>{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}</pre>