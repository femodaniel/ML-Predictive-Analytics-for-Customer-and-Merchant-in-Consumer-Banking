# ML-Predictive-Analytics-for-Customer-and-Merchant-in-Consumer-Banking
Machine Learning Project
# Nigerian Banking Analytics & ML Platform
### End-to-End Predictive Analytics for Consumer Banking

A comprehensive data analytics and machine learning platform designed for Nigerian consumer banking, featuring synthetic data generation, interactive dashboards, and predictive models for risk management and customer insights.

---

## 🎯 Project Overview

This project demonstrates enterprise-grade banking analytics and ML capabilities with relevant dataset. It includes:

- **Relevant Dataset**: Data (scalable to 10M+ records)
- **Business Intelligence**: Professional dashboards in Tableau & Power BI
- **Machine Learning**: Predictive models for credit risk, fraud detection, and customer behavior
- **Production-Ready**: Optimized for MSSQL, batch processing, and enterprise deployment

---

## 📊 Dataset Structure

### Tables (6)
1. **CustomerBio** - Customer demographics (BVN, NIN, KYC data)
2. **AccountByScheme** - All account types (Savings, Current, Overdraft, Loans)
3. **FT_Web** - Web channel transactions
4. **FT_USSD** - USSD channel transactions (*dominant in Nigeria*)
5. **FT_ATM** - ATM transactions
6. **FT_POS** - Point-of-Sale transactions

### Key Features
- **Nigerian Context**: Real FCMB branch codes, Nigerian names, USSD dominance
- **Realistic Relationships**: Star schema with proper foreign keys
- **Account Rules**: 100% customers have ≥1 Overdraft account
- **Scalability**: Tested from 67K to 10M records

---

## 🛠️ Tech Stack

### Data Generation & Storage
- **Python 3.13**: pandas, numpy, faker, pyodbc
- **MSSQL Server 2022**: Local instance with optimized schema
- **Batch Processing**: 50K-record batches with memory management

### Business Intelligence
- **Tableau**: LOD expressions, interactive dashboards
- **Power BI**: DAX measures, Power Query transformations

### Machine Learning (Planned)
- **scikit-learn**: Classification & clustering models
- **XGBoost/LightGBM**: Gradient boosting for credit risk
- **TensorFlow**: Deep learning for fraud detection
- **Prophet**: Time series forecasting

---

## 📈 Analytics Dashboards

### 1. Customer Overview Dashboard
- Customer segmentation (Retail/Premium/Corporate)
- Geographic distribution across Nigeria
- Age & gender demographics
- Registration trends

### 2. Transaction Analysis Dashboard
- Channel performance (Web/USSD/ATM/POS)
- Transaction trends & seasonality
- Top merchants & categories
- Success rate analysis
- Hourly heatmaps

### 3. Loan Portfolio Dashboard
- Loan distribution by type
- Delinquency analysis (30/60/90+ days)
- Credit score distribution
- Portfolio at Risk (PAR) metrics
- Non-Performing Loan (NPL) ratio
- Vintage analysis

---

## 🤖 Machine Learning Models

### Credit Risk Modeling
- **Objective**: Predict loan default probability
- **Features**: Credit score, days overdue, utilization, transaction patterns
- **Models**: Logistic Regression, Random Forest, XGBoost
- **Metrics**: AUC-ROC, Precision, Recall, F1-Score

### Fraud Detection
- **Objective**: Identify suspicious transactions
- **Features**: Transaction amount, time, channel, location, frequency
- **Models**: Isolation Forest, Autoencoder, GBM
- **Metrics**: Precision@K, False Positive Rate

### Customer Segmentation
- **Objective**: Group customers by behavior
- **Features**: Transaction patterns, account types, channel preference
- **Models**: K-Means, DBSCAN, Hierarchical Clustering
- **Metrics**: Silhouette Score, Davies-Bouldin Index

### Churn Prediction
- **Objective**: Identify customers likely to become dormant
- **Features**: Transaction frequency, recency, account age
- **Models**: Survival Analysis, Classification models
- **Metrics**: Lift, Precision, Recall

### Cross-Sell Recommendation
- **Objective**: Recommend next product for customers
- **Features**: Current products, demographics, transaction behavior
- **Models**: Collaborative Filtering, Association Rules
- **Metrics**: Precision@K, Hit Rate

