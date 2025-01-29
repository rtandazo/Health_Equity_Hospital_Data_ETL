# **Health Equity Hospital Data ETL**

---

## **Overview**

This project demonstrates an end-to-end **ETL process** for processing, cleaning, and transforming **CMS's Health Equity at the Hospital Level** dataset. The ETL process automates data preparation using **Python**, ensuring a structured and Tableau-ready format for analysis. The final output enables **geospatial mapping, performance benchmarking, and domain-level scoring insights** in a **Tableau dashboard**.

The analysis reveals **gaps in hospital participation and performance on health equity measures**, with **Domain 3 (Data Analysis) and Domain 5 (Leadership Engagement) emerging as the most failed domains nationwide**. Wyoming had the **lowest average score**, and states like **DC, DE, RI, VT, and CT had the lowest participation rates**. The findings highlight **systemic challenges in leadership accountability and data-driven equity efforts**.

---

## **Key Features**

### **Python ETL**
- **Automated Data Cleaning**:
  - Standardized **facility names** for uniformity
  - Ensured **ZIP codes** retained leading zeros for accurate geospatial mapping
  - Managed **missing data** where hospitals self-reported “Not Available” but still received perfect scores

- **Data Reshaping & Transformation**:
  - Reorganized the dataset to **pivot hospital domain scores** into an **analysis-friendly format**
  - Converted attestation responses into a structured **Yes/No binary system** for easier interpretation
  - Merged **hospital-level and state-level participation data** for Tableau integration

- **File Output for Analysis**:
  - **Final CSV Output**: `Health_Equity_Hospital_Clean.csv` (structured for direct Tableau ingestion)
  - **Log Messages**: Provides processing feedback and completion status

---

## **Tableau Dashboard**
📊 **[Explore the Dashboard Here](#)** *(Insert actual Tableau Public link when available)*  
The interactive **Tableau dashboard** built using this dataset includes:
- **State-Level & Zip Code Drilldowns**:
  - Users can filter by **state → zip code → hospital details**
- **Geospatial Insights**:
  - Maps displaying **state-level and zip-level** hospital equity scores
- **Stacked Bar Chart**:
  - Breakdown of **passing vs. failing hospitals per domain**
- **Highlight Table**:
  - Identifies the **five states with the lowest participation**

---

## **Skills Demonstrated**

### **Python Skills**
- **Data Cleaning & Transformation**:
  - Used **Pandas** for efficient data wrangling and normalization
  - Designed reusable functions for **standardization, renaming, and missing value handling**
  - Automated **pivoting and merging operations** to create a structured dataset

- **Automation & Scalability**:
  - Developed a **fully automated ETL script** to process updates seamlessly
  - Ensured **scalability** by structuring the ETL for **future CMS dataset updates**

### **Tableau Skills**
- **Data Visualization & Action Filters**:
  - Built **interactive dashboards** to track hospital performance and participation rates
  - Implemented **state-to-zip drilldowns** for granular insights
  - Designed **dynamic KPI summaries** to highlight key trends

- **Geospatial Analysis**:
  - Mapped hospital equity scores at **state and zip code levels**
  - Ensured **accurate geospatial representation** by cleaning and formatting ZIP codes
