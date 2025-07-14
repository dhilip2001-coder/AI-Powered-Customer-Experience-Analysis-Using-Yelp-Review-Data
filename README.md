# 📊 AI-Powered Customer Experience Analysis Using Yelp Review Data

This project demonstrates an end-to-end data pipeline and analytics workflow on Yelp reviews. Starting with a large raw JSON file (~5 GB), the data was cleaned and partitioned using Python, stored in AWS S3, and processed in Snowflake. Leveraging AI techniques like natural language processing (NLP), sentiment analysis was performed on review texts to extract customer experience insights, enabling data-driven decisions based on real user feedback.

---

## 🎯 Project Objective

This project uses NLP, Large Language Models (LLMs), and data analytics to extract actionable insights from 500,000+ unstructured Yelp reviews. The goal was to help businesses identify recurring customer issues, improve service strategies, and optimize customer experience across different geographies.

---

## 🌎 About Company

Yelp is a popular online platform that connects people with local businesses such as restaurants, shops, and services through user-generated reviews and ratings. Founded in 2004, Yelp provides a large dataset of customer feedback, making it a valuable resource for analyzing consumer sentiment, business performance, and market trends. Its publicly available data has been widely used in research and data analytics projects focused on natural language processing and sentiment analysis.

## 🛠️ Tools & Technologies Used

- **Python (Jupyter Notebook)** – Data preprocessing and file partitioning  
- **Amazon S3** – Cloud storage for raw and processed data  
- **Snowflake** – Cloud data warehouse for data transformation and analysis using SQL  
- **SQL** – Sentiment analysis logic, data querying, and aggregation  
- **Tableau** – Data visualization (In progress)
- **Libraries** - Pandas, NLTK, Snowflake Connector, OpenAI API (GPT-4) 

---

## 🧩 Problem Statement

Yelp hosts millions of unstructured user reviews that hold valuable feedback on customer experience,but turning this raw text into actionable insights at scale is a challenge. This project addresses that by:
- Ingesting and partitioning a 5GB JSON dataset of Yelp reviews
- Converting unstructured data into a queryable tabular format using Snowflake
- Applying NLP and LLMs to extract sentiment, themes, and emotional tone
- Surfacing customer pain points and feedback trends across locations and categories
- Enabling strategic decision-making through AI-enhanced dashboards in Tableau

---

## 🚀 Features

✅ Automated Pipeline: Extracts and loads raw Yelp reviews from Amazon S3 → transforms to Snowflake for scalable querying.
✅ Sentiment Analysis: Uses NLTK’s VADER to analyze polarity and categorize reviews.
✅ LLM-Based Insight Generation: GPT-4 is prompted to extract pain points, common service complaints, and emotional themes from user reviews.
✅ Dashboards: Tableau visualizations displaying trends by city, service category, and sentiment rating.

---

## 🔐 API Keys & Configuration

To use GPT-4 or Snowflake:
  1. Create a .env file:
     for example : OPENAI_API_KEY=your_key
                   SNOWFLAKE_USER=your_user
                   SNOWFLAKE_PASSWORD=your_password
  2. Install dependencies:
     for example : pip install -r requirements.txt

...

## 🔄 Workflow Overview

1. **Data Ingestion & Partitioning**  
   - Loaded a 5GB Yelp review JSON dataset using Python  
   - Partitioned the raw data into 10 smaller files for easier handling and storage

2. **Cloud Upload & Warehouse Integration**  
   - Uploaded partitioned files to an Amazon S3 bucket
   - Configured an external stage and file format in Snowflake to connect with S3
   - Loaded and parsed JSON data into Snowflake tables using COPY INTO with semi-structured handling

3. **Data Transformation & Preprocessing**  
   - Flattened nested JSON structures using SQL and Python (Pandas)  
   - Cleaned and normalized review data for downstream sentiment and language modeling

4. **Sentiment Analysis & LLM Insight Generation**  
   - Performed rule-based sentiment scoring using NLP techniques (VADER, NLTK) 
   - Integrated LLMs (GPT-4) via API to extract themes, emotions, and summarize customer pain points using prompt engineering  
   - Applied AI-driven text classification to detect high-impact review segments

5. **Insight Extraction & Visualization**  
   - Identified recurring feedback patterns by location, business category, and sentiment score 
   - Visualized trends using Tableau dashboards to surface key satisfaction drivers and areas for service improvement

---

## 📊 Key Insights Discovered

   - Frequent delays in service delivery were a major issue in metro cities.
   - Customers value employee friendliness more than product variety.
   - 1-star reviews frequently mention inconsistent pricing and long wait times.

---

### 📬 Contact
If you have any questions or suggestions, feel free to reach out:

Name: Dhilip Kumar Thallem

Email: [dhilipkumarthallem@gmail.com]

LinkedIn: [https://www.linkedin.com/in/dhilip-kumar-thallem ]

