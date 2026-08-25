# 📊 Pandas Analyzer & Sales Data Visualization Tool

---

## 🚀 Project Overview

The **Pandas Analyzer & Data Visualization** tool processes sales datasets to uncover business trends, evaluate regional performance, manage missing values, and produce publication-ready statistical charts.

---

## ✨ Key Features

* **Data Cleaning & Handling**: Detects missing records, applies mean imputation, replaces specific values, and handles row drops.
* **Array & Series Manipulation**: Implements column slicing, indexing, element-wise transformations, and multi-frame combination (`concat`, `merge`, `join`).
* **Search, Sort & Grouping**: Offers condition-based record searches, multi-column sorting, and group-level aggregations (`sum`, `mean`, `count`).
* **Descriptive Statistics**: Computes standard deviation, variance, quantiles, and summaries via `describe()`.
* **Multi-Index Pivot Tables**: Generates cross-tabular summaries for multi-dimensional sales analysis.
* **Graphic Export Engine**: Renders interactive Matplotlib/Seaborn figures and exports them to `.png` or `.jpeg` formats.
* **Menu-Driven CLI**: Provides structured numbered prompts for smooth terminal navigation.

---

## 🏗️ Class Architecture & Structure

The system is centered around the `SalesDataAnalyzer` class:

* **Attributes**:
  * `self.data`: Pandas DataFrame storing the active dataset.
* **Methods**:
  * `__init__()` / `__del__()`: Handles instantiation, resource setup, and cleanup.
  * `load_data()`: Reads the dataset from a user-specified CSV path.
  * `explore_data()`: Displays first/last rows, column lists, and schema details.
  * `clean_data()`: Identifies and remedies null or missing values.
  * `mathematical_operations()`: Executes vector and array-level arithmetic.
  * `combine_data()` / `split_data()`: Merges multiple sources or partitions records by region/product.
  * `search_sort_filter()`: Queries records based on custom constraints.
  * `aggregate_functions()`: Summarizes key performance indicators.
  * `statistical_analysis()`: Calculates spread and variance metrics.
  * `create_pivot_table()`: Structures multi-level aggregated views.
  * `visualize_data()`: Plots the chosen chart type using Matplotlib or Seaborn.

---

## 🛠️ Tech Stack

* **Language**: Python 3.8+
* **Data Processing**: Pandas, NumPy
* **Visualization**: Matplotlib, Seaborn
* **Execution Environment**: Terminal CLI / Jupyter Notebook

---

## 📁 Dataset Format

Input files should follow a standard tabular `.csv` layout:

| SalesID | Product   | Region     | Sales | Year | Profit |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 101 | Product A | North | 500 | 2022 | 120 |
| 102 | Product B | East | 600 | 2022 | 150 |
| 103 | Product C | West Coast | 700 | 2022 | 210 |
| 104 | Product D | South | 800 | 2022 | 260 |
| 105 | Product E | Central | 550 | 2022 | 140 |

---

## 🖥️ Menu Options & Functional Flow

* **Option 1 (Load Dataset)**: Prompts for the CSV file location and reads it into memory.
* **Option 2 (Explore Data)**: Previews the head, tail, column inventory, and data types.
* **Option 3 (Perform DataFrame Operations)**: Slices arrays, applies math formulas, and splits data.
* **Option 4 (Handle Missing Data)**: Locates empty cells and applies replacement or removal logic.
* **Option 5 (Generate Descriptive Statistics)**: Summarizes distribution, standard deviation, and variance.
* **Option 6 (Data Visualization)**: Generates user-selected plots based on chosen axis parameters.
* **Option 7 (Save Visualization)**: Exports the current chart figure to an image file.
* **Option 8 (Exit)**: Closes the application gracefully.

---

## 📊 Visualizations Supported

| Chart Type | Engine | Primary Use Case |
| :--- | :--- | :--- |
| **Bar Plot** | Matplotlib / Seaborn | Comparing category-wise performance across regions |
| **Line Plot** | Matplotlib | Tracking continuous sales trends over years |
| **Scatter Plot** | Matplotlib / Seaborn | Correlating metrics (e.g., Sales vs. Profit) |
| **Pie Chart** | Matplotlib | Illustrating percentage market share |
| **Histogram** | Matplotlib | Examining data distribution frequencies |
| **Stack Plot** | Matplotlib | Showing part-to-whole segment contributions |
| **Heatmap & Boxplot** | Seaborn | Analyzing correlation matrices and outlier ranges |

---

## 📂 Project Structure

* `data/`: Folder containing sample CSV datasets (`sales_data.csv`).
* `charts/`: Output directory where exported visualization images are saved.
* `analyzer/`: Python package housing the `SalesDataAnalyzer` class implementation.
* `main.py`: Command-line interface driver script containing the interactive loop.
* `PR9_Visualizer.ipynb`: Jupyter Notebook containing step-by-step experiment cells.
* `requirements.txt`: Package dependency specifications.
* `README.md`: Complete project documentation.

---
