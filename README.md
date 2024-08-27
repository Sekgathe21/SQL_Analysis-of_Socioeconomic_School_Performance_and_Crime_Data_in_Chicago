# 🎓 SQL Analysis of Socioeconomic, School Performance, and Crime Data in Chicago 🏙️

## Author
**Sekgathe Karabo Matlala**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sekgathe-karabo-matlala-13996b217/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=flat&logo=github&logoColor=white)](https://github.com/Sekgathe21)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=flat&logo=youtube&logoColor=white)](https://www.youtube.com/channel/UC2x4wrj2gQRLukNg7-Ces1Q)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat&logo=codepen&logoColor=white)](https://www.datascienceportfol.io/SekgatheKM22)

---

## 📝 Project Overview

### 🎯 Objective
The primary goal of this project is to utilize SQL to perform an in-depth analysis of three key datasets from the city of Chicago. By exploring these datasets, we aim to uncover significant correlations, trends, and patterns that can inform community development strategies, enhance education policies, and improve crime prevention measures.

### 📊 Datasets
This project leverages three major datasets, sourced from the city of Chicago and provided by IBM Skills Network. Each dataset provides unique insights into different aspects of the city's social fabric:

1. **📈 Socioeconomic Indicators in Chicago**  
   This dataset includes six socioeconomic indicators and a hardship index for each community area in Chicago from 2008-2012. The indicators include metrics such as per capita income, unemployment rates, and educational attainment.  
   **Benefit**: By analyzing these indicators, we can identify areas that may require targeted economic development and social services, helping policymakers address disparities effectively.

2. **🏫 Chicago Public Schools - Progress Report**  
   This dataset contains performance metrics for Chicago public schools, including student test scores, attendance rates, and other key academic indicators.  
   **Benefit**: Understanding school performance across the city allows for the identification of schools that may need additional resources or policy interventions to improve student outcomes.

3. **🚔 Chicago Crime Data**  
   This dataset includes detailed records of reported crimes in Chicago over several years, categorized by type, location, and date.  
   **Benefit**: Analyzing crime data can reveal patterns and correlations with socioeconomic and educational factors, providing insights that can be used to formulate more effective crime prevention strategies.

---

## 🛠️ Tools and Libraries Used

### Tools
- **🔌 SQLite**: A lightweight, serverless SQL database engine used to store and manage the datasets for this project. SQLite is chosen for its simplicity and ability to handle the data size used in this analysis.
- **📒 Jupyter Notebook**: An open-source web application that allows you to create and share documents that contain live code, equations, visualizations, and narrative text. Ideal for combining code execution with detailed explanations.

### Libraries
- **🐼 Pandas**: A powerful data manipulation library in Python, used for data cleaning, transformation, and analysis. Essential for preparing the data before loading it into SQLite and for further analysis after querying the database.
- **🗃️ SQLite3**: The Python interface for SQLite, used to interact with the SQLite database. It allows you to execute SQL queries, retrieve data, and manage database connections within your Python environment.
- **📊 Matplotlib**: A comprehensive library for creating static, animated, and interactive visualizations in Python. Used to visualize the results of the data analysis.
- **📈 Seaborn**: A Python data visualization library based on Matplotlib, providing a high-level interface for drawing attractive and informative statistical graphics. Used for creating advanced visualizations that are aesthetically pleasing and easy to interpret.

---

## 🚀 Project Workflow

### 1️⃣ Step 1: Database Creation Using SQLite
The project begins by creating a database in SQLite, which is a self-contained, serverless, and zero-configuration database engine. This database serves as the foundation for storing and querying the datasets used in the analysis.

**🛠️ Implementation**:  
- Import necessary libraries, including `sqlite3` for database interaction and `pandas` for data manipulation.
- Create the SQLite database by connecting to a database file using `sqlite3.connect()`. If the file does not exist, SQLite automatically creates it.

**✨ Benefit**:  
- Creating a centralized database allows for efficient data management and retrieval, ensuring that the data is organized in a structured format, enabling fast and reliable SQL queries.

### 2️⃣ Step 2: Data Import and Cleaning
Once the database is set up, the next step involves importing the datasets into the SQLite database. This step also includes data cleaning to ensure that the data is accurate, consistent, and ready for analysis.

**🛠️ Implementation**:  
- Load the datasets into pandas DataFrames, where initial cleaning is performed. This may involve handling missing values, renaming columns, and transforming data types to ensure compatibility with SQL.
- Insert the cleaned data into the SQLite database using `to_sql()` from pandas, which efficiently transfers data from a DataFrame to a SQL table.

**✨ Benefit**:  
- Data cleaning is a critical step to avoid errors during analysis. Clean, well-structured data ensures that subsequent queries and analyses are based on reliable information, leading to more accurate and actionable insights.

### 3️⃣ Step 3: Exploratory Data Analysis (EDA)
Exploratory Data Analysis is conducted to understand the basic characteristics of the data. This step involves executing SQL queries to examine descriptive statistics, distributions, and relationships within the datasets.

**🛠️ Implementation**:  
- Execute simple SQL queries using `sqlite3` to explore the datasets, such as counting records, calculating averages, and identifying missing values.
- Visualize data distributions using Matplotlib and Seaborn to identify trends and outliers.

**✨ Benefit**:  
- EDA helps in identifying the underlying structure of the data, revealing patterns and anomalies that guide the direction of more detailed analysis. It provides a solid foundation for making informed decisions during the subsequent steps of the project.

### 4️⃣ Step 4: Advanced SQL Queries
Advanced SQL techniques are employed to dive deeper into the data. This includes using joins, subqueries, and aggregations to answer specific research questions about the socioeconomic conditions, school performance, and crime data.

**🛠️ Implementation**:  
- Craft SQL queries to combine data from different tables, aggregate results, and filter records based on complex conditions. For example, joining socioeconomic data with crime data to analyze correlations between poverty levels and crime rates.
- Use subqueries to perform nested queries, allowing for more sophisticated analysis.

**✨ Benefit**:  
- Advanced SQL queries enable the extraction of complex insights from the data, allowing for the identification of nuanced relationships between variables. This level of analysis is crucial for uncovering actionable insights that can inform policy and strategy.

### 5️⃣ Step 5: Data Visualization and Reporting
The results of the SQL queries are visualized using Matplotlib and Seaborn. This step is crucial for effectively communicating the findings of the analysis to stakeholders.

**🛠️ Implementation**:  
- Convert data retrieved from SQL queries into pandas DataFrames, then create visualizations such as bar charts, line graphs, and heatmaps.
- Use Seaborn to enhance the visual appeal of the plots, making them more accessible and easier to interpret.

**✨ Benefit**:  
- Visualizations make complex data more understandable, allowing stakeholders to quickly grasp the key insights. Effective visual communication is essential for translating data analysis into informed decisions and actions.

### 6️⃣ Step 6: Conclusion and Recommendations (NOT YET DONE)
The final step involves summarizing the findings from the analysis and providing recommendations based on the data insights.

**🛠️ Implementation**:  
- Compile the key findings from the SQL analysis and visualizations into a summary. This includes identifying areas of concern, such as communities with high levels of socioeconomic hardship or schools with declining performance.
- Based on the analysis, make recommendations for community development, educational improvements, and crime prevention strategies.

**✨ Benefit**:  
- The conclusion and recommendations provide actionable insights that can guide policymakers and community leaders in making data-driven decisions. By basing recommendations on empirical data, the project contributes to more effective and targeted interventions.

---

## 🎉 Conclusion
This project demonstrates the power of SQL in analyzing complex datasets to uncover meaningful insights. By systematically exploring the relationships between socioeconomic factors, school performance, and crime data, we can better understand the challenges faced by communities in Chicago and propose informed strategies to address them. The tools and methodologies used in this project serve as a robust framework for conducting similar analyses in other contexts.
