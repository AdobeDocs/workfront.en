---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Environment promotion troubleshooting
description: Troubleshoot common issues with environment promotion.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
---
# Environment promotion troubleshooting

If a package installation stalls after ~10-15 minutes (something is wrong) or if a package installation is failing, startover from the beginning (ie. reassemble the existing package or create a new package). Fixes released will only impact newly assembled packages.

If a package installation fails, a common root cause is one or more of the objects selected. Address the issue with the object, reassemble the package and reattempt the install.

If still having problems, try replicating the installation in another environment as close as possible including objects and install actions selected.

Check the package contents after the package has been assembled to confirm that it has what you expect.
