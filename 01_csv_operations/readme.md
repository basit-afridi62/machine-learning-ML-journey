# 📂 CSV Operations with Pandas

This repository demonstrates **step-by-step CSV operations using pandas**, following the same sequence as in the Jupyter Notebook (`csv-operations.ipynb`).  

The goal is to practice reading, cleaning, transforming, and saving CSV data using **pandas** in Python.

---

## 📁 Folder & File Structure

Keep all the datasets in the same sequence as in this repo.  
For most datasets uploaded locally, the path is:

```
../datasets/dataset_name.csv
```

Where:

- `..` → means "go one folder back"
- `datasets` → is the folder containing all CSV files
- `dataset_name.csv` → is the specific dataset you want to load

So keep your dataset and file in this order, or you can manually set your path if needed.

Example:

```python
import pandas as pd

df = pd.read_csv("../datasets/titanic.csv")
print(df.head())
```

---

## 📖 Covered Topics

This notebook demonstrates the following operations:

1. **Importing pandas**  
2. **Opening a CSV file located on your PC**  
3. **Opening a CSV file from a URL**  
4. **Using `sep` parameter** (for comma, tab, or other delimiters)  
5. **Using `index_col` parameter**  
6. **Renaming columns**  
7. **Selecting specific columns**  
8. **Handling missing values (`NaN`)**  
9. **Replacing empty cells with NaN**  
10. **Filling missing values**  
11. **Dropping rows/columns**  
12. **Using `na_values` parameter**  
13. **Using `converters` parameter** (apply custom functions while reading)  
14. **Saving DataFrames back to CSV**  
15. **Basic exploration (`info()`, `head()`, `describe()`)**

---

## 📖 Reading CSV Files

We primarily use [`pandas.read_csv`](https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html) to load CSV files.

Example:

```python
import pandas as pd

df = pd.read_csv("../datasets/iris.csv")
print(df.info())
```

---

## 🛠 Tools & Libraries

- **Python 3**
- **pandas** → For data manipulation
- **Jupyter Notebook** → For interactive learning

---

## 💡 Notes

- Keep the same folder structure as shown, or update paths manually.
- All datasets in this notebook follow the pattern:  
  `../datasets/dataset_name.csv`
- For external URLs, ensure you have an active internet connection.

---

## 📚 Recommended References

- [pandas.read_csv() Documentation](https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html)  
- [pandas User Guide](https://pandas.pydata.org/docs/user_guide/index.html)

---

