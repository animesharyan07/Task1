# ETL Data Pipeline –

##  Objective
This project implements an automated **ETL (Extract, Transform, Load) pipeline** using Python, Pandas, and Scikit-learn.

---

##  Dataset
- **Name:** Fashion_Retail_Sales.csv
- **Description:** The dataset includes customer purchase data, product categories, ratings, and mode of payment.
- **Format:** CSV

---

## ETL Pipeline Overview

### 1. **Extract**
- Reads the raw dataset using `pandas.read_csv()`.
- File is passed as input in the `etl_pipeline_func()`.

### 2. **Transform**
- Handles missing values:
  - Numeric columns: Filled with mean or median.
- Encodes categorical data using Label Encoding.
- Scales numeric features using StandardScaler.
- Outliers are detected using the IQR method.
- Rounding applied to selected columns.

### 3. **Load**
- Saves the cleaned and transformed data into a new CSV file (`output_data.csv`).

---

## Technologies Used
- Python 3.x
- pandas
- numpy
- scikit-learn

---

##  How to Run

1. Clone this repository or download the code files.
2. Make sure your directory has:
    - `extract.py`
    - `transform.py`
    - `load.py`
    - `main.py` 
    - `Fashion_Retail_Sales.csv` (input dataset)

3. Install dependencies (if not already):
    ```bash
    pip install pandas scikit-learn numpy
    ```

4. Run the ETL pipeline:
    ```bash
    python main.py
    ```

5. Output will be saved in:
    - `output.csv`

---


