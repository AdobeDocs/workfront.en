---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Troubleshooting - corrupted interface font in proofing viewer on Mac
description: If you notice that the proofing viewer does not display interface font properly, this could be due to some issues with the fonts on your Mac machine. To resolve the problem, try the following solutions - EDIT ME.
feature: "Workfront Proof, Digital Content and Documents"
---

# Troubleshooting - corrupted interface font in proofing viewer on Mac

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

If you notice that the proofing viewer does not display interface font properly, this could be due to some issues with the fonts on your Mac machine. To resolve the problem, try the following solutions:

## Remove font duplicates

Check whether there are any duplicate fonts in the system.

1. Close the browser you are using.
1. Open the Font Book application in your Applications folder.
1. Click **All Fonts** (1).
1. Click&nbsp;**Edit** > **Look for Enabled Duplicates**.

1. Click **Yes** to resolve duplicates.
1. If you see a warning about corrupted fonts, click **Yes**.
1. Restart your computer.
1. Retry the proof.

## Clear the font cache

Sometimes, the font caches in Mac OS X become corrupted. For example, when a font or a family of fonts is reinstalled&nbsp;a number of times&nbsp;or if an application has been updated or reinstalled. Apart from the&nbsp;operating system's font cache files, some&nbsp;applications may have their own font cache.&nbsp;Deleting these font cache files can resolve issue with garbled text.

Firstly, you will need to launch Font Book, select the font or family that you are having trouble with, and press the Delete button on your keyboard. You may also right-click and select Remove Family. If you are unsure which font or family is causing the issues, you may want to try first removing duplicates as described above.

The second step would be to clear the&nbsp;font cache and there are several&nbsp;ways to&nbsp;achieve this.

The first is to simply reboot into Safe Mode by holding the Shift key immediately when you hear the boot chimes at startup. When this mode loads, a progress bar should appear, during which the system will run various checks and maintenance routines, one of which is to clear the font cache.

The second approach is to use the Terminal, which can be done by running the following command from within an administrative account:&nbsp;*sudo atsutil databases -remove*

>[!NOTE]
>
>This command will require you to enter your password, which will not be shown when typed. We recommend consulting with your IT department as this may require Administrator permissions on your machine.

Another approach would be to use a font cache utility such as e.g. FontNuke and clear the cache with its&nbsp;help.

Many prepress and artworking/design studios also use Universal Type Server software to manage licensing and distribution of fonts. Sometimes, a problem can occur with the&nbsp;Universal Type&nbsp;Server&nbsp;Font Cache, which can cause the Workfront Proof annotations to disappear.

To fix, clear the Universal Type Server Font Cache and restart Universal Type Server.

## Fix Flash font conflict

You might not have access to this functionality because it is supported by Flash, which has been deprecated in most environments.

The Legacy proofing viewer is based on Flash Player&nbsp;and sometimes, when the text is missing in the proofing viewer, it is possible&nbsp;there is&nbsp;a font conflict between OS X and Flash Player. Try the following:

1. Open Finder and open the&nbsp;**Go** tab.
1. Press the Option&nbsp;key (⌥ Alt) to open the Library folder in the dropdown list.
1. While holding the Option key, click the&nbsp;Library folder.
1. After the Library folder opens, go to Fonts folder located within.
1. Move all the fonts located in&nbsp;the Fonts folder&nbsp;into another folder, perhaps on your Desktop (please do not&nbsp;create&nbsp;another folder inside the Fonts folder).   
1. &nbsp;This action hides all your custom fonts; you should still have the standard system fonts saved in their separate location.
1. Quit and restart Safari.
1. Reopen the&nbsp;proof.

You should see your fonts now. If you don't need any of the fonts that you removed from your home directory, you can safely delete them. Otherwise, go through them in batches, copy them back to your Library/Fonts folder, and see which one is causing the problem.
