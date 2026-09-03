# Laptop Price Analysis

## 📌 Project Overview

This project analyzes a laptop price dataset to understand how technical specifications and product characteristics are associated with laptop prices.

The analysis focuses on brands, laptop types, RAM, storage, storage types, operating systems, and other specifications to identify pricing patterns and generate useful business insights.

## 🎯 Objectives

- Analyze the relationship between laptop specifications and price.
- Compare average prices across brands and laptop types.
- Investigate whether higher RAM is associated with higher prices.
- Analyze the relationship between storage and price.
- Compare prices across different storage types.
- Examine price differences across operating systems.
- Generate insights that can support pricing, product positioning, customer decisions, and inventory planning.

## 📊 Dataset

- **Dataset:** Uncleaned Laptop Price Dataset
- **Source:** Kaggle – Ehtisham Sadiq
- **Business Domain:** E-commerce / Consumer Electronics
- **Records after cleaning:** 1,268
- **Columns after cleaning:** 14
- **Main Business Metric:** Price

### Main Features

- Company
- Laptop Type
- Screen Size (Inches)
- Display Resolution
- CPU
- RAM (GB)
- Storage (GB)
- Total Storage (GB)
- Storage Type
- GPU
- Operating System
- Weight (kg)
- Price

## 🧹 Data Cleaning & Preparation

The original dataset contained several real-world data quality issues, including:

- Missing values
- Extra spaces in text values
- Mixed text and numerical values
- RAM values containing `GB`
- Weight values containing `kg`
- Storage values containing text and multiple storage configurations
- Inconsistent values and data types

The dataset was cleaned using **Excel and Power Query**.

Main preparation steps included:

- Removing unnecessary columns
- Cleaning extra spaces
- Extracting numerical RAM values
- Extracting numerical weight values
- Separating storage size from storage type
- Creating `Ram_GB`
- Creating `Weight_kg`
- Creating `Storage_GB`
- Creating `Total_Storage_GB`
- Standardizing storage types
- Fixing data types
- Checking errors and missing values
- Creating a `Storage_Group` column

## 🔎 Exploratory Data Analysis

Key statistics after cleaning:

| Metric | Result |
|---|---:|
| Average Price | 59,873 |
| Median Price | 52,055 |
| Average Screen Size | 15.13 inches |
| Average RAM | 8.45 GB |
| Average Total Storage | 612.65 GB |
| Average Weight | 2.07 kg |

### 💻 Price by Company

- **Razer** has the highest average price at approximately **178,283**.
- **Vero** has the lowest average price at approximately **11,585**.
- This indicates that laptop brands target different market price levels.

### 🎮 Price by Laptop Type

- **Workstation:** ~121,255
- **Gaming:** ~92,205
- **Ultrabook:** ~83,113
- **Netbook:** ~34,885

Higher-performance categories such as Gaming and Workstation generally have higher average prices.

### 🧠 RAM vs. Price

A clear positive relationship was observed between RAM and price:

| RAM | Average Price |
|---|---:|
| 8 GB | ~63,075 |
| 16 GB | ~103,378 |
| 32 GB | ~181,850 |

This suggests that RAM is an important factor associated with laptop price.

### 💾 Storage vs. Price

Storage capacity does not always have a direct relationship with price.

The **Very High** storage group had an average price of approximately **82,964**, while the **High** group averaged approximately **43,573**.

This indicates that storage capacity alone cannot explain laptop pricing.

### ⚙️ Storage Type vs. Price

- **SSD + Hybrid:** ~159,574
- **Flash Storage + HDD:** ~106,188
- **SSD + HDD:** ~86,253
- **Flash Storage:** ~27,430

Overall, SSD and combined storage configurations tend to appear in higher-priced laptops.

### 🪟 Operating System vs. Price

- **Windows 7:** ~89,865
- **macOS:** ~83,341
- **Android:** ~29,251
- **Chrome OS:** ~29,495

Different operating systems appear across different laptop price ranges.

## 💡 Business Insights

The analysis can support:

- **Pricing decisions:** Understand how specifications are associated with price.
- **Product positioning:** Identify budget, mid-range, and premium segments.
- **Customer decision-making:** Compare laptops based on specifications and price.
- **Inventory planning:** Identify higher-value product categories and specifications.
- **Market comparison:** Compare brands based on average prices and specifications.
- **Business strategy:** Understand which product features may be associated with higher prices.

## 🛠️ Tools Used

- **Microsoft Excel**
- **Power Query**
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

## 📁 Project Structure

```text
laptop-price-analysis/
│
├── README.md
├── data/
│   └── dataset files
│
├── notebooks/
│   └── analysis notebooks
│
└── images/
    └── analysis screenshots
```

## ⚠️ Limitations

Some unusual observations may remain, including very high laptop prices, unusual weights, or rare storage configurations. These values were not automatically removed because they may represent real products and were considered during the analysis.

## 👤 Author

**Mahmoud Khaled**

Computer and Data Science Student  
Alexandria University, Egypt

Interested in **Data Science, Data Analysis, and Machine Learning**.

---

⭐ If you find this project useful, feel free to explore the repository.
