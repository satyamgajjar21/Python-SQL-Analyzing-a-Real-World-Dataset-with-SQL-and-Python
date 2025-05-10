<p align="center">
  <a href="https://skills.network/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork22-2022-01-01" target="_blank">
    <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/assets/logos/SN_web_lightmode.png" width="200" alt="Skills Network Logo" />
  </a>
</p>

# Analyzing a Real-World Dataset with SQL and Python

This project analyzes a dataset of selected socioeconomic indicators for Chicago using SQL queries and Python visualization tools.

---

## 📌 Objectives

By the end of this project, you will be able to:

- Understand the structure of a real-world dataset with multiple indicators
- Store and query data using Db2 on IBM Cloud
- Analyze data using SQL
- Visualize relationships using Python and Seaborn

---

## 📊 Dataset Description

This dataset includes six public health-related socioeconomic indicators and a hardship index for 77 community areas in Chicago (2008–2012).

| Variable | Description |
|----------|-------------|
| `ca` | Community Area Number |
| `community_area_name` | Community name |
| `percent_of_housing_crowded` | % of crowded housing |
| `percent_households_below_poverty` | % below poverty |
| `percent_aged_16_unemployed` | % unemployed (16+) |
| `percent_aged_25_without_high_school_diploma` | % without HS diploma |
| `percent_aged_under_18_or_over_64` | % dependents |
| `per_capita_income_` | Per capita income |
| `hardship_index` | Composite hardship score (1–100) |

🔗 [View dataset on Chicago Data Portal](https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2)

---

## 🔌 Setup & Connection

This notebook uses:
- `ibm_db` for connecting to Db2 on IBM Cloud
- `ipython-sql` magic for executing SQL in notebooks
- `pandas` and `seaborn` for analysis and plotting

To connect:

```python
%sql ibm_db_sa://<username>:<password>@<host>:<port>/<database>?security=SSL