---

## 🚀 Getting Started

### Prerequisites
```bash
Python 3.13+
SQL Server 2022
Power BI Desktop
Tableau Desktop
```

### Installation
```bash
# Clone repository
git clone https://github.com/yourusername/nigerian-banking-analytics-ml.git
cd nigerian-banking-analytics-ml

# Install dependencies
pip install -r requirements.txt

# Configure database connection
# Update connection string in config.py
```

### Data Generation
```bash
# Generate 67K records (demo)
python generate_banking_data.py --records 67000

# Generate 10M records (production)
python generate_banking_data_optimized.py --records 10000000 --batch-size 50000
```

---

## 📁 Project Structure
```
nigerian-banking-analytics-ml/
├── data_generation/
│   ├── load_banking_data.py            # Demo version (67K records)
│   ├── load_banking_data_optimized.py  # Production version (10M records)
│   ├── config.py                          # Database configuration
│   └── reference_data.py                  
├── dashboards/
│   ├── tableau/
│   │   └── banking_analytics.twbx
│   └── powerbi/
│       └── banking_analytics.pbix
├── ml_models/
│   ├── credit_risk_model.py
│   ├── fraud_detection_model.py
│   ├── customer_segmentation.py
│   └── churn_prediction.py
├── sql_scripts/
│   ├── create_tables.sql
│   ├── create_indexes.sql
│   └── sample_queries.sql
├── notebooks/
│   ├── 01_exploratory_data_analysis.ipynb
│   ├── 02_credit_risk_modeling.ipynb
│   ├── 03_fraud_detection.ipynb
│   └── 04_customer_segmentation.ipynb
├── docs/
│   ├── tableau_guide.md
│   ├── powerbi_guide.md
│   └── ml_methodology.md
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 📊 Sample Insights

### Customer Demographics
- customers inspired by relevant datasets


### Transaction Patterns
- **USSD dominates**: 50% of all transactions (3M out of 6M)
- Web/ATM/POS each ~17% of transactions
- Average transaction: ₦85,000
- Peak hours: 10 AM - 2 PM, 5 PM - 7 PM

### Loan Portfolio Health
- Total loans: 2,000+ facilities
- Average credit score: 680
- Portfolio at Risk (>30 days): 8.5%
- NPL Ratio (>90 days): 3.2%

---

## 🎓 Learning Outcomes

This project demonstrates:
- ✅ Synthetic data generation for privacy-preserving analytics
- ✅ Star schema design for banking data warehouses
- ✅ Business intelligence dashboard development
- ✅ DAX and LOD expression mastery
- ✅ End-to-end ML pipeline (data → model → deployment)
- ✅ Nigerian banking domain knowledge
- ✅ Scalable data processing (67K → 10M records)

---

## 🔒 Data Privacy

**No real customer dataset is used or shared in this project.**



---

## 🤝 Contributing

This is a portfolio/demonstration project. Contributions welcome for:
- Additional ML models
- Dashboard enhancements
- Fintechs
- Nigerian Consumer banking domain improvements
- US Consumer banking domain improvements
- Performance optimizations

---

## 📄 License

MIT License - See LICENSE file for details

---

## 👤 Author

**Daniel Femi** (Your Name)
- LinkedIn: [https://www.linkedin.com/in/femidaniel]
- Email: [femodaniel@gmail.com]

---

## 🙏 Acknowledgments

- Synthetic datasets inspired by banking best practices
- Dashboard designs follow industry standards

---

## 📚 Documentation

Detailed guides available in `/docs`:
- [Tableau Learning Guide](docs/tableau_guide.md) - Newbie to Professional
- [Power BI Learning Guide](docs/powerbi_guide.md) - Newbie to Professional
- [ML Methodology](docs/ml_methodology.md) - Model development approach

---

## 🎯 Roadmap

- [x] Phase 1: Data wrangling and extraction and loading
- [x] Phase 2: Tableau & Power BI dashboards
- [ ] Phase 3: Optimized 10M record generation
- [ ] Phase 4: Credit risk ML model
- [ ] Phase 5: Fraud detection model
- [ ] Phase 6: Customer segmentation
- [ ] Phase 7: Real-time scoring API
- [ ] Phase 8: Model deployment & monitoring

---

**⭐ Star this repo if you find it useful!**
