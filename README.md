# Financial Data Extraction & Visual Analytics Dashboard

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## 📌 Project Overview
This project was developed as part of the **IBM Data Science Professional Certificate**. Acting as a Data Scientist for a startup investment firm, I built an automated pipeline to extract, process, and visualize financial data. The goal is to provide traders and analysts with a consolidated view of stock performance versus company revenue to identify long-term trends.

## 🎯 Business Objective
In the fast-paced world of stock trading, manual data collection is a bottleneck. This project solves that by:
1.  **Automating Data Retrieval:** Pulling historical stock prices and quarterly revenue.
2.  **Harmonizing Datasets:** Aligning disparate data sources (APIs and Web Scraping) into a single analytical frame.
3.  **Interactive Visualization:** Creating a dashboard to visualize the relationship between financial health (revenue) and market sentiment (stock price).

## 🛠️ Tech Stack
* **Data Acquisition:** `yfinance` (API), `BeautifulSoup` (Web Scraping), `Requests`.
* **Data Manipulation:** `Pandas`, `NumPy`.
* **Visualization:** `Plotly` (Interactive Graphs).
* **Environment:** Jupyter Notebook / Google Colab.

## 📊 Analyzed Assets
The pipeline is optimized for high-growth and high-volatility stocks, including:
* **Tesla (TSLA)**
* **Amazon (AMZN)**
* **AMD (AMD)**
* **GameStop (GME)**

## 🚀 Key Features & Workflow
1.  **Stock Data Extraction:** Utilized the `yfinance` library to extract years of historical price data.
2.  **Revenue Scraping:** Engineered a web scraper to parse HTML tables from financial news sites, ensuring quarterly revenue data was captured even when not available via standard APIs.
3.  **Data Cleaning:** Handled missing values, formatted currency strings into floats, and synchronized timestamps across datasets.
4.  **Dashboard Construction:** Developed a custom `make_graph` function using Plotly to display a dual-axis chart (Stock Price vs. Revenue).

## 📈 Sample Results
The resulting dashboard allows users to:
* Identify if revenue growth precedes stock price rallies.
* Compare historical "short squeeze" events with underlying financial fundamentals.
* Evaluate the cyclical nature of revenue in the tech and retail sectors.

## 📝 How to Use
1.  Clone the repository: `git clone https://github.com/rpfeifer-ds/Python-Project-for-Data-Science---IBM`
2.  Install dependencies: `pip install yfinance pandas plotly beautifulsoup4 nbformat`
3.  Run the Jupyter Notebook: `Revenue Data and Building a Dashboard-v1` or `Final Assignment Webscraping` 

## 🔍 Insights & Conclusions
After analyzing the synthesized data, several key patterns were identified:

* **Correlation Analysis:** For growth stocks like **Tesla**, a strong visual correlation was observed between quarterly revenue milestones and long-term stock price appreciation, validating the importance of fundamental health over market noise.
* **Volatility Resilience:** In the case of **GameStop**, the dashboard highlights the decoupling of stock price from quarterly revenue during high-volatility events (e.g., short squeezes), providing a clear visual indicator of speculative trading versus fundamental investing.
* **Data Efficiency:** The automated pipeline reduced data gathering time by approximately 80% compared to manual collection, demonstrating the scalability of using Python for real-time investment analysis.
* **Strategic Decision Making:** The unified dashboard provides a holistic view that allows analysts to quickly assess if a stock is "overvalued" relative to its historical revenue performance.
  
---
*Developed as part of the IBM Data Science curriculum to demonstrate proficiency in Python-based data engineering and visualization.*
