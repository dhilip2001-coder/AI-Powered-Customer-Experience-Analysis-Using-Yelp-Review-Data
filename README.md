# 📊 End-to-End Data Analytics and Sentiment Analysis on Yelp Reviews

This project demonstrates an end-to-end data pipeline and analytics workflow on Yelp reviews. Starting with a large raw JSON file (~5 GB), the data was cleaned and partitioned using Python, stored in AWS S3, and then processed using Snowflake for advanced SQL-based sentiment and data analysis.

---

## 🎯 Project Objective

To analyze Yelp review data by building a scalable and cloud-based pipeline that enables efficient sentiment classification and business insights using structured queries on Snowflake.

---

## 🛠️ Tools & Technologies Used

- **Python (Jupyter Notebook)** – Data preprocessing and file partitioning  
- **Amazon S3** – Cloud storage for raw and processed data  
- **Snowflake** – Cloud data warehouse for data transformation and analysis using SQL  
- **SQL** – Sentiment analysis logic, data querying, and aggregation  
- **Power BI / Tableau** – Data visualization (In progress) 

---

## 🧩 Problem Statement

Yelp provides a massive volume of user-generated content. However, deriving actionable insights from such a large and unstructured dataset requires a robust processing pipeline. This project tackles the challenge by:
- Breaking down a 5GB JSON dataset
- Converting it into a structured tabular format
- Performing sentiment analysis using SQL logic on Snowflake
- Uncovering review trends and customer sentiments

---

## 🔄 Workflow Overview

1. **Data Partitioning**  
   - Loaded a large 5GB Yelp review JSON file using Python  
   - Split the file into 10 smaller, manageable chunks

2. **Data Upload**  
   - Uploaded the processed files into an **Amazon S3 Bucket**

3. **Cloud Data Warehouse Setup**  
   - Connected S3 bucket to **Snowflake** using external stage and file format  
   - Loaded the JSON files into a **Snowflake table** using the COPY INTO command

4. **Data Transformation & Sentiment Analysis**  
   - Parsed JSON fields and flattened nested structures using SQL  
   - Implemented sentiment analysis logic using keywords and text patterns in SQL  
   - Performed aggregations and trend analysis

5. **Insight Extraction**  
   - Identified common patterns in reviews by business category, date, and sentiment  
   - Highlighted key drivers of negative/positive feedback

### 📬 Contact
If you have any questions or suggestions, feel free to reach out:

Name: Dhilip Kumar Thallem

Email: [dhilipkumarthallem@gmail.com]

LinkedIn: [https://www.linkedin.com/in/dhilip-kumar-thallem ]

