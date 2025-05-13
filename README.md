# 🎧 Spotify Data Analysis on AWS
 
**Technologies**: AWS Glue, Amazon S3, AWS Athena, Amazon QuickSight

---

## 📝 Project Overview

This project implements a complete **ETL pipeline on AWS** to analyze Spotify data, including albums, artists, and tracks. The dataset consists of:

- **438,973 albums**
- **37,012 artists**
- **438,938 tracks**

The goal is to uncover musical trends, identify top-performing artists, and explore the impact of specific albums using serverless and scalable AWS services.

---

## ⚙️ ETL Pipeline Architecture

### 1. **Extract & Load**
- The raw Spotify dataset (CSV/JSON format) was uploaded to an **Amazon S3 bucket**.

### 2. **Transform**
- Data was cleaned, formatted, and transformed using **AWS Glue** jobs (PySpark).
- Null values were handled, and relevant fields were cast to proper data types (e.g., release dates, popularity scores).

### 3. **Query & Analysis**
- Transformed data was cataloged and queried using **AWS Athena** with SQL.
- Key queries analyzed artist popularity, track counts, and genre trends.

### 4. **Visualization**
- Results were visualized using **Amazon QuickSight**, enabling interactive dashboards and trend exploration.

---

## 📊 Key Findings

- 🎤 **Most Popular Artist**: Taylor Swift — **95.8 million followers**
- 🔥 Analyzed the impact of **Bad Bunny’s album** _"Nadie Sabe Lo Que Va a Pasar Mañana"_, observing spikes in track popularity and streaming performance.
- Genre and album release trends revealed seasonal popularity spikes and emerging genres.

---

## 🚀 Technologies Used

| Tool            | Purpose                             |
|-----------------|-------------------------------------|
| **Amazon S3**   | Data storage                        |
| **AWS Glue**    | Data cleaning and transformation    |
| **AWS Athena**  | Serverless SQL querying             |
| **QuickSight**  | Interactive dashboards and visuals  |

---

## 📌 Future Improvements

- Incorporate **real-time streaming data** with Kinesis.
- Add sentiment analysis from **Spotify lyrics** (via external APIs).
- Deploy using **AWS Step Functions** for orchestrated ETL flow.

---
