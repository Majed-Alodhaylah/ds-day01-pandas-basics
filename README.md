# 📊 Student Data Analysis Project  

A project focused on **cleaning, analyzing, and visualizing student data**, with the goal of extracting useful insights and KPIs (Key Performance Indicators).  

## 📂 Project Structure

DAY01\_PANDAS\_BASICS/
│── data/
│   └── students\_medium\_dirty.csv    # Raw dataset
│
│── outputs/
│   ├── cleaned\_students.csv         # Cleaned dataset
│   └── students\_Kpis.csv            # KPIs results
│
│── notebook.ipynb                   # Main analysis notebook
│── requirements.txt                 # Required dependencies
│── README.md                        # Project documentation



## 🛠️ Libraries Used
- **pandas** → Data cleaning and manipulation.  
- **matplotlib** → Basic data visualization.  
- **seaborn** → Advanced statistical visualization (Boxplot, Heatmap, Histplot).  

## 📊 Workflow

1. **Data Loading**  

   df = pd.read_csv("data/students_medium_dirty.csv")

2. **Data Exploration**

   * `df.head()` → Preview first 5 rows.
   * `df.info()` → Data types and missing values.
   * `df.describe()` → Summary statistics.

3. **Data Cleaning**

   * Remove duplicates → `df.drop_duplicates()`
   * Handle missing values with median → `df["math"].fillna(df["math"].median())`
   * Standardize column values (e.g., Gender → Male/Female).
   * Remove invalid or unrealistic values (Outliers).

4. **Data Analysis**

   * Find top/bottom students in each subject.
   * Calculate averages (KPIs) and export results.
   * Compute correlations → `df.corr()`.

5. **Data Visualization**

   * 📊 **Histogram** → Distribution of math scores.
   * 📦 **Boxplot** → Compare science scores by gender.
   * 🔵 **Scatterplot** → Relationship between attendance and math.
   * 🌡️ **Heatmap** → Correlation between all subjects.

## 📈 Outputs

* **cleaned\_students.csv** → Final cleaned dataset.
* **students\_Kpis.csv** → Contains performance metrics:

  * Average Math
  * Average English
  * Average Science
  * Average Attendance

## 🚀 How to Run

1. Clone the repository:

   git clone
   cd DAY01_PANDAS_BASICS

2. Install dependencies
   pip install -r requirements.txt

3. Open the Jupyter Notebook:

   jupyter notebook

4. Run all cells to reproduce results and visualizations.


## 📌 Key Learnings

* Data cleaning and preprocessing with **pandas**.
* Handling missing values and duplicates.
* Extracting KPIs from raw data.
* Building visualizations to understand patterns and correlations.
* Exporting cleaned datasets for further use.

