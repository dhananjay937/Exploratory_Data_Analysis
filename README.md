# 🚗 Used Car Price Analysis - Exploratory Data Analysis (EDA)

## 📌 Overview
This project performs **Exploratory Data Analysis (EDA)** on a **used car dataset** to gain insights into **factors affecting car prices**, such as **brand, fuel type, transmission, car age, mileage, and more**. The goal is to clean and preprocess the data, engineer useful features, detect outliers, and visualize trends to understand price variations in the used car market.

This analysis can help **buyers, sellers, and financial institutions** make data-driven decisions regarding car valuation, loan approvals, and resale strategies.

---

## 📺 Dataset Information
- **Source**: The dataset used in this project contains **7,253 records** and **14 attributes** related to used cars.
- **Key Features**:
  - `S.No` - Serial number (Removed in preprocessing)
  - `Name` - Car brand and model
  - `Location` - City where the car is listed
  - `Year` - Year of manufacturing
  - `Kilometers Driven` - Distance traveled by the car
  - `Fuel Type` - Type of fuel (Petrol, Diesel, CNG, etc.)
  - `Transmission` - Manual or Automatic
  - `Owner Type` - First, Second, Third-owner cars
  - `Mileage` - Fuel efficiency (km/l or km/kg)
  - `Engine` - Engine capacity (CC)
  - `Power` - Power output (bhp)
  - `Seats` - Number of seats
  - `New Price` - Original price (mostly missing values)
  - `Price` - Selling price of the car (Target variable)

---

## 🛠️ Tech Stack & Libraries Used
This project is implemented in **Python** using the following libraries:
- `pandas` - Data manipulation and cleaning
- `numpy` - Numerical computations
- `matplotlib` & `seaborn` - Data visualization
- `warnings` - To suppress warnings

---

## 🔍 Key Steps in Analysis

### **1️⃣ Data Preprocessing & Cleaning**
✔ Removed duplicate records and unnecessary columns (`S.No`).  
✔ Checked for **missing values** and handled them by:
   - Filling with mode/median values where appropriate.
   - Dropping columns with excessive missing values (e.g., `New Price`).  
✔ Converted textual numerical values (`Mileage`, `Engine`, `Power`) into numerical format.

---

### **2️⃣ Feature Engineering**
🚀 **Created new useful features**, such as:
- **Car Age** = `Current Year - Year of Manufacture`
- **Brand & Model Extraction** from the `Name` column
- **Price per Kilometer** = `Price / Kilometers Driven`

---

### **3️⃣ Exploratory Data Analysis (EDA)**
📊 **Statistical Summary**:
- **Descriptive statistics** (mean, median, min, max, standard deviation) for numerical features.
- **Distribution analysis** to understand variations in car price, mileage, and engine capacity.

📈 **Univariate & Bivariate Analysis**:
- **Histograms & Boxplots**: To detect outliers and skewness in data.
- **Bar Charts & Countplots**: To analyze categorical features like **fuel type, transmission, owner type, and location**.
- **Correlation Heatmap**: To find relationships between numerical features.
- **Price Trends**: How different brands and fuel types impact car prices.

---

### **4️⃣ Data Transformation**
🔄 **Applied Log Transformations**:
- Used to **normalize skewed features** like `Kilometers Driven` and `Price` for better analysis.

---

### **5️⃣ Outlier Detection**
🔍 Identified **anomalous car prices** and **extreme mileage values** using:
- **Boxplots**
- **Histograms**
- **Scatter plots**

---

### **6️⃣ Saving Cleaned Data & Reports**
✅ **Final Cleaned Dataset** saved as:  
   📂 `cleaned_used_cars_data_with_EDA.csv`  
✅ **Visualizations** saved for report generation.

---

## 📊 Sample Visualizations
Here are some of the key insights from our analysis:

1. **Price Distribution Across Different Fuel Types**  
   ![Price vs Fuel Type](price_by_fuel_type.png)

2. **Correlation Heatmap**  
   ![Correlation Matrix](correlation_matrix.png)

3. **Boxplot for Car Prices (Outlier Detection)**  
   ![Boxplot for Price](boxplot_price.png)

> **More detailed visualizations are included in the repository.**

---

## 🚀 How to Run This Project
Follow these steps to run the analysis on your local machine:

### **1️⃣ Clone the Repository**
```bash
gh repo clone dhananjay937/Exploratory_Data_Analysis
```
### **2️⃣ Navigate to the Project Directory**
```bash
cd used-car-eda
```
### **3️⃣ Install Required Libraries**
```bash
pip install -r requirements.txt
```
### **4️⃣ Run the Jupyter Notebook**
```bash
jupyter notebook Exploratory_Data_Analysis.ipynb
```
OR  
Run the script directly:
```bash
python eda_script.py
```

---

## 📌 Use Cases & Applications
This analysis is **useful for**:
- **Car Dealerships**: Pricing strategies based on car condition and features.
- **Financial Institutions**: Loan approvals and risk assessment.
- **Insurance Companies**: Estimating car insurance premiums.
- **Data Science & ML Enthusiasts**: Feature selection for predictive modeling.

---

## 🌟 Contributing
🚀 **Contributions are welcome!** If you'd like to improve this analysis:
1. **Fork** this repository
2. Create a **new branch** (`feature-branch`)
3. **Commit** your changes
4. **Submit a Pull Request (PR)**

---

## 🔗 Connect & Follow
📧 Email: [patildhananjay1307@gmail.com]  
🔗 LinkedIn: [www.linkedin.com/in/dhananjay-patil-b25423315]  
---

🔔 **If you find this project useful, don't forget to ⭐ star this repository!**  
Happy Coding! 🚀😊  

