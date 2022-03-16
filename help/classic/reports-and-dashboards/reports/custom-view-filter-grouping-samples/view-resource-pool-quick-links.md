---
filename: view-resource-pool-quick-links
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: View: Resource Pool quick links
description: This view contains all of the left-hand navigation options for a resource pool. The idea behind this view is to build a Resource Pool report that can be placed on a Portfolio Manager, Resource Manager, or Executive's Dashboard, reducing the number of clicks navigating to these Resource Management tools.
---

# View: Resource Pool quick links

## Description

This view contains all of the left-hand navigation options for a resource pool. The idea behind this view is to build a Resource Pool report that can be placed on a Portfolio Manager, Resource Manager, or Executive's Dashboard, reducing the number of clicks navigating to these Resource Management tools.

## Preview

![](assets/view--resource-pool-quick-links-350x76.png)

### Text Mode Code

<pre>column.0.descriptionkey=displayorder<br>column.0.linkedname=direct<br>column.0.listsort=intAsInt(displayOrder)<br>column.0.namekey=displayorder.abbr<br>column.0.querysort=displayOrder<br>column.0.shortview=false<br>column.0.stretch=0<br>column.0.valuefield=displayOrder<br>column.0.valueformat=int<br>column.0.width=55<br>column.1.descriptionkey=name<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=direct<br>column.1.listsort=string(name)<br>column.1.namekey=name.abbr<br>column.1.querysort=name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Edit Resource Pool<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.page=/resourcePoolOpen.cmd<br>column.2.link.valuefield=objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=direct<br>column.2.listsort=string(name)<br>column.2.name=Edit<br>column.2.querysort=name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.value=Edit Pool<br>column.2.valueformat=HTML<br>column.2.width=75<br>column.3.description=View Capacity Planner<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.page=/resourcePoolEditProjBudgets.cmd<br>column.3.link.valuefield=objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=direct<br>column.3.listsort=string(name)<br>column.3.name=Plan<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.value=Plan<br>column.3.valueformat=HTML<br>column.3.width=80<br>column.5.descriptionkey=description<br>column.5.linkedname=direct<br>column.5.listsort=string(description)<br>column.5.namekey=description.abbr<br>column.5.querysort=description<br>column.5.shortview=false<br>column.5.stretch=100<br>column.5.valuefield=description<br>column.5.valueformat=HTML<br>column.5.width=150</pre>