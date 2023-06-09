# Superstore Data Visualization using Tableau
#### By: Dea Gloria A. N.
------

This project was made as a coursework requirement for Business Analytics, Applied Modelling, and Prediction (ST2187). The dataset contains 24 columns and 51,290 observations (transactions) which allows us to explore the store’s performance to make future decisions.

We are given a task to retrieve insight of the dataset from a store between Q1 2017 to Q4 2020. The report will include the company’s performance in general, followed by breakdown based on area, breakdown based on sub-category and products, and lastly forecasting for profit. All the analyses aim to help the business stakeholders to make correct decision for the company’s sustainability by maximizing profit and minimizing loss.

First, we will look at the data in general and analyse several key indicators such as total sales, total profit, trend of sales, average delivery time, average transaction value, average shipping cost, and profit margin. From this section, we will be able to get some numbers which can be used for key performance indicator (KPI).

Second, we analyze the company’s performance based on area. The metrics that we will be using is profit margin, profit, and count of transactions. We will be able to see on per market basis and even increase the granularity to observe per country’s performance. Hence, we can make some adjustments based on four basic international business strategies depending on the pressure for cost reduction and/or local responsiveness.

Third, we will observe product by each sub-category based on the average discount, average sales, and quantity of purchased items. This allows us to see which sub-category have the greatest or least discount, highest or lowest sales, and sold quantity so far. Furthermore, we can refer these values as a benchmark for future promotion.

Fourth, we can see which products are performing well and not in terms of profit margin. Moreover, we will see a scatter plot showing profit vs. sales for every product and cluster them by the profit margin. This aims to show us which product are performing well and which are not, so we can choose to cease or continue selling these items.

Lastly, we will forecast the profit for the upcoming year (2021). We will break it down per market and per sub-category as well. This can be used as an expectation or target of profit to be realized in the future. Furthermore, this forecast will also project which market or category we should focus on to maximize profit.

Finally, a list of recommendations would be given at the end of the report.

------

## 1. Overall Summary

