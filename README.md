# 📊 Pandas Advanced Implementation Project

This repository contains 5 practical Pandas-based data manipulation tasks that cover advanced-level operations such as time series handling, pivoting, multi-indexing, categorical optimization, and working with file formats like Parquet and CSV.

---

## 🔧 Implementation Tasks

### 1. 📅 Time-Indexed Data Handling
- **Objective**: Resample time series data and handle missing values using interpolation.
- **Operations**:
  - Create a `DatetimeIndex`.
  - Use `.resample()` to aggregate values over time intervals.
  - Apply `.interpolate(method='time')` to fill in missing data points.
- **Use-case**: Useful in processing stock prices, IoT sensor data, or daily sales tracking.

---

### 2. 🔄 Pivot and Melt DataFrames
- **Objective**: Convert data between long and wide formats.
- **Operations**:
  - Use `.pivot()` to reshape data from long to wide.
  - Use `pd.melt()` to convert data back from wide to long.
- **Use-case**: Great for reporting, visualization, and Excel-style transformations.

---

### 3. 🧮 Multi-Index DataFrame Creation and Query
- **Objective**: Create a DataFrame with hierarchical indexing and query by index level.
- **Operations**:
  - Create a `MultiIndex` using `pd.MultiIndex.from_arrays()`.
  - Slice and filter using `.loc[]` and `.xs()` (cross-section).
- **Use-case**: Used in grouped data analysis such as sales by region and year.

---

### 4. 🧠 Categorical Conversion and Memory Optimization
- **Objective**: Convert string columns to categorical types and compare memory usage.
- **Operations**:
  - Use `.astype('category')` for optimization.
  - Measure memory with `.memory_usage(deep=True)`.
- **Use-case**: Essential when working with large datasets containing repeated labels (like cities, product names, etc.).

---

### 5. 🏁 Parquet vs CSV Performance Benchmark
- **Objective**: Compare performance of reading/writing CSV vs. Parquet files.
- **Operations**:
  - Use `.to_csv()` / `.read_csv()` for CSV.
  - Use `.to_parquet()` / `.read_parquet()` for Parquet.
  - Time the operations with `time.time()`.
- **Use-case**: Helps choose the best storage format for performance and size efficiency.

---

## 🛠 Requirements

- Python 3.7+
- pandas
- pyarrow or fastparquet (for Parquet)
- numpy (optional)

```bash
pip install pandas pyarrow
```
---
## 📌 Key Takeaways
Understand real-world Pandas workflows.

Learn performance tradeoffs between formats.

Practice with time series, reshaping, and memory optimization.
