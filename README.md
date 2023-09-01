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

### **Random Forest Model Interpretations**
- According to my random forest model, the item maximum retail price (Item_MRP) is the most important feature. This seems fairly intuitive as price will often dictate sales. 
- Grocery stores, item visibility, and type 3 supermarkets were all top coefficients in the linear regression model. 
- About half the time, a decision was made based on Item_MRP. - - The model made decisions based on the Grocery Stores about 20% of the time.
- This random forest model did a decent job of making decisions based on both effective and ineffective features.

![image](https://github.com/Kridge42/Product-Sales/assets/126993169/5d69afe1-0066-4b15-a142-42f3c8b2c05d)

- SHAP value summary plots really drive at the same features in the model. The SHAP bar plot and dot plot clearly reinforce the top five most important features. Four of the five top SHAP values are in the most important features and that relationship is clearly defined in the dot plot. Red means a higher importance impact on model output and blue means less importance impact on model output. Purple is between the two and it is interesting to note the dot plot displays both positive and negative values as well affected and how much that feature was valued at the same time.   

![image](https://github.com/Kridge42/Product-Sales/assets/126993169/20876498-58b3-45a9-9bfb-044ddb2122de)

-5,788
-3,788
-1,788
211.9
2,212
4,212
6,212
8,212
1.021e+4
Item_Type_Dairy = 1
Outlet_Size_High = 1
Outlet_Type_Grocery Store = 0
Item_Visibility = 0.0195
Item_MRP = 261.3
base value
8,304.04
8,304.04
higher
→
f(x)
←
lower
Outlet_Type_Supermarket Type1 = 1
Outlet_Type_Supermarket Type1 = 1
![image](https://github.com/Kridge42/Product-Sales/assets/126993169/4bb3e573-3281-4568-b2e9-54636e81000e)


##### **For any additional questions, please contact me by email**
