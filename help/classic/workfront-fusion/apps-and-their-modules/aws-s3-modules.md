---
filename: aws-s3-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: AWS S3 modules
description: The Adobe Workfront Fusion AWS S3 modules let you perform operations on your S3 buckets.
---

# AWS S3 modules

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

The Adobe Workfront Fusion AWS S3 modules let you perform operations on your S3 buckets.

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
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
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
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

## Prerequisites

To use AWS S3 modules, you must have an Amazon Web Service account.

## Connect AWS to Workfront Fusion {#connect-aws-to-workfront-fusion}

To connect AWS S3 to Workfront Fusion you must connect your AWS account to Workfront Fusion. To do so, you'll first need to create an API user in AWS IAM.

1. Sign in to your AWS&nbsp;AIM&nbsp;account. 
1. Navigate to **Identity and Access Management** > **Access Management** > **Users**.

1. Click **Add User**.
1. Enter the name of the new user and select the **Programmatic access** option in the Access type section.
1. Click **Attach existing policies directly**, then search for **AmazonS3FullAccess** in the search bar. Click it when it appears, then click **Next**.

1. Proceed through the other dialog screens, then click **Create User**.
1. Copy the provided **Access key ID** and **Secret access key**.

1. Go to Workfront Fusion and open the AWS S3 module's **Create a connection** dialog.
1. Enter the Access key ID and Secret access key from step 7 to the respective fields and click **Continue** to establish the connection.

The connection has been established. You can proceed with setting up the module.

## AWS S3 modules and their fields

