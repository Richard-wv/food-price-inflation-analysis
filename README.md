# Food Price Inflation Analysis

## Project Overview

A comprehensive data analysis project developed for a data analytics hackathon, focusing on global food price inflation trends using World Bank's Real-Time Food Price Monitoring data.

## Hackathon Achievement

This project demonstrates advanced ETL (Extract, Transform, Load) capabilities through:
- **Data Integration**: Successfully merged complex datasets with 4,773+ duplicate key resolution
- **Feature Engineering**: Created 9 analytical features including time-series and categorical variables
- **Data Quality**: Implemented 6-point validation system ensuring zero data quality issues
- **Pipeline Automation**: Built reusable, production-ready data processing workflow

## Dataset & Structure

**Source**: Global Food Price Inflation 2024 (Kaggle)
- Original datasets: Country-level + Item-level food price data
- Final output: Clean, analysis-ready dataset with 18 optimized columns

```
data/
├── Original datasets (2 files)
├── Cleaned datasets (4 intermediate files)  
└── food_price_feature_engineered_clean.csv (final)
```

## Technical Implementation

**Core ETL Pipeline** ([`jupyter_notebooks/etl.ipynb`](jupyter_notebooks/etl.ipynb)):
1. **Data Cleaning**: Standardized columns, parsed dates, coerced numeric fields
2. **Smart Merging**: Multi-level join strategy with duplicate resolution
3. **Feature Engineering**: Time, price, and categorical feature creation
4. **Validation**: Comprehensive quality checks and automated cleanup

## Key Technical Features

✅ **Robust Error Handling**: Resolved 4,773 duplicate keys before merging  
✅ **Feature Engineering**: 9 analytical variables (time, price trends, categories)  
✅ **Data Validation**: 6-point quality system with automated cleanup  
✅ **Production Ready**: Reusable functions and comprehensive documentation  

## Technologies

- **Python 3.12+** | **Pandas** | **NumPy** | **Jupyter Notebooks**

## Results

**Final Dataset**: 18 columns, zero quality issues, ready for analysis and visualization
- Successfully processed complex real-world data with missing values and duplicates
- Created scalable ETL pipeline suitable for production environments
- Demonstrated advanced data engineering skills through comprehensive validation

