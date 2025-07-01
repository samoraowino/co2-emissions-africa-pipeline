# CO₂ Emissions Data Pipeline for African Countries

This project presents an end-to-end data engineering pipeline focused on analyzing and storing carbon emissions data for African nations. It includes data ingestion, cleaning, normalization into a relational database, and exploratory data analysis (EDA) through visualizations.

## Project Summary

- **Objective**: To build a clean and structured data pipeline for CO₂ emissions data in Africa and generate meaningful insights.
- **Data Source**: Publicly available CSV dataset on CO₂ emissions.
- **Tools Used**: Python, SQLite, pandas, matplotlib, seaborn, DBeaver.

## Project Components

### 1. Data Ingestion
- Read raw CSV file using `pandas`.
- Initial inspection and schema review.

### 2. Data Cleaning & Transformation
- Handled missing values.
- Converted column types (e.g., years to integers).
- Created new columns such as CO₂ emissions per capita.

### 3. Database Design (Normalization)
- Structured the database into 3 normalized tables:
  - `Country`: Stores country name, code, and sub-region.
  - `Year`: Holds the distinct years.
  - `Emissions`: Main fact table with foreign keys to `Country` and `Year`.

### 4. SQL Integration
- Created and populated tables using SQLite.
- SQL dump provided (`co2_emissions_dump.sql`) for reproducibility.

### 5. Exploratory Data Analysis (EDA)
Visualizations created include:
- CO₂ Emissions Over Time (per country)
- Emissions Per Capita Over Time
- GDP vs CO₂ Emissions Scatter Plot
- Top 5 CO₂ Emitters in Latest Year
- Emissions by Sub-Region

### 6. Data Ethics Reflection
- Addressed underreporting biases.
- Justified cleaning assumptions and per capita normalization.
- Reflected on the importance of transparent and equitable data use.
