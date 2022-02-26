---
filename: risk-to-net-value-d
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Risk to Net Value (Draft - Alina) in the new Adobe Workfront experience
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Risk to Net Value (Draft - Alina) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
in
<em>the new Adobe Workfront experience</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> in  <em>the new Adobe Workfront experience</em></MadCap:conditionalText>`

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

In the Portfolio Optimizer, the Risk to Net Value indicator measures the Potential Risk value taking into account the Net Value provided by all projects displayed in the Portfolio Optimizer.&nbsp;

For achieving the most efficiency within the portfolio, you want to see that the Risk indicator is low and the Net Value indicator is high.&nbsp;

The Risk value and Net Value indicators are represented from the perspective of how they relate to each other.

Depending on whether you are viewing the Portfolio Optimizer in the Preview or Production environment, the Risk to Net Value indicator calculates differently.&nbsp;

If you view the Portfolio Optimizer in the Production environment, the Risk to Net Value indicator is the same in the New and Legacy Portfolio Optimizer, and it is calculated by the following formula:

* The Risk indicator is calculated by the following formula:  
  *Risk value indicator = Risk / (Risk + Net Value)*

* The Net Value indicator is calculated by the following formulas:   
  *Net Value indicator = 1 - Risk / (Risk + Net Value)* 
  Or  
  *Net Value indicator = Net Value / (Risk + Net Value)*

In the Preview environment, depending on which Portfolio Optimizer you are using, the Risk to Net Value metric is calculated differently:

* `Portfolio Optimizer`

  * `The Risk indicator is calculated by the following formula:  
    *Risk value indicator = Risk / (Risk + Net Value)*` 
  * `The Net Value indicator is calculated by the following formulas:   
    Net Value indicator = 1 - Risk / (Risk + Net Value)   
    Or  
    Net Value indicator = Net Value / (Risk + Net Value)`

* `Legacy Portfolio Optimizer`

  * `The Risk indicator is calculated by the following formula:  
    *Risk value indicator = Risk / (Risk + Legacy Net Value)*` 
  * `The Net Value indicator is calculated by the following formulas:  
    Net Value indicator = 1 - Risk / (Risk + Legacy Net Value)  
    Or  
    Net Value indicator = Net Value / (Risk + Legacy Net Value)`

>[!NOTE]
>
>The Risk to Net Value indicator calculates based on the projects that you display in the Portfolio Optimizer, and not on all the projects which are associated with the portfolio.&nbsp;

For more information about how Net Value is calculated, see "Calculating Net Value."

![risk_to_net_value_indicator_new_optimizer.png](assets/risk-to-net-value-indicator-new-optimizer-350x154.png)

