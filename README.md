# **Product Sales**
### **Sales predictions for various stores**
#### Author: Kevin Ridge

Exploring various store performance in terms of sales and how their product types perform based on basic variables.

### **Data Dictionary**
![image](https://user-images.githubusercontent.com/126993169/230653647-9deec3e4-4899-4ad0-92b8-d38054aa5be6.png)

Link to the original data source: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/

## **Data preparation:**
- Filled missing values to retain information
- Cleaned up data by removing inconsistent labels
- Verified no duplicated values for accuracy
- Inspected columns to find correlations to sales

## **Results:**
### **Correlation to Item Outlet Sales**
![Correlation map](https://user-images.githubusercontent.com/126993169/230656021-4276269c-8da3-47a4-8d65-43febada6d29.png)
##### **Item MRP is the only feature that relates well to Item Outlet Sales. More data would provide better predictive results.**

### **Item Type Sales**
![Item types](https://user-images.githubusercontent.com/126993169/230657020-2beecd76-bb4f-4ee7-be4b-54bb8feac4c0.png)
##### **Each category sold well. No particular item type accounts for a majority of outlet sales.** 

### **Outlet Performance**
![Outlet type](https://user-images.githubusercontent.com/126993169/230658087-0ddcd73a-5e50-4920-b9d8-4f0c5d439087.png)
##### **Small grocery stores have much lower sales than the supermarket types. Supermarket type 3 is the top performer in generating sales.**

## **Model:**
- I used a random forest model to predict item outlet sales.
- The accuracy of the returned metrics is 60%.
- Based on that number with the available data, this would not predict outlet sales very well.
### **Recommendations:**
- More data is needed.
- More featured variables relative to item outlet sales would provide better sales predictions.
- More information about the outlets such as location and quarterly reports would provide great insight.
### **Limitations & Next Steps:**
- Limited data, irrelevant features, and lack of information produced a model that underperforms.
- The machine learning model used here is rather simple compared to others.
- Even with this data, s more complex machine-learning model could produce more accurate results.

- ## **LinearRegression coefficients plot**
![image](https://github.com/Kridge42/Product-Sales/assets/126993169/70d0e7e6-93d6-4a47-84fe-c0fb2aa6b342)

### **Model observations based on 3 largest coefficients**
- According to this model, the type 3 supermarket is observed to increase Item Outlet Sales by 1525.01 rupees. 
 - Build more supermarket type 3's, and sales could rise significantly.
- This model observes a negative relationship between Outlet Sales and Item visibility.
 - In other words, the visibility of an item is not likely to affect whether or not a customer buys items.
 - The Item Visibility is a potential opportunity for improvement of sales. If we took a much closer look at individual item sales and their visibility, we might be able to increase the sales of particular items.
- In this model, the Grocery stores are decreasing sales by 1608.00 rupees.
 - Grocery stores have many produce items that will expire before purchase. This is pure speculation based on this model, but room for improvement could happen in inventory management at the grocery stores.


- ## **Tree-based model's feature importances**
![image](https://github.com/Kridge42/Product-Sales/assets/126993169/cfbcf01c-315b-4e66-a853-48b50545b65a)


##### **For further information**
For any additional questions, please contact by email
