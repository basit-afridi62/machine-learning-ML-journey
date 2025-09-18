# SQL Database Operations with Pandas

This notebook demonstrates how to connect to a **MySQL database**, run SQL queries, and convert results into Pandas DataFrames for analysis.

---

## 📂 Dataset Organization

Keep all datasets in the same sequence as they are in the repository.  
For most locally uploaded datasets, the path is structured as:
../datasets/world.sql


Here:
- `..` → means going one folder back  
- Then open `datasets` folder  
- Select `world.sql` file to run  

⚠️ **Important:**  
Ensure your datasets follow this folder structure, or manually set your dataset path if needed.

---

## 🌍 World Dataset

- **Dataset Source:** [Kaggle - World SQL Dataset](https://www.kaggle.com/busielmorley/worldcities-pop-lang-rank-sql-create-tbls?select=world.sql)  
- Or use the `world.sql` file already present in the `datasets` folder of the repository.

### ⚙️ Setup Instructions
1. Run the `world.sql` file inside your **WAMP** or **XAMPP** server to create the `world` database.
2. Ensure MySQL server is running locally on your machine.
3. yu can download the video to see that how world.sql can be run on WampServer.

---

## 🔧 Requirements

- Python 3.11+
- MySQL Server (WAMP / XAMPP)
- mysql-connector-python
- Pandas

Install the required Python packages:

```bash
pip install mysql-connector-python pandas