When you configure AWS S3 modules, Workfront Fusion displays the fields listed below. Along with these, additional AWS S3 fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions) 
* [Searches](#searches)

### Actions {#actions}

* [Create Bucket](#create-bucket) 
* [Get File](#get-file) 
* [Upload File](#upload-file) 
* [Make an API Call](#make-an-api-call)

#### Create Bucket {#create-bucket}

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting yourAWS account to Workfront Fusion, see <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect AWS to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name </td> 
   <td> <p>Enter the name of the new bucket.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Region </td> 
   <td> <p>Select your regional endpoint. For more information, see the discussion of <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regional endpoints</a> in the AWS documentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get File {#get-file}

Downloads a file from a bucket.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting yourAWS account to Workfront Fusion, see <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect AWS to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Region </td> 
   <td> <p>Select your regional endpoint. For more information, see the discussion of <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regional endpoints</a> in the AWS documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bucket </td> 
   <td> <p>Select the bucket you want to download the file from.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Path</p> </td> 
   <td> <p>Enter the path to the file, e.g. <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Upload File {#upload-file}

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting yourAWS account to Workfront Fusion, see <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect AWS to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Region </td> 
   <td> <p>Select your regional endpoint. For more information, see the discussion of <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regional endpoints</a> in the AWS documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Folder (optional) </p> </td> 
   <td> <p>Specify the target folder that you want to upload a file to.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Source file</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Headers (optional)</p> </td> 
   <td> <p> Insert request headers. Available headers can be found in the <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">AWS S3 documentation - PUT object</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Make an API Call {#make-an-api-call}

For a detailed discussion of the Amazon S3 API, see [Amazon S3 REST API Introduction](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting yourAWS account to Workfront Fusion, see <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect AWS to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Region </td> 
   <td> <p>Select your regional endpoint. For more information, see the discussion of <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regional endpoints</a> in the AWS documentation.</p> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>URL Enter a host URL. The path must be relative to<code> https://s3.&lt;selected-region&gt;.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Headers</td> 
   <td> <p>Add a request header. You can use the following common request headers. For more request headers refer to <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">AWS S3 API Documentation</a>.</p> <p>You don't have to add authorization headers; Workfront Fusion 2.0 already did that for you.</p> 
    <table> 
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>Header Name</th> 
       <th> <p> Description</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>Content-Length</p> </td> 
       <td> <p>Length of the message (without the headers) according to RFC 2616. This header is required for PUTs and operations that load XML, such as logging and ACLs.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>Content-Type</p> </td> 
       <td> <p>The content type of the resource, in case the request content is in the body. Example: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>Content-MD5</p> </td> 
       <td> <p>The base64 encoded 128-bit MD5 digest of the message (without the headers) according to RFC 1864. This header can be used as a message integrity check to verify that the data is the same data that was originally sent. Although it is optional, we recommend using the Content-MD5 mechanism as an end-to-end integrity check. For more information about REST request authentication, go to <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">REST Authentication</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>Date</p> </td> 
       <td> <p>The current date and time according to the requester. Example: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. When you specify the <code>Authorization </code>header, you must specify either the <code>x-amz-date</code> or the <code>Date </code>header.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>Expect</p> </td> 
       <td> <p>When your application uses 100-continue, it does not send the request body until it receives an acknowledgment. If the message is rejected based on the headers, the body of the message is not sent. This header can be used only if you are sending a body.</p> <p>Valid Values: 100-continue</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>Host</p> </td> 
       <td> <p>For path-style requests, the value is <code>s3.amazonaws.com</code>. For virtual-style requests, the value is <code>BucketName.s3.amazonaws.com</code>. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Virtual Hosting</a> in the <i>Amazon Simple Storage Service Developer Guide</i>.</p> <p>This header is required for HTTP 1.1 (most toolkits add this header automatically); optional for HTTP/1.0 requests.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>x-amz-content-sha256</p> </td> 
       <td> <p>When using signature version 4 to authenticate the request, this header provides a hash of the request payload. When uploading an object in chunks, set the value to <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> to indicate that the signature covers only headers and that there is no payload. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Signature Calculations for the Authorization Header: Transferring Payload in Multiple Chunks (Chunked Upload) (AWS Signature Version 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>x-amz-date</p> </td> 
       <td> <p>The current date and time according to the requester. Example: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. When you specify the <code>Authorization </code>header, you must specify either the <code>x-amz-date</code> or the <code>Date </code>header. If you specify both, the value specified for the <code>x-amz-date</code> header takes precedence.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>x-amz-security-token</p> </td> 
       <td> <p>This header can be used in the following scenarios:</p> 
        <ul> 
         <li>Provide security tokens for Amazon DevPay operations. Each request that uses Amazon DevPay requires two <code>x-amz-security-token</code> headers: one for the product token and one for the user token. When Amazon S3 receives an authenticated request, it compares the computed signature with the provided signature. Improperly formatted multi-value headers used to calculate a signature can cause authentication issues.</li> 
         <li>Provide a security token when using temporary security credentials. When making requests using temporary security credentials you obtained from IAM, you must provide a security token using this header. To learn more about temporary security credentials, go to Making Requests.</li> 
        </ul> <p>This header is required for requests that use Amazon DevPay and requests that are signed using temporary security credentials.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>Query String</td> 
   <td> <p>Add the desired query strings such as parameters or form fields.</p> </td> 
  </tr> 
  <tr> 
   <td>Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:   <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Searches {#searches}

* [List Files](#list-files) 
* [List Folders](#list-folders)

#### List Files {#list-files}

Returns a list of files from a specified location.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting yourAWS account to Workfront Fusion, see <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect AWS to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Region </td> 
   <td> <p>Select your regional endpoint. For more information, see the discussion of <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regional endpoints</a> in the AWS documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bucket </td> 
   <td> <p>Select the Amazon S3 bucket you want to search for files.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Prefix (optional)</p> </td> 
   <td> <p> Path to a folder to look up files in, e.g. <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Folders {#list-folders}

Returns a list of folders from a specified location.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting yourAWS account to Workfront Fusion, see <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect AWS to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Region </td> 
   <td> <p>Select your regional endpoint. For more information, see the discussion of <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regional endpoints</a> in the AWS documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bucket </td> 
   <td> <p>Select the Amazon S3 bucket you want to search for folders.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Prefix (optional)</p> </td> 
   <td> <p> Path to a folder to look up folders in, e.g. <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

