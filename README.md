# 🏥 National Health Insurance – Big Data Capstone Project

**Name:** Manzi Delphin  
**ID:** 26021  
**Group:** E  
**Course:** Introduction to Big Data Analytics  
**Instructor:** Eric Maniraguha  
**Academic Year:** 2024–2025, Semester III

---

## 📁 Project Files & Links

- 🔗 **Dataset Used**: [Health Insurance Dataset (CSV)](https://drive.google.com/file/d/1F_jX5rBTG5SgXLhvQKNcsauHe4uBx8Ez/view?usp=drive_link)  
- 📊 **Power BI Dashboard**: [Power BI Project Folder](https://drive.google.com/drive/folders/1vREgCCeBvOl0GlEBufvNIAWMhZszEftN?usp=drive_link)  
- 📽️ **PowerPoint Presentation**: [Capstone Slides](https://docs.google.com/presentation/d/14-2x7pPbJeggJ1BNIWLzI-pz5HAHLQXp/edit?usp=drive_link)

---

## ✅ PART 1: PROBLEM DEFINITION & PLANNING

### 🏷️ I. Sector Selection
☑ **Health**

### ❓ II. Problem Statement  
> This project investigates disparities and patterns in national health insurance coverage across countries using survey-based health indicators. Using big data analytics, it aims to identify trends across demographics, regions, and years to support equitable policy decision-making.

### 📦 III. Dataset Identification  
- **Dataset Title:** National Health Insurance – Global DHS Indicators  
- **Source Link:** [Dataset Download](https://drive.google.com/file/d/1F_jX5rBTG5SgXLhvQKNcsauHe4uBx8Ez/view?usp=drive_link)  
- **Number of Rows and Columns:** 15,000+ rows × 20 columns  
- **Data Structure:** ☑ Structured (CSV)  
- **Data Status:** ☑ Requires Preprocessing

---

## 🐍 PART 2: PYTHON ANALYTICS TASKS

### ➡️ 1. Clean the Dataset
We began by inspecting for missing values, inconsistent formats, and extreme outliers. String values were normalized, and outliers in numerical fields were capped using IQR.

<img width="758" height="268" alt="Part 2 1 1 Handle missing values, inconsistent formats, and outliers" src="https://github.com/user-attachments/assets/538d93eb-611a-4022-8f34-761415880031" />


### ➡️ 2. Apply Data Transformations
Categorical values were encoded using LabelEncoder, and numerical features such as age, household size, and insurance value were scaled using StandardScaler to ensure modeling fairness.

<img width="996" height="717" alt="Part 2 1 2 data transformations" src="https://github.com/user-attachments/assets/366540b7-ba87-4aa8-8595-ed701d4d268c" />


---

### ➡️ 3. Conduct Exploratory Data Analysis (EDA)

We analyzed central tendencies, distributions, and correlations between variables. This helped us detect relationships and understand variable behavior.

#### Descriptive Statistics
<img width="991" height="731" alt="Part 2 2 1 Generated descriptive statistics " src="https://github.com/user-attachments/assets/d9106d65-a689-4ca7-921e-9a7ecfca468d" />


#### Distribution Visuals
We used histograms and boxplots to observe feature spread and detect skews and group variances.

<img width="975" height="647" alt="Part 2 2 2 Visualized distributions" src="https://github.com/user-attachments/assets/37483448-5dca-4e17-a53d-47845ebe4754" />

<img width="991" height="392" alt="Part 2 2 2 Boxplot of Numeric Features" src="https://github.com/user-attachments/assets/595cdebb-266a-4c13-952b-4f317819b2c6" />


#### Correlation Analysis
This heatmap revealed strong and weak linear relationships between numeric indicators, guiding feature selection.

<img width="980" height="730" alt="Correlation Heatmap of Numeric Features" src="https://github.com/user-attachments/assets/693fe0ce-06d0-4a6d-a2de-7d5fea1c8d97" />


---

### ➡️ 4. Apply ML / Clustering

Given the nature of the health indicators, we used **K-Means Clustering** to group similar health insurance profiles.

#### Optimal Cluster Count
The elbow method was used to determine the best number of clusters (k).

<img width="978" height="483" alt="Elbow Method for Optimal K" src="https://github.com/user-attachments/assets/77432a1a-d2df-462f-909a-3b11df509b72" />


#### Cluster Visualization
We plotted clusters to identify patterns of insurance coverage and access grouped by similarity.

<img width="980" height="583" alt="Health Insuarance Types Clustered by coverage" src="https://github.com/user-attachments/assets/3b0a2717-a029-473e-b2a7-897515dc30a0" />


---

### ➡️ 5. Evaluate the Model

We evaluated clustering using the **Silhouette Score**, which indicated good separation and cohesion. For classification attempts, **Accuracy**, **Precision**, and **F1-Score** were computed.

---

### ➡️ 6. Structure Code & Add Innovation

- All code was modular with reusable functions
- Markdown cells explained each step
- A custom risk score metric was developed for households
- Feature importance from clustering enhanced interpretability

---

## 📊 PART 3: POWER BI DASHBOARD TASKS

### ➡️ 1. Communicate the Problem & Insights
> The Power BI dashboard enables exploration of health insurance indicators by year, country, region, and demographic. It communicates disparities, trends, and patterns clearly.

### ➡️ 2. Incorporate Interactivity
- **Slicers** for `SurveyYear`, `Country`, `Indicator`, `CharacteristicCategory`
- **Drill-through** pages from overall indicators to demographic-specific reports

### ➡️ 3. Use Appropriate Visuals
- **Line Chart**: Trends over time
- **Clustered Column Chart**: Top indicators per region
- **Map**: Insurance values by country
- **Pie Chart**: Demographic proportions
- **Bar Chart**: Value per country

### ➡️ 4. Ensure Design Clarity
- Color theme: Blue/White (healthcare standard)
- Clearly labeled visuals, logical layout, grouped by insights
- KPI cards at the top for total indicators, average values

### ➡️ 5. Add Innovative Features
- Custom tooltips with CIHigh/CILow and precision
- DAX formulas: Value change, CI range
- AI Visual: Key influencers affecting insurance value
- Bookmarks to toggle between views

#### Problem Statement 

<img width="1282" height="711" alt="Problem Statement" src="https://github.com/user-attachments/assets/4525502c-9cd8-43ff-8ea5-1a51411602e8" />

#### 🌐 Final Dashboard

<img width="1236" height="718" alt="Power Bi Dashboard" src="https://github.com/user-attachments/assets/1da1639f-deba-428a-80dd-a88ee515f70f" />


---

## 📨 PART 4: SUBMISSION & COMMUNICATION

### 🔍 GitHub Repository Contents:
- `dataset/cleaned_health_insurance_rwa.csv`
- `notebooks/analysis.ipynb`
- `dashboard/insurance_dashboard.pbix`
- `images/` folder
- `README.md` (this file)

### 📅 PowerPoint Presentation Includes:
- Introduction and Objective  
- Data Cleaning and Analysis Methods  
- Clustering and Modeling Results  
- Power BI Dashboard Walkthrough  
- Recommendations and Next Steps

---

## 🙏 Thank You

> *Big data enables us to move beyond anecdotal assumptions toward data-driven policies that expand access to health care for all.*
