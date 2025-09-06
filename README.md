# Pusula_Tuba_Calci
Tuba Çalcı - tubacalci@hotmail.com

# Data Science Intern Case Study

## 📌 Overview
This project was prepared as part of the **Data Science Intern Case Study**.  
The dataset consists of **2,235 observations** and **13 features** related to physical medicine & rehabilitation.  

The **target variable** is:  
➡️ **`TedaviSuresi`** (Treatment duration in sessions)

---

## 📝 Tasks
### Task 1: Exploratory Data Analysis (EDA)
- Data structure exploration (`.shape`, `.info()`, `.describe()`)
- Missing value analysis and visualization
- Distribution plots of numerical and categorical features
- Correlation analysis with `TedaviSuresi`
- Key insights summarized with figures

### Task 2: Data Pre-Processing
- Handling missing values  
  - Median for numerical  
  - Mode/`"Unknown"` for categorical  
- Grouping rare categories under `"Other"`
- Encoding categorical variables using **One-Hot Encoding**
- Standardizing numerical features using **StandardScaler**
- Train/Test split (80/20), consistent and model-ready datasets created
- Validation with a baseline **RandomForest** model (R² ≈ 0.89)

---

## 📂 Project Structure
- `case_study.ipynb` → Main Jupyter Notebook (EDA + Preprocessing)  
- `Talent_Academy_Case_DT_2025.xlsx` → Original dataset  
- `train_ready.csv`, `test_ready.csv` → Preprocessed train/test feature sets  
- `y_train.csv`, `y_test.csv` → Target values for train/test  
- `Case Study - Tuba Çalcı.pdf` → PDF report including findings, visualizations, and insights  
- `README.md` → Project overview & usage instructions  

---

## ⚙️ How to Run

To reproduce the analysis:

1. **Clone this repository**
   ```bash
   git clone https://github.com/tubacalci/Pusula_Tuba_Calci.git
   cd Pusula_Tuba_Calci
   ```
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Jupyter Notebook**
   ```bash
   jupyter notebook case_study.ipynb
   ```

4. **Open the PDF Report**
   Check Case Study - Tuba Çalcı.pdf for a summary of findings and insights.

 ---

   ## 🔑 Key Insights
   - TedaviSuresi is mostly standardized at 15 sessions
   - UygulamaSuresi clusters around 20 minutes
   - High missingness in Alerji, KanGrubu, KronikHastalik columns
   - No strong linear correlation detected with numerical features
   - Gender, Department, Blood Type show only slight variations in treatment duration
   - Final datasets: 1788 rows, 88 features (train) and 447 rows, 88 features (test)
