## Part 2: Python Analytics Tasks

### 1. Data Cleaning
- Handled missing values by applying appropriate imputation or removal techniques.
- Standardized column names for consistency and readability.
- Detected and managed outliers to avoid skewed results.
- Converted data types where necessary (e.g., converting coverage rates to float).
- Applied transformations for further analysis (e.g., encoding categorical variables).

---

### 2. Exploratory Data Analysis (EDA)
- Generated descriptive statistics such as mean, median, standard deviation, and range.
- Visualized key distributions and relationships:
  - Coverage rate across districts and provinces.
  - Urban vs. rural coverage differences.
  - Temporal changes in insurance coverage.
- Identified top-performing and underserved districts.

---

### 3. Machine Learning / Clustering Model
- Selected **K-Means Clustering** to group districts based on insurance coverage patterns.
- Determined the optimal number of clusters using the **Elbow Method**.
- Trained the clustering model using selected coverage features.

---

### 4. Model Evaluation
- Used **Silhouette Score** to evaluate the clustering performance.
- Visualized cluster groupings to confirm separation and cohesiveness.

---

### 5. Code Structure & Documentation
- Organized code into modular functions for cleaning, analysis, and modeling.
- Included markdown cells and detailed comments for clarity and reproducibility.

---

### 6. Innovation
- Implemented a **custom scoring function** combining insurance coverage and population type.
- Compared K-Means clustering results with Agglomerative Clustering for deeper insights.