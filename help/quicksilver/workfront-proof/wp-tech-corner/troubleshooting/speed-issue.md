---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Speed issues in [!DNL Workfront Proof]
description: This help page can help you determine if any speed issues that you might be experiencing when using [!DNL Workfront Proof] are related to your ISP or [!DNL Workfront Proof]'s content delivery network.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
---
# Speed issues in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

This help page can help you determine if any speed issues that you might be experiencing when using [!DNL Workfront Proof] are related to your ISP or [!DNL Workfront Proof]'s content delivery network.

Speed problems are generally due to the local ISP connection or local internet access setup (for example, where a proxy server is used) and so are unfortunately outside of the control of [!DNL Workfront Proof].

That said, there are a few steps you can take to check your connection speed which will allow for the root cause of the issues you are experiencing to be determined. All of these steps are equally important for the troubleshooting process and we would encourage you to take the time to gather information on all of the listed steps to ensure the most accurate diagnosis of the problem.

Once you gather all the details, we would recommend that you consult with your local IT department to identify any local issues.

## Establish which part of the system is slow

When you use [!DNL Workfront Proof], you might be working with the Dashboard, for example, managing folder content and users or with the [!DNL Workfront Proof] Viewer: conducting a proof review, checking the comments already made, and so on.

Determining which exact part of the system is slow is the first step in troubleshooting speed issues. When you report [!DNL Workfront Proof] being slow, make sure to describe the following:

* Are you experiencing slowness in any other webpages?
* Does the problem occur in the Dashboard or [!DNL Workfront Proof] Viewer?
* Which exact part of the system is slow? (e.g. processing a new proof or opening a comment in [!DNL Workfront Proof] Viewer)

## Run traceroute and ping tests

When you are experiencing performance issues it is important to run the traceroute command to verify the connection. To do this please open the Command Prompt in your system (Terminal in Mac/Linux) and perform the following steps:

1. Type one of the following, then wait for the tracerout to be completed:

   * Windows: **tracert app.proofhq.com** 
   * Mac/Linux: **traceroute app.proofhq.com** 

1. (Windows only) Type **ping app.proofhq.com**.
1. When the ping completes, right-click in the command prompt and Select All.
1. Copy and paste the results into the the reply to your email. 
   Make sure you allow traceroute and ping to finish before sending the results to the Support Team.

## Test connection speed using Speedtest.net

1. Open a browser and go to Speedtest.net.
1. Follow the instructions in the Speedtest knowledge base to test the speed of your internet connection.
1. Copy and paste the results into an email our Support Team.

## Check network tab in the browser console

The web console available in the modern browsers gathers useful information about any network latencies, which will prove helpful for us to determine the root cause of the speed issues you are experiencing.

To check the loading times for a webpage:

1. Open your browser's console and the Network tab.
1. Re-load the page.
1. Take screenshots or record a screencast of the results.
1. Share the results with the Support Team.

Please make sure the screenshot shows all the data—you can expand the console window when taking a screenshot or scroll down in a screencast.

You can also check your browser's documentation for more detailed instructions.

## Check your connection on a different network and machine

Checking whether you experience the same problem with connection speed using a different device or network is a crucial step in the troubleshooting process. Please try switching to a different machine or a mobile device, as well as try using alternative network (e.g. mobile data).

Compare the connection in different combinations: using a different machine on the same network, using the same machine on a different network and using both alternative machine and network, then share the results with the Support Team.
