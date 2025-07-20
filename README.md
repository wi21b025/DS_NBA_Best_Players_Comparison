
# 🏀 NBA Best Players Comparison 

This project aims to finally answer the question:  
**Who is the best at their best — Michael Jordan, Kobe Bryant, or LeBron James?**

It brings together NBA data from CSV files, web scraping, and live API calls. The pipeline applies ETL (Extract, Transform, Load) concepts using **Apache Kafka** for streaming, **PySpark** for processing, and **MongoDB** for storage. The final notebook delivers a focused, data-driven comparison of these three players during their peak years.

---

## 🧱 Project Architecture

![Project Architecture](NBA%20Data%20Notebook/images/Architecture.jpg)

This architecture shows the full data pipeline:

- Data is collected from Kaggle, the NBA API, and web scraping tools.
- Kafka handles streaming of real-time API data.
- PySpark processes data and MongoDB stores the structured output.
- Final analysis and visualization are done using Pandas, Seaborn, NumPy, and Matplotlib inside Jupyter Notebook

---

## 📁 Project Structure

```
CSV Data/
├── CSV-Script.ipynb                    

WebScraper/
├── NBA WEB Producer.ipynb                
├── NBA WEB Consumer.ipynb                
├── NBA-Data-WebScraping.ipynb
├── Data/                                 

Kafka API PubSub/
├── NBA API Producer.ipynb                
├── API Data Consumer with Spark.ipynb    

NBA Data Notebook/
├── NBA Data Notebook.ipynb               – merges all sources and performs final analysis
├── images/                               
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
Environment      | Conda, Jupyter Notebooks
```
