---
filename: deactivate-user-api
content-type: api
product-area: user-management
navigation-topic: general-api
title: Deactivate a User via the API
description: When a user leaves your organization, you can deactivate the user, making their Adobe Workfront license available for another user and preventing them from being inadvertently assigned work. By deactivating a user, you preserve their work history, including their work assignments and their association with notes, hours, and documents.
---

# Deactivate a User via the API

When a user leaves your organization, you can deactivate the user, making their Adobe Workfront license available for another user and preventing them from being inadvertently assigned work. By deactivating a user, you preserve their work history, including their work assignments and their association with notes, hours, and documents.

To learn more about deactivating a user, see " [Deactivate a user](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

For information about using the Core API, see [API basics](../../wf-api/general/api-basics.md).

To deactivate a user via the API:

1. Generate an API key by using the following API request:  
   <pre><strong><domain></strong>.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=<strong>username</strong>&password=<strong>password</strong>&method=PUT</pre>

1. Locate the GUID for the user you want to deactivate.

   1. Use the following API request to retrieve the GUID for all users in your system, note that the **isActive** field shows **true** for users that are currently active and **false** for users that have been deactivated:&nbsp;  
      <pre><strong><domain></strong>.my.workfront.com/attask/api/v7.0/USER/search?fields=isActive</pre>

1. Locate the GUID for the user you want to deactivate, use the following **PUT** request to change the user's **isActive** field value to **false**:&nbsp;  
   <pre><strong><domain></strong>.my.workfront.com/attask/api/v7.0/USER/<strong><user's GUID></strong>?updates={"isActive":"false"}&method=put&apiKey=<strong><apiKey></strong>&fields=isActive</pre>

1. The response will show that the **isActive** field value has changed&nbsp;from **true** to **false**indicating that the user has been deactivated:

[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>