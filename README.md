# Vehicle Dataset Analysis with Pandas

This repository contains a Data Analysis project executed in Google Colab using Python and Pandas. The project focuses on indexing, filtering, and querying a car sales dataset (`cars_dataset.csv`) containing 500 records.

---

## 📊 Dataset Overview

The dataset (`cars_dataset.csv`) comprises 500 rows and 12 vehicle-related attributes:

| Column Name | Description |
| :--- | :--- |
| **Manufacturer** | Vehicle maker (e.g., Audi, Toyota, BMW) |
| **Model** | Specific model name (e.g., A4, Corolla, X5) |
| **Sales_in_thousands** | Total sales units (in thousands) |
| **__year_resale_value** | Estimated resale value after one year |
| **Vehicle_type** | Category (Passenger or SUV) |
| **Price_in_thousands** | Vehicle price (in thousands USD) |
| **Engine_size** | Engine capacity in Liters |
| **Horsepower** | Vehicle engine power Output |
| **Wheelbase** | Distance between front and rear wheels (inches) |
| **Width** | Vehicle width (inches) |
| **Length** | Vehicle length (inches) |
| **Curb_weight** | Total vehicle weight (in thousands of lbs) |

---

## 🚀 Key Features & Operations

The notebook demonstrates fundamental Pandas data manipulation operations:

* **Data Loading**: Reading CSV files into Pandas DataFrames.
* **Direct Column Selection**: Extracting series and specific values via direct index reference (`df['Model'][0]`).
* **Label-Based Selection (`.loc`)**:
  * Range slicing by column names (`df.loc[0:5, ['Manufacturer', 'Vehicle_type']]`).
  * Multi-condition boolean filtering (`df.loc[(df.Manufacturer == 'Audi') & (df.Engine_size == 2.1)]`).
* **Positional Selection (`.iloc`)**:
  * Slicing specific rows and numeric column positions (`df.iloc[0:5, [0, 1, 2, 3, 4]]`).
  * Subsetting entire columns or row slices.
* **Boolean Masking**: Generating boolean vectors to filter datasets dynamically.

---

## 💻 Tech Stack

* **Language**: Python 3
* **Libraries**: `pandas`, `numpy`
* **Environment**: Google Colab / Jupyter Notebook

---

## 🛠️ Usage Instructions

1. Clone this repository or download the `.ipynb` notebook file.
2. Ensure you have the dataset uploaded in your execution directory under the name `cars_dataset.csv`.
3. Run the notebook using Google Colab or Jupyter Notebook:
   ```bash
   pip install pandas numpy
   jupyter notebook
