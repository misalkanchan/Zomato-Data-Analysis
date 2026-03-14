# 🍽️ Zomato Data Analysis

Exploratory Data Analysis (EDA) of a Zomato restaurants dataset to uncover trends in restaurant types, ratings, online ordering behaviour, and customer spending patterns.

---

## 📌 Project Overview

This project performs end-to-end exploratory data analysis on a Zomato dataset containing 148 restaurants. The goal is to extract meaningful insights about restaurant preferences, ordering modes, pricing, and ratings using Python and static visualizations.

---

## 📂 Project Structure

```
Zomato-Data-Analysis/
│
├── Zomato_Data_Analysis.ipynb    # Main Jupyter Notebook with full EDA
├── Zomato_data.csv               # Dataset used for analysis
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```

---

## 📊 Dataset

**File:** `Zomato_data.csv`  
**Records:** 148 restaurants

| Column | Description |
|---|---|
| `name` | Name of the restaurant |
| `online_order` | Whether online ordering is available (Yes/No) |
| `book_table` | Whether table booking is available (Yes/No) |
| `rate` | Restaurant rating (cleaned to float, e.g. 4.1) |
| `votes` | Number of customer votes |
| `approx_cost(for two people)` | Approximate dining cost for two (in INR) |
| `listed_in(type)` | Category of restaurant (Buffet, Cafes, Dining, Other) |

---

## 🔍 Key Analysis Performed

- **Data Loading & Cleaning** – Loading CSV, cleaning the `rate` column from `"4.1/5"` format to float
- **Restaurant Type Distribution** – Count plot of restaurant categories
- **Votes by Restaurant Type** – Line plot of total votes per category
- **Rating Distribution** – Histogram of restaurant ratings
- **Couple Spending Analysis** – Count plot of approximate cost for two people
- **Online vs Offline Ratings** – Box plot comparing ratings by order mode
- **Heatmap Analysis** – Pivot table heatmap of restaurant type vs online order availability

---

## 💡 Key Insights

- **Dining** restaurants are the most common category in the dataset.
- **Dining** restaurants have also received the maximum total votes from customers.
- **Majority** of restaurants received ratings between **3.5 and 4.0**.
- Most couples prefer restaurants with an approximate cost of **₹300 for two**.
- Restaurants that accept **online orders** tend to receive **higher ratings** than those that don't.
- The heatmap reveals that **Dining restaurants** predominantly prefer **offline ordering**, while **Cafes** lean toward online ordering.

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas** – Data manipulation and cleaning
- **NumPy** – Numerical operations
- **Matplotlib** – Static visualizations
- **Seaborn** – Statistical plots and heatmaps
- **Jupyter Notebook** – Development environment

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/Zomato-Data-Analysis.git
cd Zomato-Data-Analysis
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch the notebook
```bash
jupyter notebook Zomato_Data_Analysis.ipynb
```

> **Note:** If running on Google Colab, upload `Zomato_data.csv` to `/content/` and update the file path in the data loading cell accordingly.

---

## 📧 Contact

Feel free to raise an issue or reach out if you have any questions or suggestions!
