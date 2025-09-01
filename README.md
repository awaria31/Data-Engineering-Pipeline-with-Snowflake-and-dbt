## Modern ELT Data Pipeline with Airbyte, Snowflake, and dbt

Built an end-to-end ELT pipeline that ingests data with **Airbyte**, loads it into **Snowflake**, and transforms it with **dbt** to create staging views and fact tables for analysis. This project demonstrates modern data engineering practices for data integration and analytics.

## What I Did
- Connected multiple data sources: Google Sheets survey, CSV files, and Snowflake Marketplace datasets.  
- Configured Airbyte to load raw data into Snowflake.  
- Created dbt models to clean and transform data (e.g., survey transformations, valid ticker staging, trading fact table).  
- Analyzed data in Snowflake and Python (`pandas`, `matplotlib`) to calculate profit metrics and build visualizations.  

## Tech Stack
Airbyte · Snowflake · dbt · SQL · Python  

## 📂 Repo Structure
```p4-elt-pipeline/
├─ p4.ipynb        # SQL + Python analysis
├─ report.pdf      # Final report with screenshots
├─ files/          # CSV exports from dbt models
│  ├─ staging_valid_fx_tickers.csv
│  ├─ staging_valid_stock_tickers.csv
│  ├─ staging_valid_stock_info.csv
│  ├─ staging_valid_fx_info.csv
│  └─ fact_tab_trading.csv
└─ models/         # dbt transformations
   ├─ schema.yml
   ├─ staging/
   │  ├─ transform_survey.sql
   │  ├─ staging_valid_fx_tickers.sql
   │  ├─ staging_valid_stock_tickers.sql
   │  ├─ staging_valid_stock_info.sql
   │  └─ staging_valid_fx_info.sql
   └─ marts/
      └─ fact_tab_trading.sql
```

