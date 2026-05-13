
##  Project Overview

This project performs a comprehensive analysis of customer behavior using a real-world e-commerce consumer behavior dataset. The goal is to help businesses understand **who their customers are**, **how they shop**, and **what can be done to improve retention and revenue**.

The project covers:
- Exploratory data analysis (EDA)
- Feature engineering
- Customer segmentation via clustering
- Churn risk prediction
- Business insight generation

The final output includes an interactive Jupyter Notebook and an exported HTML dashboard.

---

## Objectives

- Understand customer purchasing patterns and preferences
- Analyze loyalty levels and satisfaction trends
- Identify customers at high risk of churning
- Segment customers into meaningful behavioral groups
- Discover monthly purchasing and seasonal trends
- Provide data-driven business recommendations

---

## Dataset

The dataset contains approximately **1,000 customer transaction records** with the following attributes:

| Category | Attributes |
|---|---|
| **Demographics** | Customer ID, Age, Gender, Income Level, Education Level |
| **Purchase Info** | Purchase Amount, Frequency of Purchase, Purchase Category |
| **Behavior** | Brand Loyalty, Purchase Intent, Discount Usage, Social Media Influence |
| **Satisfaction** | Product Ratings, Customer Satisfaction |
| **Technical** | Device Used, Payment Method, Shipping Preference, Time of Purchase |

**File:** `data/Ecommerce_Consumer_Behavior_Analysis_Data.csv`

---

## Technologies Used

| Technology | Version | Purpose |
|---|---|---|
| Python | 3.8+ | Core programming language |
| Pandas | Latest | Data loading, manipulation, and analysis |
| NumPy | Latest | Numerical computations |
| Matplotlib | Latest | Custom data visualizations |
| Seaborn | Latest | Statistical and heatmap visualizations |
| Scikit-learn | Latest | K-Means clustering and preprocessing |
| Jupyter Notebook | Latest | Interactive development environment |

---

## ⚙️ Project Workflow

```
Raw Data → Data Cleaning → Feature Engineering → EDA → ML Clustering → Insights & Recommendations
```

### 1️⃣ Data Loading & Exploration
- Loaded the dataset using Pandas
- Explored structure, data types, and sample records
- Generated summary statistics for numeric and categorical features

### 2️⃣ Data Cleaning
- Detected and handled missing values
- Removed or imputed null entries using appropriate strategies
- Ensured data type consistency across all columns

### 3️⃣ Feature Engineering
Created three new features to enrich the analysis:

| Feature | Description |
|---|---|
| `loyalty_score` | Composite score derived from Brand Loyalty, Customer Satisfaction, and Product Rating |
| `purchase_month` | Extracted month from transaction timestamp for trend analysis |
| `churn_risk` | Binary label (High / Low) based on satisfaction and purchase frequency thresholds |

### 4️⃣ Exploratory Data Analysis (EDA)
- Analyzed distributions for age, income, and purchase amount
- Examined category-wise and device-wise purchasing behavior
- Investigated correlation between satisfaction, loyalty, and churn

### 5️⃣ Customer Segmentation (K-Means Clustering)
Applied K-Means clustering to group customers based on:
- Purchase Amount
- Frequency of Purchase
- Customer Satisfaction
- Brand Loyalty

### 6️⃣ Data Visualization
Generated a full suite of charts and plots for storytelling and business communication.

---

## Key Features

### ✅ Loyalty Score Calculation
A composite loyalty metric calculated from:
- Brand Loyalty (weighted)
- Customer Satisfaction (weighted)
- Product Rating (weighted)

### ✅ Churn Risk Prediction
Customers labeled as **High Risk** or **Low Risk** based on:
- Low satisfaction scores
- Infrequent purchasing behavior

### ✅ Customer Segmentation
Customers grouped into distinct behavioral clusters using unsupervised machine learning (K-Means), enabling personalized marketing strategies per segment.

### ✅ Monthly Trend Analysis
Month-over-month analysis of purchase volume and revenue to identify seasonal patterns and peak periods.

---

## 📊 Visualizations

The project includes the following charts and plots:

| # | Chart | Purpose |
|---|---|---|
| 1 | Customer Segment Distribution | Shows the spread of customers across K-Means clusters |
| 2 | Purchase Category Analysis | Identifies the most popular product categories |
| 3 | Monthly Purchase Trend | Tracks purchase volume over time |
| 4 | Churn Risk Count Plot | Visualizes High vs Low risk customer distribution |
| 5 | Loyalty Score Distribution | Examines the spread of customer loyalty |
| 6 | Customer Behavioral Insights | Heatmaps and correlation plots for behavioral features |

---

## Machine Learning

### K-Means Clustering

**Algorithm:** K-Means (Unsupervised Learning)

**Purpose:** Group customers into segments based on behavioral similarity.

**Features Used:**

```
- Purchase Amount
- Frequency of Purchase
- Customer Satisfaction
- Brand Loyalty
```

**Process:**
1. Standardized features using `StandardScaler`
2. Determined optimal `k` using the Elbow Method
3. Fitted K-Means and assigned cluster labels
4. Visualized and interpreted each customer segment

---

## 📈 Results & Insights

- ✅ Identified **loyal, high-value customers** for reward and retention programs
- ✅ Detected **high churn-risk customers** requiring immediate intervention
- ✅ Uncovered **seasonal trends** with notable purchase spikes in specific months
- ✅ Found **device usage patterns** — mobile shoppers represent a significant portion
- ✅ Discovered **social media's influence** on purchase decisions across segments
- ✅ Mapped **satisfaction vs loyalty** to reveal hidden at-risk segments

---

## 💡 Business Recommendations

Based on the analysis results, the following strategies are recommended:

1. **Personalized Campaigns** — Target high-value customer segments with exclusive offers and loyalty rewards.
2. **Churn Prevention Programs** — Reach out proactively to high-risk customers with discounts and re-engagement emails.
3. **Category-Specific Advertising** — Increase spend on ads for top-performing product categories.
4. **Loyalty Reward System** — Introduce a tiered rewards program for frequent and high-spending customers.
5. **Mobile Experience Optimization** — Improve the mobile shopping experience since a large segment shops via mobile devices.
6. **Social Media Strategy** — Leverage the influence of social media by creating targeted campaigns for socially-influenced buyers.

---

## 📁 Project Structure

```
Customer-Behavior-Analysis/
│
├── data/
│   └── Ecommerce_Consumer_Behavior_Analysis_Data.csv   # Raw dataset
│
├── notebooks/
│   └── customer_behavior_analysis.ipynb                # Main Jupyter Notebook
│                                       
├── README.md                                           # Project documentation
└── requirements.txt                                    # Python dependencies
```

---

##  Getting Started

### Prerequisites

Make sure you have **Python 3.8+** and **pip** installed on your machine.

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/customer-behavior-analysis.git
cd customer-behavior-analysis
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 3️⃣ Launch Jupyter Notebook

```bash
jupyter notebook
```

Then open:

```
notebooks/customer_behavior_analysis.ipynb
```

## 📄 `requirements.txt`

```
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

##  License

This project is created for **educational and portfolio purposes only**. The dataset used is publicly available and intended for learning and demonstration.

---

##  Author

**P Reddy Nohith**

- GitHub: https://github.com/ReddyNohith
- LinkedIn: https://www.linkedin.com/in/reddynohith/
- Email: mailto.nohith@gmail.com

---

>  If you found this project helpful, please consider starring the repository!
