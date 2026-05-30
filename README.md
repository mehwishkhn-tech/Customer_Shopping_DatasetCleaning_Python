# Customer_Shopping_DatasetCleaning_Python
# 🛍️ Customer Shopping Behavior Analysis
## Step 1: Data Cleaning (Python)

### 📌 Project Overview
This project analyzes customer shopping behavior across 
multiple shopping malls in Istanbul, Turkey. This file 
covers the data cleaning process performed using Python 
and Pandas before loading the data into PostgreSQL for 
analysis and Power BI for visualization.

---

### 👩‍💻 Author
**Mehwish Nisha Khan**

---

### 🛠️ Tools & Libraries Used
- **Python 3.14**
- **Pandas** — data manipulation and cleaning
- **NumPy** — numerical operations
- **Matplotlib** — data visualization
- **Seaborn** — statistical visualization

---

### 📂 Dataset
- **Source:** Kaggle
- **Dataset Name:** Customer Shopping Dataset - Retail Sales Data
- **Total Rows:** 99,457
- **Total Columns:** 10 (original) → 12 (after cleaning)

#### Original Columns:
| Column | Description |
|--------|-------------|
| invoice_no | Unique invoice number |
| customer_id | Unique customer ID |
| gender | Gender of customer |
| age | Age of customer |
| category | Product category purchased |
| quantity | Number of items purchased |
| price | Price per item |
| payment_method | Mode of payment |
| invoice_date | Date of purchase |
| shopping_mall | Shopping mall name |

---

### 🧹 Data Cleaning Steps Performed

#### Step 1 — Imported Libraries
Imported Pandas, NumPy, Matplotlib and Seaborn for 
data cleaning and analysis.

#### Step 2 — Loaded Dataset
Loaded the raw CSV file into a Pandas DataFrame and 
confirmed the shape as (99,457 rows × 10 columns).

#### Step 3 — Explored the Data
Used df.head(), df.info(), df.describe() and df.dtypes 
to understand the structure and content of the dataset.

#### Step 4 — Checked Missing Values
Checked all columns for null values using df.isnull().sum().
Result: No missing values found in any column ✅

#### Step 5 — Checked & Removed Duplicates
Checked for duplicate rows using df.duplicated().sum().
Result: No duplicate rows found ✅

#### Step 6 — Standardized Column Names
Cleaned all column names by:
- Converting to lowercase
- Removing extra spaces
- Replacing spaces with underscores

#### Step 7 — Created Total Amount Column
Created a new calculated column:
total_amount = quantity × price
Rounded to 2 decimal places using .round(2)
for clean and professional numeric values.

#### Step 8 — Created Age Group Column
Categorized customers into 4 age groups:
| Age Group | Age Range |
|-----------|-----------|
| Young Adult | 18 - 25 |
| Adult | 26 - 35 |
| Middle Aged | 36 - 50 |
| Senior | 51 - 70 |

#### Step 9 — Exported Clean Data
Exported the final cleaned dataset as a new CSV file 
ready for PostgreSQL import.

---

### 📊 Final Clean Dataset
- **Total Rows:** 99,457
- **Total Columns:** 12
- **New Columns Added:** total_amount, age_group
- **Missing Values:** 0
- **Duplicates:** 0

---

### 🚀 Project Workflow
