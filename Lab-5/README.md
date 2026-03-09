#  ARTI308 – Lab 5: Car Price Prediction

##  Overview
This lab demonstrates how to build a **machine learning pipeline** to predict car prices using structured data.  
The workflow includes **data preprocessing, feature engineering, model training, evaluation, and feature importance analysis** using Python and Scikit-learn.

The main goal is to predict the **price of a car** based on its characteristics such as mileage, engine size, fuel type, and model.

---

#  Dataset

The dataset contains information about used cars with the following features:

| Feature | Description |
|-------|-------------|
| model | Car model |
| year | Manufacturing year |
| price | Car price (target variable) |
| transmission | Transmission type |
| mileage | Distance driven |
| fuelType | Fuel type |
| tax | Road tax |
| mpg | Fuel efficiency (miles per gallon) |
| engineSize | Engine capacity |

###  Target Variable
```python
price