# Titanic Data Analysis – Task 1

This project performs **exploratory data analysis (EDA)** on the Titanic dataset as part of Task 1. The goal is to analyze the dataset visually and statistically to identify important patterns and trends.

📁 **Dataset used**: `task1_Titanic-Dataset.csv`

---

## 📂 Files Included

| File Name                  | Description                                                    |
|----------------------------|----------------------------------------------------------------|
| `task1_Titanic-Dataset.csv` | Original Titanic dataset                                       |
| `cleaned_titanic.csv`        | Cleaned dataset after removing irrelevant columns              |
| `Task2_Intern.ipynb`         | Jupyter Notebook with code, outputs, and visual analysis        |

---

## ✅ Tasks Performed

### 1️⃣ Generate summary statistics (mean, median, std, etc.)
- Used `describe()` and `median()` to calculate statistical summaries.
- Analyzed central tendency and spread of numerical features: `Pclass`, `Age`, `SibSp`, `Parch`, `Fare`.

### 2️⃣ Create histograms and boxplots for numeric features
- Plotted **histograms** with KDE to understand feature distributions.
- Used **boxplots** to detect outliers in variables like `Age` and `Fare`.

### 3️⃣ Use pairplot/correlation matrix for feature relationships
- Created a **pairplot** (`seaborn.pairplot`) to visualize pairwise relationships colored by survival status.
- Generated a **correlation matrix** heatmap to observe linear relationships between features and the target (`Survived`).

---

## 🔍 4️⃣ Identify Patterns, Trends, or Anomalies

- **Outliers**: Strong outliers observed in `Fare` and `Age`.
- **Skewness**: Features like `Fare` show a skewed distribution (heavily concentrated at low values).
- **Correlations**:
  - `Fare` and `Survived`: Positive correlation → higher fare associated with survival.
  - `Pclass` and `Fare`: Negative correlation → lower class, lower fare.
  - `Age` and `Survived`: Slight negative relationship → older passengers less likely to survive.

---

## 📈 5️⃣ Basic Feature-Level Inferences from Visuals

- **Fare**: Survivors generally paid higher fares → wealthier passengers had better survival chances.
- **Age**: Survivors were slightly younger on average; children had higher survival.
- **Pclass**: First-class passengers (Pclass = 1) had higher survival rates than second or third class.
- **SibSp**: Passengers with 1–2 siblings/spouses had slightly higher survival than those alone or in large families.
- **Parch**: No strong pattern, but small family groups may have had slightly better outcomes.

---

## 🛠️ Libraries Used

- **Pandas** – data handling
- **NumPy** – numerical operations
- **Seaborn** and **Matplotlib** – visualizations

---

## 📌 Conclusion

This analysis of the Titanic dataset provides insights into passenger survival based on fare, class, age, and family structure. These findings were derived through statistical summaries and visual EDA, helping build a foundation for future predictive modeling.

---
