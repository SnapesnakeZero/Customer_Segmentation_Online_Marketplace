# Customer_Segmentation_Online_Marketplace
**Important Note: Because the excel file size is too huge, to access the original dataset please download it through link source below**
## Background & Objective
**Background**: 
<br>
According to data collected from Interactive Media in Retail Group (IMRG), there were 5000% increase of consumer buy product from online platform in year 2010 compared to year 2000. This huge increase in just 10 years indicate that there are fundamental changes in the way consumer shop product.
<br><br>
To be able to keep up with the changes of consumer buying behavior, company must adapted so they don't lose it's consumer and also expand it's market range. Many big company have enough fund and resource to adapted to this change, but many small retailers doesn't have enough resourse to transform itself. 
<br><br>
The data that we will be using this time originated from a small retailer located in UK consisting of 80 members. The retailer is registered as non-store business. The retailer that was found in 1981 mainly selling unique all-occation gifts. For years in the past, this retail heavily relied on direct mailing catalogue and order were taken over phone calls. But in the past two years, they tried to transform it's business adapting to the internet boom by creating website for selling the product and using Amazon to sell and market it's product. It's seems thou that the retailer still doesn't have enough understanding upon it's consumer.  
<br><br>
This project was taken in order for small online retailers and new entrants to the retail sector to be able have better understanding about it's consumer and create marketing plan based on consumer focused.  
<br>**Objective**:
<br>
* Getting business insight about the retailer performance originated from UK in the span of the data collected.
* Getting business insight about consumer originated from UK in the span of the data collected
* Create a clustering model to identify segmentation of it's consumer and using those information to decide where, when, how, and to whom a product, service, or brand will be marketed.
* To increase marketing efficiency by directing effort specifically toward the designated segment in a manner consistent with that segment’s characteristics.
## Problem Statement
**Goal**:
* Getting business insight about the retailer performance in the span of the data collected.
* Getting business insight about consumer in the span of the data collected
* Create a clustering model to identify segmentation of it's consumer and using those information to decide where, when, how, and to whom a product, service, or brand will be marketed.
* To increase marketing efficiency by directing effort specifically toward the designated segment in a manner consistent with that segment’s characteristics.
<br>

**Research Question**:
<br>
* Who are our best customers in UK?
* Who has the potential to be converted in more profitable customers in UK?
* Which customer we must retain in UK?
* Which group of customers is most likely to respond to our current campaign in UK?
<br>

**Business Benefit**:
<br>
* Retailer know how to treat consumer that originated from UK with spesific criteria
* Retailer able to create product differentiation based on the characteristic of each consumer that originated from UK
<br>

**Expected Outcome**:
<br>
* Had business insight about the retailer performance in the span of the data collected.
* Had business insight about consumer originated from UK in the span of the data collected
* Consumer segmentation analysis
* Recommendation based on customer segmentation
<br>

**(Note: We will do RFM Analysis and combine it with predictive algorithm to achive in depth insight)**

## Data Source
The data was taken from Online Retail II data set source from UCI Machine Learning Library: 
<br>
https://archive.ics.uci.edu/ml/datasets/Online+Retail+II
<br>
<br>
Dataset contain all the transaction occuring for a UK-based and registered non-store online retail between 01/12/2009 and 09/12/2011. The company mainly sells unique all-occasion gift-ware. Many customers of the company are wholesalers
<br>
<br>
It was mention in UCI Machine Learning Library that the data was taken for the purpose of research and was publish in Journal of Database Marketing & Customer Strategy Management. Below attached citation pertaining the research:
<br>
<b>Chen, D. Sain, S.L., and Guo, K. (2012), Data mining for the online retail industry: A case study of RFM model-based customer segmentation using data mining, Journal of Database Marketing and Customer Strategy Management, Vol. 19, No. 3, pp. 197-208.</b>

## Data Dictionary
The dataset contain one csv file called `online_retail_II.xlsx`. The data set contain 8 feature/column The description upon each feature in `online_retail_II` will be mention below:
* `InvoiceNo`= Invoice number. Nominal. A 6-Digit integral number uniquely assigned to each transaction. <b>(if this code starts with the letter 'c', it indicates a cancellation)</b>
* `StockCode` = Product (item) code. Nominal. A 5-digit integral number uniquely assigned to each distinct product
* `Quantity`: The quantitites of each product (item) per transaction. (Numeric)
* `Description`: Product (item) name. Nominal
* `InvoiceDate`: Invoice date and time. Numeric. The day and time when a transaction was generated
* `UnitPrice`: Unit Price. Numeric. Product price per unit in sterling
* `CustomerID`: Customer number. Nominal. A 5-digit integral number uniquely assigned to each customer
* `Country`: Country name. Nominal. The name of the country where a customer resides.

## Conclusion
There were 4 cluster created after applied RFM Method and K Means Method. Below this attach the interpretation on each cluster:
* Cluster 0 = This Cluster contains 22% of total customers. It belongs to the "Loyal Customer" segment because customers haven't done transactions recently but they purchase products frequently and spend a lot in the retailer.

* Cluster 1 = This Cluster contain 18% of total customer. It belongs to the "Lost Cheap Customer" because customers haven't done transactions recently, rarely purchase products, and only spent a little amount in the retailer.

* Cluster 2 = This Cluster contain 30% of total customer. It belongs to the "Best Customer" because customers have done transactions recently, purchase products frequently, and spend a lot of money in the retailer.

* Cluster 3 = This Cluster contains 20% of the total customer. It belongs to the "Promising/New Entrant" because customers have done transactions recently but rarely purchase products and spend little amount in the retailer.

## Recommendation
By looking through the cluster interpretation and RFM model interpretation above, we created recommendation for each customer segment based on Recency, Frequency, and Monetary that listed below:

* For the `Loyal Customer` segment: Retailer must as much as possible retain customers in this segment because the customers in this cluster tend to spend a lot of money and purchase frequently. What the retailer suggested is to do is allocate some budget for giving promotion to the customer in this segment. They can send messages through Whatsapp or email to inform customers that they just got a discount on a product. The goal here is to engage the customer and attract customer attention at the same time so that the customer attracted to buy product again and at the same time retain the customer loyalty
* For the `Best Customer` segment: This segment contains customers that any company dreams of, they purchase recently, frequent buyers, and spend a lot of money in the company. What the retailer suggested to do is to reward the customer in this segment. You can do it by giving them early access to the product, giving them discount vouchers, and many more. The goal is to retain customer loyalty and also motivate customer to keep purchasing and spend more money 
* For `Lost Cheap Customer`: This segment contains customers that are disliked by all companies, because customers in this segment haven't done transactions recently, rarely purchase products, and only spent little amount in the retailer. What the retailer suggested to do is to start a marketing campaign to reach out to customers and revive their interest into the company product. 
* For `Promising/New Entrant` segment: This segment contains customers that recently/first time bought products in the company. This was symbolized by the high recency and low score in frequency and monetary. What the retailer suggested to do is to create brand awareness to this kind of customer and also offer a free trial to the product. The goal here is to instill the retailer brand to the customer, make a good impression to customers, and persuade them to buy more.
