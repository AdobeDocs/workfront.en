---
title: Fourth Quarter 2026 Financial Management enhancements
description: Fourth Quarter 2026 Financial Management enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Fourth Quarter 2026 Financial Management enhancements

This page describes Financial Management enhancements made with the Fourth Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Fourth Quarter 2026 release cycle, see [Fourth Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Enhancements to company billing rates

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Multiple updates have been made to the company billing rates functionality.

### For customers on all Workfront and Workflow packages

* We have updated the dialog boxes for adding and editing company billing rates with a more modern design that is consistent with other areas of Workfront.
* The "Allow company-level billing rates to override project-level billing rates" setting properly adds the rate overrides when a company is added to a project, and the planned revenue calculations use the company-level billing rates.
* Users without access to Edit General Finance and Edit Billing Rates at the project level can no longer add a company to a that project.

### For customers on the Workflow Ultimate package only

Rate attributes are now available to apply to company-level billing rates. Effective dates can also be applied to company rates.

NOTE: Company-level rates have not been added to the rate hierarchy.

For more information, see [Override job role billing rates at the company level](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md) and [Override Project-Level Billing Rates with Company-Level Billing Rates](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Attribute hierarchies now stay connected automatically

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026
>This feature is only available for organizations on the Workflow Ultimate package.

When using rate attributes as filters in various areas of Workfront such as Advanced Assignments, additional validation is now applied to parent-child filtering.

Previously, if you linked one attribute to a parent, and that parent to a grandparent, the system didn't automatically recognize the original attribute as belonging to the grandparent too. Now when you choose the lowest level attribute, every level above it is assigned automatically.

For information about attributes, see [Define rate attributes](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).
