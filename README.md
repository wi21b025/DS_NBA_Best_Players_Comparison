
# 🏀 NBA Best Players Comparison – Data Science Project

This project aims to finally answer the question:  
**Who is the best at their best — Michael Jordan, Kobe Bryant, or LeBron James?**

It brings together NBA data from CSV files, web scraping, and live API calls. The pipeline applies ETL (Extract, Transform, Load) concepts using **Apache Kafka** for streaming, **PySpark** for processing, and **MongoDB** for storage. The final notebook delivers a focused, data-driven comparison of these three players during their peak years.

---

## ✅ Key Features

- Multisource data ingestion: static datasets, scraped stats, and API feeds
- Kafka-based data streaming and PySpark transformation
- Cleaned and unified dataset loaded into MongoDB
- Visual analysis comparing peak performance across multiple metrics
- Fully implemented in Jupyter notebooks for transparency and reproducibility

---

## 📁 Project Structure

```
CSV Data/
├── CSV-Script.ipynb          – loads and cleans historical data

WebScraper/
├── NBA WEB Producer.ipynb    – scrapes player stats
├── NBA WEB Consumer.ipynb    – processes scraped data
├── NBA-Data-WebScraping.ipynb
├── Data/                     – yearly scraped CSVs

Kafka API PubSub/
├── NBA API Producer.ipynb    – pulls and sends NBA API data to Kafka
├── API Data Consumer with Spark.ipynb – processes streamed data using PySpark

NBA Data Notebook/
├── NBA Data Notebook.ipynb   – merges all sources and performs final analysis
├── images/                   – architecture and data flow diagrams
```

---

## 🧰 Tech Stack

```
Component        | Technology
-----------------|-------------------------------------
Language         | Python 3.10+
Streaming        | Apache Kafka
Processing       | PySpark, Pandas
Storage          | MongoDB
Scraping         | BeautifulSoup, Requests
API              | NBA Stats API
Data             | CSV (Kaggle, Basketball Reference)
Visualization    | Matplotlib, Seaborn
Environment      | Jupyter Notebooks
```
