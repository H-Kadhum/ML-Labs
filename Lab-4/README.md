
- **Dataset.csv** → Raw dataset used in the lab  
- **4- Data Quality Assessment & Preprocessing.ipynb** → Jupyter Notebook containing all preprocessing steps  
- **README.md** → Lab documentation  

---

## Dataset Description

The dataset includes the following features:

- `model` – Car model  
- `year` – Manufacturing year  
- `price` – Car price  
- `transmission` – Transmission type  
- `mileage` – Distance driven  
- `fuelType` – Type of fuel  
- `tax` – Road tax  
- `mpg` – Miles per gallon  
- `engineSize` – Engine size (liters)  

---

## Data Quality Assessment Steps

The following checks were performed:

- Dataset inspection using `head()`, `info()`, and `shape`
- Data type verification
- Missing values detection
- Duplicate records detection
- Statistical summary using `describe()`

---

## ⚙️ Data Preprocessing

### 1- Handling Missing & Duplicate Values
- Checked for null values  
- Removed duplicate rows if present  

### 2- Encoding Categorical Variables
Categorical features such as:
- `model`
- `transmission`
- `fuelType`

were encoded to prepare the dataset for machine learning algorithms.

### 3- Feature Scaling (Min-Max Normalization)

Numerical features were scaled using **Min-Max Normalization** to transform values into a range between 0 and 1.

Formula used:

X_scaled = (X - X_min) / (X_max - X_min)

Applied to numerical columns including:
- `price`
- `mileage`
- `tax`
- `mpg`
- `engineSize`
- `year`

This ensures that features with different ranges do not negatively impact distance-based models.

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## How to Run

1. Open Jupyter Notebook.
2. Ensure `Dataset.csv` is in the same folder as the notebook.
3. Run all cells sequentially.
4. Review the cleaned and scaled dataset output.

---

## Outcome

By the end of this lab:

- The dataset is cleaned and structured.
- Categorical variables are encoded.
- Numerical features are normalized.
- The dataset is ready for machine learning modeling.

---

## Author

Hussian Kadhum  
Lab 4 – Data Quality Assessment & Preprocessing  