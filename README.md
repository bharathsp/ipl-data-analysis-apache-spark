# 🏏 IPL Data Analysis using Databricks & PySpark

![Databricks + AWS](https://img.shields.io/badge/Platform-Databricks%20%7C%20AWS-orange)
![Language](https://img.shields.io/badge/Language-PySpark-blue)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

### 📌 Project Description

This project focuses on analyzing **Indian Premier League (IPL)** data using **Databricks**, by building an end-to-end data pipeline. Data is read from an **Amazon S3 bucket**, and various transformations are applied using **PySpark** and **Spark SQL** to derive insights and create visualizations.

---

### 🚀 Objectives
- 🔹 Read & process IPL data from AWS S3
- 🔹 Apply data transformations using PySpark
- 🔹 Run analytical queries using Spark SQL
- 🔹 Perform Exploratory Data Analysis (EDA)
- 🔹 Visualize insights using Matplotlib & Seaborn

---

### 🧱 Architecture Diagram

![Data Modeling - Architecture Diagram](https://github.com/user-attachments/assets/5a5b1b1a-b18d-4478-98b5-0b00995765c2)

---

### 📂 IPL Dataset

- **Source**: [Kaggle - IPL Complete Data till 2017](https://www.kaggle.com/datasets/oneplustricks/ipl-complete-data-till-2017)
- **Description**: Ball-by-ball data for all IPL matches (637 matches till 2017 season)

---

### ☁️ Amazon S3

Amazon S3 is a cloud object storage service by AWS that allows you to store any format of data (CSV, Parquet, audio, video, etc.).

#### ✅ Steps to Use:
1. Go to AWS Console → S3 → Create Bucket (e.g., `ipl-data-analysis-project`)
2. Upload the IPL dataset from Kaggle to the bucket.

> 📥 Example path: `s3://ipl-data-analysis-project/Ball_By_Ball.csv`

---

### 🔥 Databricks

Databricks is a unified analytics platform that simplifies big data and AI use cases, built on top of Apache Spark. It handles cluster management, autoscaling, and supports collaborative notebooks.

#### ✅ Key Features Used:
- Spark DataFrame transformations
- Spark SQL queries
- Visualization with Matplotlib & Seaborn

---

### 🛠️ Code Snippet to Load Data

```python
# Load Ball by Ball data from S3 into Databricks
ball_by_ball_df = spark.read.format("csv") \
    .option("header", "true") \
    .load("s3://ipl-data-analysis-project/Ball_By_Ball.csv")
```
---

### 📊 Analysis & Visualization

Using PySpark and Spark SQL:

* Top run-scorers, wicket-takers
* Powerplay performance
* Match-winning patterns
* Team-wise comparison and more...

Visualized using:

* 📈 Matplotlib
* 📊 Seaborn

---

### 📎 Technologies Used

| Tool                     | Purpose                            |
| ------------------------ | ---------------------------------- |
| **Databricks**           | Cloud-based data processing        |
| **Amazon S3**            | Cloud storage for raw data         |
| **PySpark**              | Data processing and transformation |
| **Spark SQL**            | Querying structured data           |
| **Matplotlib & Seaborn** | Data visualization                 |

---

### 📥 How to Run

1. Upload data to S3
2. Create Databricks notebook
3. Connect to S3 and load data using PySpark
4. Perform transformations and analysis
5. Plot insights using Python libraries

---

### 📌 License

This project is open source and available under the [MIT License](LICENSE).

---

### 👨‍💻 Author

**Bharath S P**
🔗 [LinkedIn](https://www.linkedin.com/in/bharath-s-p-2a7612184)
📫 [bharathsp0805@gmail.com](mailto:bharathsp0805@gmail.com)
