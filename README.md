# 🎮 Video Game Sales Analysis: Identifying Success Drivers
## Data Preparation and Exploratory Data Analysis (EDA)

This project analyzes historical sales data for **video games** from the global market, including user and critic ratings, genres, and platforms (e.g., Xbox, PlayStation). The data is available up to **December 2016**.

My primary task as a Data Analyst was to **identify the patterns that determine game success** to allow the company ("Streamchik" online store) to bet on potentially popular products and effectively plan marketing campaigns for the upcoming year (2017).

---
### 📌 Reproducible Data Science Pipeline

The analysis follows a reproducible DS pipeline: 

<img width="724" height="187" alt="image" src="https://github.com/user-attachments/assets/7fb27933-0708-449a-8f82-9bae6d03a669" />


---
## 🎯 Objectives / Analyst Role

My role involved the following steps:
- **Prepare high-quality data** (cleaning, structuring, type conversion).
- **Identify the relevant period** for forecasting (2014-2016).
- **Determine key market patterns** across platforms and genres.
- **Create a user portrait** for each major region (NA, EU, JP).
- **Test statistical hypotheses** regarding user ratings.

---
## ✔ Execution Summary

### 1. Data Inspection and Error Correction

---
### 2. Cleaning and Standardization
- Converted all column names to **snake_case** (lowercase).
- Standardized data types as described above.

**Result:** Consistent column names and reliable data types for calculations.

---
### 3. Feature Engineering
Created one essential feature for analysis:
- **`total_sales`**: The sum of sales across all regions (NA, EU, JP, Other).

---
### 4. Exploratory Data Analysis (EDA)

Conducted visual and statistical analysis of key game characteristics:

#### • Determining the Relevant Period
- The analysis focuses on the period **2014-2016** as the most actual data for the 2017 forecast.

#### • Platform Analysis
- **Top Total Sales (2014–2016):** **PS4** (**288.15 million copies**), **XOne** (**140.36 million**), **3DS** (**86.68 million**).
- **Platform Lifespan:** Platforms typically appear and disappear within a characteristic span of **~10 years**.
<img width="548" height="249" alt="image" src="https://github.com/user-attachments/assets/489183e0-08f1-4f86-b22b-eca002f73253" />

- **Median Sales (2014–2016):** **XOne** slightly leads in median sales (0.205 million copies), but the difference with PS4 and WiiU is insignificant.
- **Outliers ("Stars"):** PS4, XOne, and WiiU have the highest outliers, indicating individual games with very high sales volumes.
<img width="636" height="538" alt="image" src="https://github.com/user-attachments/assets/05000d9b-2bed-4e39-a32d-66a0fcfa080d" />




#### • Score Influence on Sales
- **Finding**: **Critics and users** do not demonstrate a strong direct correlation with sales.
- Many games with high critic scores have weak sales.

#### • Genre Distribution
- **Most Profitable Genres (by median sales):** Shooter (**0.24 million**), Role-Playing (**0.20 million**), and Sports (**0.19 million**).
- **Least Profitable Genres:** Adventure, Puzzle, Strategy (median below **0.07 million**).

---
## 5. User Portrait by Region (2014–2016)

<img width="627" height="227" alt="image" src="https://github.com/user-attachments/assets/220a33b6-78d8-4e10-958f-9c2c478d3190" />

---
## 6. 🔬 Hypothesis Testing

**Alpha threshold (Significance level):** **0.05**.

### 6.1. Platform Ratings Hypothesis (Xbox One and PC)
- **H₀ (Null Hypothesis):** The average user ratings for Xbox One and PC platforms are **the same**.
- **H₁ (Alternative Hypothesis):** The average user ratings for Xbox One and PC platforms are **different**.
- **Result:** The average user ratings for Xbox One and PC **do not statistically differ**.

### 6.2. Genre Ratings Hypothesis (Action and Sports)
- **H₀ (Null Hypothesis):** The average user ratings for Action and Sports genres are **the same**.
- **H₁ (Alternative Hypothesis):** The average user ratings for Action and Sports genres are **different**.
- **Result:** The average user ratings for Action and Sports genres **statistically differ**.

---
## 7. 💡 General Conclusion

The analysis is focused on the relevant period **2014-2016** to predict sales for 2017.

**Key Recommendations for 2017:**
1.  **Platforms:** Focus on **PS4** and **XOne** as the leading platforms in total sales and potential profitability. For the Japanese market, **3DS** remains the priority.
2.  **Genres:** Invest in marketing campaigns for **Shooter**, **Sports** (high median sales), and **Role-Playing** (stability, especially in JP).
3.  **Marketing:**
    * **NA/EU:** Emphasize content with an **"M" (Mature)** rating, as it generates the largest share of revenue.
    * **JP:** Advertising must account for the strong preference for the **Role-Playing** genre and the **3DS** platform.

These insights create a reliable foundation for strategically allocating advertising budgets and selecting games for procurement in 2017.
