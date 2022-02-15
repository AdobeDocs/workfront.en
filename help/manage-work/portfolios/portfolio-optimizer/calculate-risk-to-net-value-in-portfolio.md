---
filename: calculate-risk-to-net-value-in-portfolio
product-area: portfolios
navigation-topic: portfolio-optimizer
---



# Calculate the Risk to Net Value in a portfolio {#calculate-the-risk-to-net-value-in-a-portfolio}

In the Portfolio Optimizer, the Risk to Net Value indicator measures the Potential Risk taking into account the Net Value provided by all projects displayed in the Portfolio Optimizer.&nbsp;


For achieving the most efficiency within the portfolio, you want to see that the Risk indicator is low and the Net Value indicator is high.&nbsp;


The Risk and Net Value indicators are represented from the perspective of how they relate to each other. 


*`Adobe Workfront`* calculates the Risk and Net Value indicators using the following formulas: 



* The Risk indicator is calculated by the following formula:  


  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```


* The Net Value indicator is calculated by the following formulas:   


  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  
  Or  


  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```






>[!NOTE]
>
>The Risk to Net Value indicator calculates based on the projects that you display in the Portfolio Optimizer, and not on all the projects which are associated with the portfolio.&nbsp;


