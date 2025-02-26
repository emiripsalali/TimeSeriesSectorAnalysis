# TimeSeriesSectorAnalysis
A time series classification project analyzing stock sector similarities using machine learning. Features data collection, preprocessing, feature engineering, and model development with Python.


# 📊 Stock Sector Classification Using Time Series

## 📌 Project Overview
This project is part of the **AI Specialization Program - Data-Intensive Applications Module** and focuses on **time series classification for stock sector similarity analysis**. The goal is to analyze the historical behavior of stocks from different sectors and classify them based on their sectoral similarity. The insights derived from this model can be useful for investment strategy development.

## 🎯 Objectives
- Collect stock price data from **Yahoo Finance** and sectoral information via **web scraping**.
- Preprocess and clean stock price data for analysis.
- Extract relevant time-series features using **tsfresh**.
- Implement **machine learning models** to classify stocks into their respective sectors.
- Evaluate model performance using classification metrics.
- Provide sectoral similarity insights for investment strategies.

## 🛠 Technologies & Tools
- **Python** (Main programming language)
- **Jupyter Notebook** (Main development environment)
- **Libraries**: `yfinance`, `BeautifulSoup`, `requests`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `tsfresh`, `XGBoost`, `CatBoost`
- **Data Sources**: Yahoo Finance API, StockAnalysis web scraping
- **Machine Learning Models**: Random Forest, Gradient Boosting, XGBoost

## 📂 Project Structure
```
├── data/                          # Data storage directory
│   ├── stock_sectors/             # Raw scraped stock sector data
│   ├── features/                  # Extracted and processed feature data
│   ├── train_test_split_data.pkl   # Preprocessed training/testing dataset
├── notebooks/                     # Jupyter notebooks for analysis
│   ├── YZUP_VYU_Emir_Can_IPSALALI.ipynb  # Main project notebook
├── scripts/                       # Python scripts for automation
├── README.md                      # Project documentation
```

## 🔄 Workflow
### 1️⃣ Data Collection
- **Web Scraping**: Extract sector & industry names using `BeautifulSoup`.
- **Stock Data Retrieval**: Download historical stock price data from `yfinance`.

### 2️⃣ Data Preprocessing
- Handle missing values via **forward/backward filling**.
- Normalize stock prices using **log transformation**.
- Convert categorical sector data using **one-hot encoding**.

### 3️⃣ Feature Engineering
- Extract statistical time-series features using `tsfresh`.
- Apply **feature selection** using RFE & Lasso.

### 4️⃣ Model Development
- Train multiple classification models:
  - Random Forest 🌲
  - Gradient Boosting 🚀
  - XGBoost ⚡
- Evaluate models using **accuracy, F1-score, and ROC-AUC**.

### 5️⃣ Sector Similarity Analysis
- Use trained models to **predict sector affiliations** of stocks.
- Generate sector **similarity matrices** for investment strategies.

## 📊 Results & Insights
- Stocks were successfully classified into **Financials, Healthcare, and Technology** sectors.
- The best-performing model was **XGBoost** with the highest classification accuracy.
- The project demonstrated how **machine learning** can be applied in **sector-based investment analysis**.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/emiripsalali/TimeSeriesSectorAnalysis.git
   cd TimeSeriesSectorAnalysis
   ```
2. Open the Jupyter Notebook:
   ```bash
   jupyter notebook notebooks/YZUP_VYU_Emir_Can_IPSALALI.ipynb
   ```

## 📌 Future Improvements
- Add **more sectors** for classification.
- Integrate **deep learning models** (LSTMs) for time-series analysis.
- Incorporate **macro-economic factors** for enhanced prediction.

## 📬 Contact
**👤 Emir Can İpsalalı**  
📧 eipsalal@gmail.com  
🌍 [LinkedIn](https://www.linkedin.com/in/emircanipsalali/)
