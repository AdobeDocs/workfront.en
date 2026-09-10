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
TQID: https://experienceleague.adobe.com/N6spdHNxoRMwUjQY6HrHPm11d7kZaYHMbDGAkeqbyvY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Environment promotion troubleshooting

This article describes how to troubleshoot environment promotion.

## Problem: Environment promotion package is stalling or failing

If your environment promotion package is stalling or failing, try the following:

* If a package installation stalls after 10-15 minutes, or if a package installation is failing, reassemble the existing package or create a new package.

* If a package installation fails, there may be an issue with one or more objects. Check the error messages, which identify the object and can help identify the issue. After you address the issue with the object, reassemble the package and reattempt the install.

* If you are still having problems with an installation, try replicating the installation in a different target environment. Keep as close as possible to the original installation, including objects and install actions selected.

* We recommend always checking the package contents after the package has been assembled to confirm that it contains the objects you expect.


## Problem: Custom form fails to promote

This may occur because the custom form includes a calculated field. If a calculated field references a field that is not referenced in a custom form, a package that includes this form does not promote, and the user may see the following message:

"The following fields are invalid: Invalid Custom Expression Invalid Expression: Invalid Custom Expression."

This issue can arise when referencing an existing field that is not attached to any custom forms in the target environment, or with a newly created field.

To resolve this issue, do one of the following:

* Create a package with a project-type custom form that includes the referenced field. After promoting this package to the target environment, promote the originally intended package containing the calculated field.
* Manually create the referenced field in the target environment and associate it with a project-type custom form. After this is done, the field will be recognized, and you can promote the package without encountering the error.
