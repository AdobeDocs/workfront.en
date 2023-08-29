---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager permissions troubleshooting
description: The permission profiles available in [!DNL Adobe] Workfront for proofing users are Administrator, Supervisor, and Manager.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
---
# [!UICONTROL [!DNL Workfront] Proof Manager] permissions troubleshooting

Following are the permission profiles available in [!DNL Adobe Workfront] for proofing users:

* [!UICONTROL Administrator]
* [!UICONTROL Supervisor]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

When granting a user [!UICONTROL Manager] permissions, the following troubleshooting information is available:

* **PROBLEM:** Users with [!UICONTROL Manager] permissions cannot view proofs created by other users. Instead, they see the [!UICONTROL Access Denied] screen. 

   ![](assets/access-denied-350x161.png)

   **SOLUTION:** Users with [!UICONTROL Manager] permissions must be explicitly added to the proofs. Proofs should always be created via the [!UICONTROL Advanced proofing options] window and users should always be added via this option.

* **PROBLEM:** Users with [!UICONTROL Manager] permissions cannot add proof versions to the proofs created by other users (they could potentially submit a proof in the documents set, but the versions would NOT be connected to the original set created by another user).\
   **SOLUTION:** Users with [!UICONTROL Manager] permissions can submit the versions to another user's proof only if the user with [!UICONTROL Manager] permissions when both of the following :

   * Explicitly added to the proofs
   * Set as [!UICONTROL Authors] (proof role) on the proofs

* **PROBLEM:** Users with [!UICONTROL Manager] permissions cannot edit comments of other users on a proof they do not own or they did not create.\
   **SOLUTION:** If users with [!UICONTROL Manager] permissions do not own the proofs, but they should be able to edit comments, add them as [!UICONTROL Authors] (or [!UICONTROL Moderators]).\
   These three types of permissions are available in [!DNL Workfront] for [!UICONTROL Planner], [!UICONTROL Worker], [!UICONTROL Requester], [!UICONTROL Reviewer] type licenses. System Administrator or User Admin in [!DNL Workfront] can edit Users' profiles and adjust [!DNL Workfront Proof] permissions from there. 
