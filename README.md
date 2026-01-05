# 🏙️ Urbanization and Housing Affordability — Data Science Project  

---

## 🪜 **Step 1: Data Importing**
The dataset titled **[Global Housing Market Analysis (2015–2024)](https://www.kaggle.com/datasets/atharvasoundankar/global-housing-market-analysis-2015-2024)** was obtained from **Kaggle**.  
It covers global housing and economic indicators from 2015 to 2024 for multiple countries, focusing on housing affordability, prices, and urban development.

The data was imported into R and prepared for analysis. Initial inspection (using `head()` and `View()`) confirmed proper structure and variable names.

---

## 🪜 **Step 2: Feature Selection**
The dataset originally contained 11 variables, including housing, rent, inflation, and construction indexes.  
For this study, only the variables relevant to **urbanization and housing affordability** were retained:

| Variable | Description |
|-----------|--------------|
| **Country** | Name of the country |
| **Year** | Year of observation |
| **House Price Index** | Relative measure of housing prices (base = 100) |
| **Affordability Ratio** | Median house price divided by median household income |
| **Urbanization Rate (%)** | Percentage of population living in urban areas |
| **Population Growth (%)** | Annual population growth rate |

These features were selected because they best capture the relationship between **urbanization** and **housing affordability** trends globally.

---

## 🪜 **Step 3: Data Cleaning**
A comprehensive data cleaning process was performed to ensure data quality and reliability.

### 🔹 Missing and Duplicate Values
- The dataset was checked for missing and duplicate values.  
- No missing values or duplicate records were found.  
- The dataset is complete and required no imputation.

### 🔹 Outlier Detection
- Boxplots were used to visually inspect outliers in key numerical variables.  
- No extreme or influential outliers were observed.  
- All values fall within reasonable ranges.

### 🔹 Text Cleaning
- Leading, trailing, and extra spaces were removed from country names.  
- This ensured consistency during grouping and aggregation.

### 🔹 Data Type Standardization
- Numeric variables were verified and standardized.  
- The dataset structure was confirmed to be suitable for statistical analysis.

---

## 🪜 **Step 4: Data Transformation**
Several transformations were applied to enhance analytical depth.

### 🔹 Derived Variable — *Price-to-Income Ratio*
A new affordability metric was created to better represent the relationship between house prices and income levels.  
This metric provides deeper insight into housing affordability trends.

### 🔹 Urban Growth Categorization
Based on the **Urbanization Rate (%)**, countries were classified into:
- **Low Urban Growth**: Below 65%  
- **Medium Urban Growth**: 65%–80%  
- **High Urban Growth**: Above 80%  

This categorization enables meaningful comparison across different levels of urban development.

### 🔹 Country-Level Summary Dataset
Data was aggregated at the country level to compute average values for:
- House Price Index  
- Affordability Ratio  
- Price-to-Income Ratio  
- Urbanization Rate  
- Population Growth  

This summarized dataset highlights macro-level housing and urbanization trends.

---

## 🪜 **Step 5: Exploratory Data Analysis (EDA)**
Exploratory analysis was conducted to identify relationships and trends among variables.

### 🔹 Descriptive Statistics
Summary statistics were used to analyze distributions, central tendencies, and variability.

### 🔹 Correlation Analysis
A correlation matrix and heatmap revealed:
- A strong relationship between affordability measures and house prices  
- A moderate association between urbanization and housing prices  
- A weaker influence of population growth

### 🔹 Visualization
Multiple plots were created, including:
- Histograms for distribution analysis  
- Boxplots comparing urban growth categories  
- Scatter plots illustrating affordability and urbanization effects  
- Country-level bar charts  
- Time-series plots of housing prices over years  

These visualizations clearly demonstrate how urbanization intensifies housing affordability challenges.

---

## 🪜 **Step 6: Predictive Modeling & Machine Learning**
Predictive modeling was performed to estimate housing prices using economic and urban indicators.

### 🔹 Models Implemented
- **Multiple Linear Regression** to analyze linear relationships  
- **Random Forest Regression** to capture non-linear patterns

### 🔹 Model Evaluation
Models were evaluated using:
- Root Mean Square Error (RMSE)  
- Mean Absolute Error (MAE)

The Random Forest model achieved better predictive performance.

### 🔹 Feature Importance
Feature importance analysis showed:
- **Affordability Ratio**
- **Price-to-Income Ratio**

as the most influential predictors of housing prices.

---

## 🪜 **Overview of Results**
- The dataset consists of **200 year-level observations** and a summarized country-level dataset.  
- Urbanization is strongly associated with rising house prices and reduced affordability.  
- Machine learning models outperform traditional regression methods.  
- The project successfully demonstrates a complete **data science lifecycle**.

---

## 👥 **Group Members**
- Maryam Tahir  
- Yashfeen Fatima  
- Esha Ashfaq  

---

## 🛠️ **Tools Used**
- R (readr, dplyr, ggplot2, tidyr, GGally, randomForest)

---

## 📊 **Data Source**
[Kaggle – Global Housing Market Analysis (2015–2024)](https://www.kaggle.com/datasets/atharvasoundankar/global-housing-market-analysis-2015-2024)
