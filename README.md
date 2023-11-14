walmart-Sales-Analysis-using-PySpark

•	Dataset- Walmart-recruiting-store-sales-prediction

https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting/data

Preprocessing and Data Analysis:

•	Most of the Store types in the data set are TYPE A.

<img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/b58196f8-fc23-42e3-b27c-db2183cbcf91">

 

•	As the Size of the store increases the sales also increases.

 <img width="397" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/1bb804f2-0602-4dfb-aad5-30aec65886c7">



•	Type A Store has done most of the sales.

<img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/cbb76a2c-6a24-47a3-8032-82bb2e9001c8">

 


•	only slight variation in sales with respect year
•	In 2011 sales are relatively lower than both 2010 and 2012
•	In first month sales are least and in 12th month sales are higher .May be due to festivals

 <img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/34ec370d-d1c7-42aa-8371-a53a84cb4ece">





•	During the holiday there is a slight increase of sales.

<img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/92c7ed18-2860-4371-9f4e-cd274e4aec38">
 

•	Sales does not depend on the fuel.

<img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/fb53e269-6926-470f-b82b-5e6e67ac5c2e">

 
•	Sales don’t depend on the temp but during too cold and too hold there is a slight change.

<img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/b9bc8b34-3ab3-49b1-9091-7f26bc25e374">

 

•	Only slight changes in the sales when unemployment increases.

<img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/b6f51e4c-c370-4609-8e5d-c3f6e25e9f35">

 
•	CPI(Consumer Price Index) does not effect sales.

<img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/cd0712a0-1f51-4a77-871d-b7df7faa0485">


•	Dept does affect sales
•	Different department have different sales

 <img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/931dff35-cc87-479f-9376-6c8450cd4e4f">




•	Based on the features we have removed some of the features that are not important and kept
'Store', 'IsHoliday', 'Type', 'Size', 'week', 'Dept', 'year'.



Models Analysis:
•	Random Forest Regressor:
The WMAE loss for the training set is 10986.69728484865.
The WMAE loss for the validation set is 10842.144435508004.



•	Linear Regression:
	RMSE on training data: 14569.467490828793
	RMSE on validation data: 14583.551300042831

•	Decision Tree Regression:
The WMAE loss for the training set is 9468.314207525373.
The WMAE loss for the validation set is 9183.5112872512.

Feature Importance:

•	Random Forest Regressor:

 <img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/5773f996-d415-4161-9629-ac5de0daaab2">

•	Decision Tree Regressor:

 <img width="468" alt="image" src="https://github.com/surajlokesh/walmart-Sales-Analysis-using-PySpark/assets/43951851/85977af2-ded0-4df8-8080-e03e713c8868">

Summary:
1. Sales heavily depend on Type and Department.
2. Size of store also play major role in sales big store usually have more weekly_sales.
3. A type store did more sales than b and c.
4. weekly sales also depend on week of the year holidays weeks are good for sales.

