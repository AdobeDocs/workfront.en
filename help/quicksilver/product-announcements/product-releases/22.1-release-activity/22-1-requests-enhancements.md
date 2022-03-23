

# 22.1 Requests enhancements

This page describes all Requests enhancements made with the 22.1 release to the Preview environment. These enhancements will be made available in the Production environment 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

the week of January 17, 2022.

For a list of all changes available with the 22.1 release, see [22.1 Release overview](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Interface improvement for users who don’t have access to create requests

To improve users’ experience when working with requests, we have introduced an improvement to the interface that indicates to the logged-in user that they do not have access to create requests. With this improvement, the New request button is dimmed for users without access to create issues. Hovering over the dimmed button displays a tooltip that explains that the Workfront administrator restricted the current user’s access to create requests.

Prior to this enhancement, the New request button did not display in the Requests area for these users. Copying and submitting a request as new is also restricted.

For more information about creating requests, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copy and submit requests

To optimize your process for submitting requests, we are introducing new functionality that allows you to copy an existing request and submit it as a new request. This is helpful when you submit similar requests frequently. In this case, you can reuse an existing request, make a few changes, then submit it as a new request.

With this change, users who can view requests that others submitted can also copy these requests and submit them as new. You can prevent this from happening by updating the following setting in the request queue project:&nbsp;People from the same company will inherit the same permissions for all requests.

>[!NOTE]
>
>You cannot copy and resubmit issues that were submitted to a request queue without a queue topic before this functionality was released.

For more information, see [Copy and submit requests](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

```<iframe class="vimeo-player_0" src="assets/647433535?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>```

[View this video in full-screen mode.](https://vimeo.com/647433535/32c681ac04)

## Updated Summary panel experience in the Submitted section of the Requests area

>[!NOTE]
>
>This feature was temporarily removed from the Preview environment on November 12, 2021. It will be re-added at a later date.

To improve visibility and interaction with the Summary panel, we have added a label to the Open Summary icon in the Submitted section of the Requests area. The label is now dynamic and it updates depending on whether the panel is open or closed.

When opening the Summary panel without first selecting a request, a more user-friendly image now displays to clearly instruct the user to select an item before opening the panel. For more information, see [Locate submitted requests](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

With this change, the Summary panel for tasks, issues, and documents has also been updated. For information about the Summary panel, see [Summary overview in the new Adobe Workfront experience](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
