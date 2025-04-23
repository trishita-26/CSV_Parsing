
```markdown
# CSV Cleaner and Parser 🧹📊

This project provides a lightweight and effective Python script for cleaning and parsing CSV files. It's ideal for preprocessing raw datasets during data engineering workflows.

## 🔧 Features

- ✅ Removes duplicate rows
- ✅ Drops rows with all missing values
- ✅ Strips whitespace and standardizes string columns (lowercase)
- ✅ Fills missing values with `"missing"`
- ✅ Generates a log file for data cleaning activity

## 📁 File Structure

```
CSV_Parsing/
├── cleaner.py             # Main Python script for cleaning CSVs
├── raw.csv                # Example input CSV (for demo/testing)
├── cleaned.csv            # Cleaned output CSV
├── logs/
│   └── clean_log.txt      # Logs for cleaning steps and file status
└── README.md              # Project documentation
```

## 🚀 Getting Started

### 🔨 Requirements

- Python 3.x
- pandas

Install dependencies:
```bash
pip install pandas
```

### ⚙️ How to Use

#### 1. Clone the Repository
```bash
git clone https://github.com/trishita-26/CSV_Parsing.git
cd CSV_Parsing
```

#### 2. Run the Script

```bash
python cleaner.py --input raw.csv --output cleaned.csv
```

This will:
- Clean the data from `raw.csv`
- Save the output to `cleaned.csv`
- Log the process in `logs/clean_log.txt`

> 📝 Make sure the `logs/` directory exists. The script creates it automatically if missing.

### 🧪 Sample Input (`raw.csv`)
```
Name,Age,Email
alice,25.0,alice@example.com
bob,,bob@example.com
charlie,30.0,
alice,25.0,alice@example.com
david,28.0,david@sample.com
eve,22.0,eve@example.com
```

### ✅ Sample Output (`cleaned.csv`)
```
Name,Age,Email
alice,25.0,alice@example.com
bob,missing,bob@example.com
charlie,30.0,missing
david,28.0,david@sample.com
eve,22.0,eve@example.com
```

## 💡 Use Cases

- Initial data cleaning before loading into a database or data warehouse
- Preprocessing CSV files before analysis or visualization
- Learning and showcasing data engineering practices

## 🧑‍💻 Author

👤 [Trishita](https://github.com/trishita-26)  
Engineering student with a passion for building data pipelines and automation tools.

---

### 📬 Feedback

If you found this useful or have suggestions to improve, feel free to open an issue or star the repo ⭐

```

---

Let me know if you want to add a badge (e.g., Python version, license) or link this project to a blog or LinkedIn post!
