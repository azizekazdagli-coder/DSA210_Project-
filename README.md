# DSA 210 Introduction to Data Science Course Project
**Student:** Azize Keriman Kazdağlı  

---

## ✈️ Project Overview: Analyzing European Air Traffic Drivers
This project investigates the multifaceted drivers of international air traffic across European Union countries. By merging high-volume flight data (approx. 650,000 records) with socio-economic indicators, the study aims to quantify how a country's economic strength influences travel patterns and identifies non-economic anomalies such as extreme weather events.

## 📊 Milestone 1: Data Collection, EDA, and Hypothesis Testing
In this stage, the project focuses on establishing a robust data pipeline and validating the core research question through statistical rigor. 

### 1. Data Sources & Enrichment
To ensure a comprehensive analysis, the baseline aviation dataset was enriched with the following sources: 
* **Aviation Data:** Daily flight records (departures/arrivals) from European airports (2016-2024). 
* **Economic Indicators:** GDP per capita data obtained from the **World Bank** to represent national purchasing power.
* **Demographic Data:** Population figures from the **World Bank** used to normalize flight counts (Flights per Capita).
* **Visa Statistics:** Schengen visa application and approval rates to analyze inbound traffic constraints.

### 2. Exploratory Data Analysis (EDA)
The analysis utilizes Python (Pandas, Seaborn, Matplotlib) to uncover patterns within the 27 EU member states.
* **Correlation Analysis:** A heatmap was generated to visualize the linear relationship between GDP, population, and flight volumes.
* **Trend Visualization:** Scatter plots with regression lines illustrate the positive correlation between national wealth and outbound travel frequency.
* **Anomaly Detection:** Specific dates with extreme traffic drops (e.g., December 10, 2017 - Storm Ana) were identified to isolate weather-related impacts from economic trends.

### 3. Hypothesis Testing
A formal statistical test was conducted to address the primary research question: 
* **H₀ (Null Hypothesis):** There is no significant correlation between a country's GDP per capita and its outbound flights per capita.
* **H₁ (Alternative Hypothesis):** There is a significant positive correlation between GDP per capita and outbound flight volume.
* **Method:** **Pearson Correlation Coefficient**.
* **Result:** The null hypothesis was rejected ($p < 0.05$), confirming that economic prosperity is a statistically significant driver of air traffic.

## 🛠️ Requirements & Execution
The analysis is contained within a Jupyter Notebook. To reproduce the findings:
1.  Ensure `master_dataset_EU_only.csv` is in the root directory.
2.  Install dependencies: `pip install -r requirements.txt`. 
3.  Run `DSA210_Azize_Milestone1_Final.ipynb`.

## 📈 Future Work
The next phase will involve building predictive models (e.g., Linear Regression, Random Forest) to forecast flight traffic based on the validated economic and policy-related features. 
