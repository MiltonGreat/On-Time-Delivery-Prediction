# On-Time-Delivery-Prediction

### Overview

This project implements a machine learning model to predict whether a delivery will arrive on time based on various customer, product, and shipment-related features. The model uses a Random Forest Classifier trained on real-world delivery data to provide accurate predictions.

The primary goal of this project is to empower logistics and supply chain teams to optimize operations and improve customer satisfaction by identifying potential delays in advance.

### Dataset

This data includes the following features:

- Customer_care_calls: Number of calls made by the customer to customer care.
- Customer_rating: Customer's satisfaction rating (1–5).
- Cost_of_the_Product: Cost of the purchased product.
- Prior_purchases: Number of purchases made by the customer before this order.
- Gender: Customer's gender (encoded as 0 = Female, 1 = Male).
- Discount_offered: Discount applied to the product.
- Weight_in_gms: Weight of the product in grams.
- Mode_of_Shipment: Shipment method (e.g., Ship, Flight).
- Warehouse_block: Block in the warehouse where the product was stored.
- Product_importance: Importance level of the product (e.g., Low, Medium, High).

##### Target Variable
- Reached.on.Time_Y.N: Binary variable indicating if the delivery was on time (1 = Yes, 0 = No).

### Workflow

##### Data Preprocessing:
- Handled missing values and scaled numerical features.
- One-hot encoded categorical variables like Mode_of_Shipment, Warehouse_block, and Product_importance.

##### Exploratory Data Analysis (EDA):
- Visualized feature distributions and correlations with the target variable (Reached.on.Time_Y.N).

##### Feature Engineering:
- Created meaningful features from categorical and numerical variables to enhance model performance.

##### Machine Learning Model:
- Trained a Random Forest Classifier to predict the likelihood of a delivery arriving on time.

##### Real-Time Predictions:
- Provides real-time predictions for new orders using the trained model.

### Results

- Accuracy: 67%
- Precision (Class 1): 79%
- Recall (Class 1): 61%
- F1-Score (Class 1): 69%
- ROC-AUC: 0.75

### Source

https://www.kaggle.com/datasets/willianoliveiragibin/on-time-delivery/data
