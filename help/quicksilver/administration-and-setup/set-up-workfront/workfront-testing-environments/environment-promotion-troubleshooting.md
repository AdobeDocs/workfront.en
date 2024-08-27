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
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
---
# Environment promotion troubleshooting

If your environment promotion package is stalling or failing, try the following:

* If a package installation stalls after 10-15 minutes, or if a package installation is failing, reassemble the existing package or create a new package.

* If a package installation fails, there may be an issue with one or more objects. Check the error messages, which identify the object and can help identify the issue. After you address the issue with the object, reassemble the package and reattempt the install.

* If you are still having problems with an installation, try replicating the installation in a different target environment. Keep as close as possible to the original installation, including objects and install actions selected.

* We recommend always checking the package contents after the package has been assembled to confirm that it contains the objects you expect.
