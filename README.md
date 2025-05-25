
# 🦅 Bird Migration Analysis with SQL and Data Visualization

This project showcases my practical skills in working with relational data using SQL and visualizing insights using Python-based tools.
The dataset was downloaded from [Kaggle](https://www.kaggle.com/datasets/sahirmaharajj/bird-migration-dataset-data-visualization-eda)
> 🎯 This project combines knowledge gained from university coursework with self-directed learning.

## 📌 Project Objectives

- Showcase knowledge of **SQL** by running queries on a dataset stored in an in-memory SQLite database.
- Use **Pandas** for data processing and transformation.
- Visualize trends and insights using **Seaborn** and **Matplotlib**.
- Analyze bird migration patterns: distances, environmental factors, and species behavior.

  ## 📂 Project Structure

- `Bird_MigrationsSQL_PD.ipynb`: Main notebook with code, SQL queries, and visualizations.
- `README.md` – Project summary and explanation (this file)
- `bird_migration_data.csv`: Dataset used for the analysis.

## 📊 Key Analysis Steps

1. **Data Import and Overview**
   - The dataset includes bird species, regions, habitats, weather conditions, migration reasons, and start/end points.
   - Data is loaded from a CSV file and imported into an SQLite database.

2. **Distance Calculation**
   - The Haversine formula is used to calculate the geographic distance between migration start and end points.

3. **Correlation Analysis**
   - A correlation matrix was generated to examine linear relationships between numerical features such as coordinates and migration distance.
   - The matrix revealed **very weak linear correlations**, with most coefficients below `0.02`. This indicates that the variables are largely **independent** in terms of linear relationships.
   - Consequently, **linear models may not effectively capture patterns** in this dataset. Further analysis may benefit from **non-linear methods** or a focus on **categorical variables** such as species and weather conditions.

4. **Migration Distance Distribution**
   - Visualizations are used to understand the common lengths of migration routes.

5. **SQL Queries + Visual Insights**
   - SQL is used to filter, group, and analyze the data.
   - Results are visualized for easier interpretation.

## 📈 Sample Visual Insights

- **Migration distance histogram**: The mean migration distance is 9,959 km, with a wide distribution ranging from 106 km to 19,971 km, reflecting the diversity of migratory patterns across species.
- **Boxplots by species**: Some birds migrate significantly farther.
- **Weather vs distance**: Most migrations occur under moderate conditions.

## 📉 Data Quality Observations
During the analysis of migration counts by start and end months, it was observed that **some months had zero recorded migrations**, leading to missing bars in the visualizations. However, based on biological expectations and patterns seen in other species, it is likely that this is due **missing data rather than a true absence of migration events**. For example, certain birds are known to start or end migrations in those months, yet the dataset lacks corresponding entries.

## 🛠️ Technologies Used

- **Python**: `pandas`, `numpy`, `random`, `sqlite3`, 
- **Visualization**: `matplotlib`, `seaborn`
- **Jupyter Notebook** for interactive coding and presentation

## 🗒️ Notes

- This project was created as a way to **demonstrate my SQL knowledge** after completing the free interactive course [SQLBolt](https://sqlbolt.com) and expanding on that foundation through self-study.
- I used [SQLiteOnline](https://sqliteonline.com) as a lightweight SQL compiler to quickly visualize and test queries during development.
- 🤝 While the core work was my own, I leveraged resources like **Stack Overflow** and **AI-based tools (e.g., ChatGPT)** to support learning and troubleshooting — reflecting how modern analysts work collaboratively and iteratively in real-world scenarios.

---

This project is a showcase of data manipulation using SQL and effective data visualization using Python tools.
