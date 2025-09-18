# JSON File Operations with Pandas

This notebook demonstrates how to work with **JSON files** in Python using **pandas**.  
It covers reading JSON data from both **local files** and **URLs** and converting them into DataFrames for analysis.

---

## 📂 Dataset Organization

Keep all the datasets in the same sequence and structure as they are in the repository.  
For maximum datasets uploaded locally, the path used is:

```
../datasets/dataset_name.json
```

Here:
- `..` means **go one folder back** from the current file location.
- Then enter the `datasets` folder.
- Finally, select the `dataset.json`.

You can manually set your path if you store your datasets elsewhere.  
Maintaining this folder structure is recommended for smooth execution.

---

## 📖 Learning Resource

For more details, refer to the official pandas documentation:  
🔗 **[pandas.read_json](https://pandas.pydata.org/docs/reference/api/pandas.read_json.html)**

---

## 📌 Notebook Content

### 1️⃣ Uploading JSON File from Local Storage
- Loads a local `titanic.json` file using:
```python
pd.read_json('../datasets/titanic.json')
```
- Displays the contents as a DataFrame with rows and columns.

### 2️⃣ Loading JSON File from a URL
- Demonstrates reading JSON data directly from a remote source:
```python
pd.read_json('https://raw.githubusercontent.com/ybifoundation/Dataset/main/Titanic.json')
```
- Converts the online dataset into a DataFrame for quick analysis.

---

## 🛠️ Requirements
- Python 3.11+
- pandas (latest version recommended)

Install pandas if you haven't already:
```bash
pip install pandas
```

---

## ✅ Summary
This notebook is a quick reference for reading and working with JSON data.  
It provides examples for both **local** and **remote** JSON files, keeping the dataset path structure consistent for reproducibility.
