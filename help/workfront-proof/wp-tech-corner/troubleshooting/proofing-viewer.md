---
filename: proofing-viewer
content-type: tips-tricks-troubleshooting
product: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Troubleshooting - Workfront Proof proofing viewer
description: Important: This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see Proofing.
---

# Troubleshooting - *Workfront Proof* *proofing viewer*

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product *Workfront Proof*. For information on proofing inside *Adobe Workfront*, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

If your *proof* content is not loading and you can only see an empty *proofing viewer*, it’s most likely because something is blocking this action locally. Try the possible solutions below.

## Ensure&nbsp;Your Browser and Flash Player Versions are Up-to-Date

All developers constantly work on their applications and they regularly release new features and fixes for their products. This is to improve user experience and maintain security level so it’s the best practice to use only the newest versions. This also helps avoiding conflicts between the applications.

### Flash Player Plugin Version

To check your current Flash Player version visit the [Adobe website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [Flash Player download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original Adobe plugin, so if your browser uses a built-in solution deactivate it and install the Adobe solution.

### Browser Version

Nowadays most of the browsers update automatically, but if you’re experiencing any troubles it’s worth checking what version you’re using and perform update, if needed.

In your browser go to Menu and locate the About option (in some cases this may be visible under Help menu). In the About pop-up you’ll find information about the current browser version and also an option to update/check for updates.

Please see in Chrome:

![ProofView_3.png](assets/proofview-3-350x206.png)

Once your have the latest Flash Player plugin and browser version installed try to re-open your *proof* and see if the issue is resolved.

## Ensure&nbsp;Your Local Flash Storage is Available

Our *Workfront Proof* Viewer is based on Flash, and we store some data about the *proofs* (i.e., comments, *proof* tiles, *Workfront* Proof Viewer settings) on your computer using Flash Player. If the *Workfront Proof* Viewer opens, but there is no content inside you will want to make sure that the Flash Storage is available on your machine and that *Workfront Proof* is allowed to use it.

If there is some storage allocated, but you’re working with the bigger *proofs* with multiple pages and comments try to increase the Flash Storage and re-load your *proof*.

Please see our [Problems With Viewing Proofs - Flash Shared Objects Explained](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md)&nbsp;for the detailed instructions.

## Identify Where the&nbsp;Problem Is

<ul> 
 <li> Are the <em>proofs</em> opening in a different browser?&nbsp;</li> 
 <li>If you’re using one browser on a daily basis and you’re having trouble with viewing the <em>proofs</em> there try to open the same <em>proof</em> in a different browser on your computer. To do this simply copy the <em>proof</em> link from the URL bar of your main browser and paste it into a different browser. If the <em>proof</em> opens ok there, review your main browser configuration, plugins and extensions as these may be interfering.</li> <note type="note">
  We do not have any preferable browser, but if you’re having any performance issues in your current browser we would advise&nbsp;switching to a different one. 
 </note> 
 <li>Are the <em>proofs</em> opening on a different machine in your location?<br>If your <em>proof</em> is not opening in any browser on your machine try to open it on a different computer in your location and/or outside your location. This will allow you to determine if an issue is down to your particular machine or if it’s something in your local network.<br>If your security level is higher your connections to <em>Workfront Proof</em> may be blocked by: 
  <ul>
   <li>Your local AV software</li>
   <li>Your network security solution</li>
   <li>DNS, firewall or proxy configuration</li><note type="note">
    These are the settings that are beyond&nbsp;our control. There are various security solutions available and we are not able to tell which are implemented in your network and which may be blocking connections to 
    <em>Workfront Proof</em>. It is also not up to 
    <em>Workfront</em> Proof to decide on your internal security configuration. If you’re having problems with opening the 
    <em>proofs</em> on the multiple machines in your location/network we would recommend you to get in touch with your IT team so they could check the network settings and authorize or add the 
    <em>Workfront</em> Proof to the allowlist, if needed.
   </note>
  </ul></li> 
 <li> Are the connections to <em>Workfront Proof</em> allowed in your network?<br>Inside the Proof Viewer we load the tiles - fragments of the pages. If this content does not load ok at your end it may be that some connections to <em>Workfront Proof</em> are blocked in your network. You will want to make sure that all connections and all content from *.proofhq.com is added to the allowlist. Your IT team should be able to help with verifying this.&nbsp;</li> 
</ul>

## Review Plugins

If your browser and Flash Player plugin is up-to-date and your network is not blocking the connections to *Workfront Proof* there may be something in your browser that is affecting viewing the *proofs*. Nowadays there are multiple plugins and extensions available in your browser and some of them interfere or are in conflict with the others.

The best practice is to remove all the unknown add-ons and keep only the ones that you use and that you trust. Each browser should give you options to check/modify/delete the plugins and extensions. Our *Workfront Proof* Viewer is based on Flash and we use JavaScript to load the viewer so you will want to especially review the plugins that could affect these.

Please visit the pages listed below for more detailed instructions from the developers on how to disable the browser add-ons:

* Chrome: [plugins](https://support.google.com/chrome/answer/142064?hl=en-GB)&nbsp;/ [extensions](https://support.google.com/chrome/answer/113907?hl=en-GB)

* Firefox: [add-ons](https://support.mozilla.org/en-US/kb/disable-or-remove-add-ons)
* Internet Explorer: [add-ons](http://windows.microsoft.com/en-GB/internet-explorer/manage-add-ons#ie=ie-11)
* Safari: [add-ons](http://support.apple.com/en-gb/HT203353)

If there is any particular add-on interfering with loading the *proofs* you can try checking the details in the browser’s console.

![ProofView_4.png](assets/proofview-4-350x57.png)

In most of the newer browsers there are some additional Developers tools available and they can be used for more advanced troubleshooting.

If you’re having troubles with viewing the *proofs*:

* Open your browser’s console and re-load the *proof*.
* Check if there are any alerts or messages in the console. These details can help identifying what’s the root cause of the issues.
* Have your IT team to analyze the results. They should be able to advise and help resolving the local problem.
* Share the results with our [Support team](https://support.workfront.com/hc/en-us/requests/new). We&nbsp;will be happy to assist.

If you don’t know how to open the console in your browser, please see the recorded steps:

* [Firefox](http://screencast.com/t/eP6FRtk4vxWS) 
* [Internet Explorer](http://screencast.com/t/bYzq1iQv) 
* [Google Chrome](http://screencast.com/t/2anpeAzOOyj) 
* [Safari](http://screencast.com/t/rnOvgl3GidjL)

You can also check your browser developer’s documentation for more detailed instructions.

## Check Mixed Content Settings

All of the connections to *Workfront Proof* are over HTTPS. However, in the *Workfront* Proof Viewer we load the tiles over HTTP and the data is secured with the tokens. This creates Mixed Content that some of the browsers or security solutions may be blocking (by default or as per manual configuration).

If this is the reason why the *proofs* are not opening on your computer (you should be able to see the relevant alerts in the browser’s console) authorize such connections for *Workfront Proof* or amend your settings to allow passive mixed content on your machine. The mixed content may be blocked by your browser, AV software, network configuration etc - to determine the exact cause please get in touch with your IT team/network administrators. They should also be able to help with enabling the mixed content on your machine.

Contact our [Support team](https://support.workfront.com/hc/en-us/requests/new) if you need any assistance from our end.
