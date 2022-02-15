---
filename: how-access-levels-permissions-work-together
title: How access levels and permissions work together
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,diagram,levels,permissions
navigation-topic: access-levels
---




# How access levels and permissions work together {#how-access-levels-and-permissions-work-together}

When User A shares a `Workfront` object with User B, User B's access to the object is determined by a combination of two things:



* User B's access level, assigned by the `Workfront administrator`. 
* User B's permissions to the object, specified by User A.


User B's actions on the object can be further restricted on the object, but they cannot be unrestricted beyond is allowed on his access level.&nbsp;


For example:



*  If User B's access level doesn't allow him to create tasks, he can't add tasks to the object, even if User A gave him permissions to add tasks to it. 
*  If User B's access level does allow him to create tasks, but User A did not grant permissions to add tasks to the project, he can't add tasks to the object, but he can add tasks to other objects where he has been granted permissions to do so.


Permissions in `Workfront` are inherited hierarchically. For more information about inherited permissions, see the [Understand inherited Permissions](sharing-permissions-on-objects.md#understanding-inherited-permissions) section in [Share Permissions on objects](sharing-permissions-on-objects.md).


For more information about permissions, see [Permissions in the access model](permissions-in-the-access model.md).


For information about license types and access levels, see [Create or modify access levels](create-modify-access-levels.md).
