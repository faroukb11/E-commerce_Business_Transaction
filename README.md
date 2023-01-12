# E-commerce_Business_Transaction
EDA project
# E-commerce_Business_Transaction(Overview)
In this project, I conducted an exploratory data analysis on a UK e-commerce sales data from Kaggle .
After analyzing the data set , I will answer the following 10 questions :
* How was the sales trend over the months?
* What are the most frequently purchased products?
* How many products does the customer purchase in each transaction?
* What are the most profitable segment customers?
* Based on your findings, what strategy could you recommend to the business to gain more profit?

## Code and Resources Used 
**Python Version:** 3.7  
**Packages:** pandas, numpy, matplotlib, seaborn  
**Kaggle Dataset :** https://www.kaggle.com/datasets/gabrielramos87/an-online-shop-business  



## Data Strucure
This is a sales transaction data set of UK-based e-commerce (online retail) for one year. This London-based shop has been selling gifts and homewares for adults and children through the website since 2007. Their customers come from all over the world and usually make direct purchases for themselves. There are also small businesses that buy in bulk and sell to other customers through retail outlet channels.

The data set contains 500K rows and 8 columns. The following is the description of each column :

| Feature| Description |
| --- | --- |
| TransactionNo (categorical) |  A six-digit unique number that defines each transaction. The letter “C” in the code indicates a cancellation. |
| Date (numeric) | The date when each transaction was generated. |
| ProductNo (categorical) | A five or six-digit unique character used to identify a specific product. |
| Product (categorical) |  Product/item name. |
| Price (numeric)| The price of each product per unit in pound sterling (£).|
| Quantity (numeric) | The quantity of each product per transaction. Negative values related to cancelled transactions.|
| CustomerNo (categorical) | A five-digit unique number that defines each customer.|
| Country (categorical) |  Name of the country where the customer resides.|

## Data Cleaning
After studying the data, I needed to clean it up for analysis. I made the following changes and created the following features:

*	Removed rows with null values 
*	Set the Date column to datetime format 
*	Created 3 seperate columns Year, month and MonthName from Date
*	Created Totalrevenue attribute which is the revenue generated per transaction (quantity x price)
*	Created Region attribute 
*	Created two seperate data frames for confirmed and cancelled orders 


## EDA
I looked at the distributions of the data and the value counts for the various features. Below are a few highlights from the pivot tables and charts. 

![alt text](https://github.com/faroukb11/E-commerce_Business_Transaction/blob/main/egionp.jpeg "Revenue repartition per region")

![alt text](https://github.com/faroukb11/E-commerce_Business_Transaction/blob/main/tp10sellip.png "Best selling products")
![alt text](https://github.com/faroukb11/E-commerce_Business_Transaction/blob/main/tp10country.png "Top 10 highest revenue generating countries ")
![alt text](https://github.com/faroukb11/E-commerce_Business_Transaction/blob/main/-10sellip.png "Most cancelled products")
![alt text](https://github.com/faroukb11/E-commerce_Business_Transaction/blob/main/sales_evolution.jpeg "Sales evolution")



## Answering Questions
**1- How was the sales trend over the months?**

  Looking at the Sales evolution graph , the sales were the hightest in autumn(September,October,November) but they tend to struggle significally  between winter and spring.


**2- What are the most frequently purchased products?**
  
  The 10 most frequently purchased products are shown in the table below :
  
| Product name| Total number of orders |
| --- | --- |
| Cream Hanging Heart T-Light Holder |  2336 |
| Jumbo Bag Red Retrospot | 2115 |
| Regency Cakestand 3 Tier | 2019 |
| Party Bunting |  1708 |
| Lunch Bag Red Retrospot| 1597 |
| Assorted Colour Bird Ornament	 | 1491 |
| Popcorn Holder	 | 1426 |
| Set Of 3 Cake Tins Pantry Design |  1399 |
| Pack Of 72 Retrospot Cake Cases		 | 1373 |
| Lunch Bag Black Skull | 1329 |

**3- How many products does the customer purchase in each transaction?**

The average quantity of products purchased in each transaction is 283.

**4- What are the most profitable segment customers?**

The most profitable segment customers are the european clients (98% of sales) especially the UK based smalll businesses as they buy in bulk the best selling products.


**4- Based on your findings, what strategy could you recommend to the business to gain more profit?**

After analyzing the data , i noticed that the mojority of  sales were made in the Uk but they are increasing in other  european countries such as the Netherlands ,Germany and France . i would suggest focusing on marketing and advertising  in those countries in order to boost sales. Aside from Europe , Japan is the tenth most revenue generating country and i would recommend introducing new products that are more suitable to the customers culture .
