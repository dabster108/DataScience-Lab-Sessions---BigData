
# Big Data Lab Sessions

This repository contains lab exercises and assignments for **Big Data Lab** sessions. The main focus is on **PySpark** for processing large datasets efficiently using Python.

---

## 🔹 Prerequisites

Before starting, ensure your system has the following installed:

- **Java 11** (OpenJDK recommended)  
  PySpark requires Java to run. Java 11 is compatible with PySpark 3.4.

- **Python 3.10**  
  The project and virtual environment use Python 3.10 for compatibility with PySpark.

- **PySpark 3.4**  
  PySpark 3.4 is used to run all Spark jobs.

---

## 🔹 Setup Instructions

Follow these steps to set up your development environment:

1️⃣ **Install Java 11**

- **macOS (Homebrew):**
```bash
brew install openjdk@11
````

* **Linux (Ubuntu):**

```bash
sudo apt update
sudo apt install openjdk-11-jdk
```

* **Windows:**
  Download and install from [Adoptium](https://adoptium.net/) or Oracle.

* **Verify Java version:**

```bash
java -version
```

You should see `java version "11.x.x"`.

---

2️⃣ **Install Python 3.10**

* **macOS (Homebrew):**

```bash
brew install python@3.10
```

* **Linux (Ubuntu):**

```bash
sudo apt install python3.10 python3.10-venv python3.10-dev
```

* **Windows:**
  Download from [Python.org](https://www.python.org/downloads/release/python-3100/).

* **Verify Python version:**

```bash
python3 --version
# or
python3.10 --version
```

---

3️⃣ **Create a Virtual Environment**

```bash
python3.10 -m venv pyspark_env
```

* Activate virtual environment:

  * **macOS / Linux:** `source pyspark_env/bin/activate`
  * **Windows:** `pyspark_env\Scripts\activate`

* Install required packages:

```bash
pip install --upgrade pip
pip install pyspark==3.4.0 pandas matplotlib seaborn
```

---

4️⃣ **Project Structure**

```
bigdata-lab-sessions/
├── Day 01/
│   ├── Assignmentsession.ipynb
│   └── ...
├── Day 02/
│   └── ...
├── pyspark_env/       # Virtual environment (ignored in Git)
├── .gitignore
└── README.md
```

* Make sure to **ignore the virtual environment and .env files** in Git:

```
pyspark_env/
.env
__pycache__/
*.pyc
.DS_Store
```

---

5️⃣ **Running Notebooks**

1. Activate the virtual environment.
2. Start Jupyter Notebook or Lab:

```bash
jupyter lab
# or
jupyter notebook
```

3. Open the relevant notebook in `Day XX/` folder.
4. Run each cell to perform PySpark operations and analyze data.

---

## 🔹 Notes

* Use **PySpark DataFrames** for efficient large-scale data operations.
* Ensure **Java 11** and **Python 3.10** are correctly set; mismatched versions cause runtime errors.
* Follow the order of lab sessions to avoid dependency issues between notebooks.

---

## 🔹 References

* [PySpark Official Documentation](https://spark.apache.org/docs/latest/api/python/)
* [Java 11 Installation Guide](https://adoptium.net/)
* [Python 3.10 Downloads](https://www.python.org/downloads/release/python-3100/)