![Overall Summary](https://github.com/deagloriaa/superstore-data-visualization/blob/main/pictures/1.png)

First, we shall look at the company’s overall performance from 2017 to 2020. The purpose is to have a general idea on how the store is performing so far. There are 51,290 transactions with an average transaction value (ATV) of $246.49. The ATV is generated by sum of sales divided by total transactions. Meanwhile, the average ship time is 4 days with an average cost of $26.38 per order. The overall profit margin is 11.61%, indicating a good company performance as 10% profit margin is the rule of thumb for average.

From these transactions, we established a total sales of $12,642,502 and a total profit of $1,467,457. We can observe that technology is the most dominating category for both measures. In terms of customer segment, the highest sales come from regular consumer, followed by corporate, and lastly home office. Ultimately, there is an increasing trend of sales on quarter 4 every year, followed by a decreasing trend on quarter 1 the next year. This might happen due to holiday season in Q4 (i.e. Christmas) which generally increase the tendency for customer to shop.

## 2. Regional Analysis

![Regional Analysis](https://github.com/deagloriaa/superstore-data-visualization/blob/main/pictures/2.png)

In this section, we would like to analyse the performance for each market and/or country. Hence, we introduce a new measure called Profit Margin which is calculated by sum of profit divided by sum of sales.

The map depicts each country’s performance based on its profit margin. This allows business stakeholders to decide which countries should be more focused on or to improve on. For example, Armenia has the highest profit margin ratio at 44% whereas Turkmenistan generates the lowest profit margin at -163%. This implies that the company generates 44% profit in Armenia for the sales meanwhile it generates 163% loss in Turkmenistan. Hence it would make sense to improve the company’s strategy for Turkmenistan, or else we can choose to be more focused on other countries such as Armenia.

Observing the transaction count by market, US dominates the most transaction that generates profit at 8,058 transactions. Meanwhile, among 11,002 transactions in the APAC market, 7,672 generates profit whereas 3,330 generates loss (highest loss transaction count among all market). However, even though APAC’s sum of profit is around $150,000 higher than the US, their profit ratio is roughly the same at around 12%.

Comparing to other market, we can observe a good performance in Canada. Even though there are only 384 transactions (377 profit, 7 loss) and the sum of profit is relatively small compared to other markets (around $18,000), Canada yields the highest profit ratio at 27%. Meanwhile, EMEA doesn’t show a significant profit and profit margin such as other markets.

## 3. Product Analysis by Sub-Category

![Product Analysis by Sub-Category](https://github.com/deagloriaa/superstore-data-visualization/blob/main/pictures/3.png)

Moving on to the products, we will observe the discount, sales, and quantity of each sub-category. The treemap portrays that tables induces the greatest average discount at 29% meanwhile paper has the least discount at 11%. Tables also raise the highest average sales at $879.26, followed by copiers and bookcases. Lastly, binders are the most ordered sub-category of all time while tables are least ordered. This condition happens in general because as a price (sales) increases, the quantity demanded decreases assuming the items are considered as normal goods.

## 4. Product Analysis Breakdown by Products

![Product Analysis Breakdown by Products](https://github.com/deagloriaa/superstore-data-visualization/blob/main/pictures/4.png)

This section is still related with the sub-category product analysis. On the left side, we are able to observe that tables generate a negative value of profit margin. Relating to the packed bubble chart on the previous dashboard, this implies that even though the average sales of tables are the highest in amount, does not mean that the performance is good. It turns out that for each cents of tables sold, they generate 8.5% loss in average. Meanwhile, papers have the highest profit margin at 24.2%. This implies that for each cents of papers sold, they produce 24.2% profit in average, indicating a good performance even though the sales is small in amount.

On the right side, we plot sales on the x-axis and profit on the y-axis for every product. Additionally, we use the slope (  y/x  ), which is the profit margin for clustering. Based on tableau’s automatic clustering feature, it generates 5 clusters which we infer as:

- Cluster 1: Good profit margin
- Cluster 2: Even profit margin
- Cluster 3: Very good profit margin
- Cluster 4: Bad profit margin
- Cluster 5: Very bad profit margin

The purpose of this scatter plot is to infer which specific products are performing well and which are not. We are also able to do filtering based on the sub-category or clusters. Hence, the business stakeholders will be able to make decision on which product should they be more focused on and which should be removed. For instance, the annotated product above belongs to cluster 5, the cluster of products that we prefer not to focus on anymore as it generates a negative value of profit margin. On the opposite, products in cluster 1 and 3 should be more promoted to increase the company’s performance.

## 5. Profit Forecasting

![Profit Forecasting](https://github.com/deagloriaa/superstore-data-visualization/blob/main/pictures/5.png)

The last part aims to project our company’s profit until 2021 Q4 based on data from 2017 until 2020. The forecasted profit takes into consideration the seasonality of every quarter. Based on the overall profit chart, we expect a profit drop in Q1 2021 (following the trend of Q1 on previous years). Afterwards, the profit is predicted to rise gradually from Q2 to Q4 2021.

Observing the trend by market, profit is likely to escalate in Africa, EU, LATAM, and US. Meanwhile, Canada, EMEA, and APAC might generate profit or loss. This is because of the 95% confidence interval that we observe through the black line. The lower bound implies the lowest possible value of the forecasted profit whereas the higher bound implies the highest.

In terms of category, profit is forecasted to augment constantly for furniture throughout 2021. For office supplies, there seems to be a significant increase from Q1 to Q3 2021 followed by a slight decrease at the end of the year. Lastly, profit for the technology category is expected to ascend tremendously along the year with a minor drop between Q2 and Q3.

------

## Recommendation
Based on the analyses, some recommendations that could be made are:
1.	Enhance selling products that are low demanded on Q4 as it is the highest selling season of the year. Meanwhile, products that are highly demanded can be strongly promoted on Q1 to uplift the sales.
2.	Offer a bundle deal of high and low demanded product to increase the sales of the low demanded product.
3.	Create a loyalty program based on ATV (e.g. minimum spend $50 discount 10%).
4.	Drop countries with extremely negative profit margin and focus more on countries with positive profit margin. If the country has a slight negative/positive profit margin, we can try to make amendment in our business strategy.
5.	Even though transactions in Canada is not as many as other markets, they generate an impressive profit margin. Hence, we should explore more from this potential market.
6.	Tables are the sub-category that has the greatest discount and sales yet give a negative profit margin. Therefore, we should sell the remaining stock of tables with the current sales price and halt the production/import afterwards. At the same time, we can gain profit from other sub-categories such as copiers to subsidise the loss from tables sold.
7.	Similar to tables, specific products which belong to cluster 4 and 5 in the scatter plot should be cleared out of stock and stop selling them thereafter. Concurrently, focus on selling the products in cluster 1 and 3 while trying to elevate the profit for products in cluster 2.
8.	Set a target for profit to be acquired in 2021 based on the forecasting as benchmark.

------

## Conclusion
Through the first dashboard, we obtain general idea about company’s performance from 2017 to 2020 such as $246.46 ATV and 11.61% profit margin. Total sales during this period is $12,642,502 and with $1,467,457 profit. We observe that technology is the most dominating category while consumer is the largest segment. We also see that the trend of sales is high at Q4 annually.

The second dashboard allows us to explore company’s performance by area. We are able to decide which market or country should we focus on (e.g. Armenia) and which to drop (e.g. Turkmenistan).

Analyzing further in terms of products, dashboard 3 & 4 allows us to identify which products are well-performing and not. Therefore we can decide which products to sell in the future and which to cease.

Lastly, the last dashboard enables us to forecast company’s profit for the upcoming year. This can be used as the benchmark for profit targeting. Overall, the forecast shows a positive trend for profit.

To conclude, this report has shown that the company operation is in a healthy state and it definitely has the potential to excel in the very near future.
