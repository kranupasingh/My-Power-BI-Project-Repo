# 📊 Power BI Retail & Sales Analytics Project

---
<p align="center"> <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" /> <img src="https://img.shields.io/badge/Power%20Query-217346?style=for-the-badge&logo=microsoft&logoColor=white" alt="Power Query" /> <img src="https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" alt="DAX" /> <img src="https://img.shields.io/badge/Data%20Analytics-5A67D8?style=for-the-badge&logo=googleanalytics&logoColor=white" alt="Data Analytics" />

---
**<p align="center">📖 Project Overview**

This project was completed as part of my Level 3 Data Analytics Bootcamp and focuses on using Microsoft Power BI to demonstrate the end-to-end data analytics process, from data transformation and modelling through to analysis, visualisation and data storytelling.
The aim was to create dashboards that highlight sales performance, profitability, trends and regional insights, while allowing users to interact with the data and explore different areas of the business.

---
**<p align="center">🎯Project Objectives**

The key objectives of this project were to:

-🧹 Clean and transform raw retail and sales data

-🔄 Prepare data for analysis using Power Query

-🗄️ Create relationships between tables

-🧮 Develop calculated columns and DAX measures

-📊 Analyse sales and profitability

-📈 Identify trends and patterns over time

-🌍 Compare regional performance

-🛍️ Analyse product and category performance

-🎛️ Create interactive reports and dashboards

-💡 Communicate findings through data storytelling

-🚀 Demonstrate how data can support business decision-making

-🔄 Data Analytics Process

---
**<p align="center"> Core Skills Demonstrated**
---
**🧹 Data Transformation & Cleaning (Power Query)**

Power Query was used to import, clean and prepare the datasets for analysis.

Activities included:
- Importing raw datasets
- Cleaning and preparing the data (remove errors, duplicates and null values)
- Reviewing data quality
- Converted data types and enforced schema consistency
- Renaming fields where required
- Applied transformations such as
    + Group by
    + Replace values
    + Conditional columns
    + Parameter creation
    + Query referencing
      
The transformation stage helped ensure that the data was structured consistently and ready for modelling, analysing and visualisation.

---
**<p align="center">🗄️Data Modelling and Semantic Layer**

Relationships between tables were created to support effective analysis within Power BI.
- Built star-schema with fact and dimension tables
- Managed relationships (one-to-many, cross filter direction)
- Configured semantic models for efficient reporting
- Created hierarchies (e.g. Year - Month - Day)
- Set up model properties such as formatting, summarisation, and data categories

<img width="841" height="447" alt="image" src="https://github.com/user-attachments/assets/0eb7a9db-164f-4f13-a7e7-9ac912206abe" />

This diagram show the star-schema data model used in Power BI, with clearly defined fact and dimension tables. It highlights how relationships are created between tables. A well-structured data model helped ensure that filters, calculations and visualisations interacted correctly throughout the report.

---
**<p align="center">🧮DAX Calculations**

DAX (Data Analysis Expressions) was used to create calculated columns and measures to support the analysis.

Examples included:

💰 Profit margins

📈 Year-over-year growth

📊 Cumulative sales

🔢 Key performance metrics


These calculations allowed the raw data to be transformed into meaningful business measures that could be used throughout the dashboards

**DAX Measures for Regional Sales Percentages**

These DAX measures calculate sales percentages at different geographic levels: Region, Country, and Group. They use DIVIDE(), CALCULATE(), and REMOVEFILTERS() to control context, and ISINSCOPE() to ensure correct behaviour inside hierarchical visuals such as matrices.

<img width="940" height="389" alt="image" src="https://github.com/user-attachments/assets/93b979a2-c117-43c6-b8e9-9b85bf2b888f" />

1. Sales % All Region Percentage of total sales across all regions, ignoring the Region filter.
Sales % All Region = DIVIDE( SUM(Sales[Sales]), CALCULATE( SUM(Sales[Sales]), REMOVEFILTERS(Region) ) )
2. Sales % Country Percentage of total sales for the country, ignoring the Region level. With ISINSCOPE() for correct matrix behaviour:
Sales % Country = IF( ISINSCOPE(Region[Region]), DIVIDE( SUM(Sales[Sales]), CALCULATE( SUM(Sales[Sales]), REMOVEFILTERS(Region[Region]) ) ) )
3. Sales % Group Percentage of total sales for the group, ignoring both Region and Country filters. With ISINSCOPE() for hierarchical accuracy:
Sales % Group = IF( ISINSCOPE(Region[Region]) || ISINSCOPE(Region[Country]), DIVIDE( SUM(Sales[Sales]), CALCULATE( SUM(Sales[Sales]), REMOVEFILTERS(Region[Region], Region[Country]) ) ) )


---
**<p align="center">📊 Data Visualisation**

A range of Power BI visualisations were developed to communicate the retail and sales story.

<table> <thead> <tr> <th>Visualisation</th> <th>Purpose</th> </tr> </thead> <tbody> <tr> <td>📊 <strong>Bar Charts</strong></td> <td>Compare categories, sales and performance</td> </tr> <tr> <td>📈 <strong>Line Charts</strong></td> <td>Analyse sales and profit trends over time</td> </tr> <tr> <td>🧾 <strong>Card Visuals</strong></td> <td>Display key metrics such as total sales and profit</td> </tr> <tr> <td>🥧 <strong>Pie Charts</strong></td> <td>Show sales distribution by product category</td> </tr> <tr> <td>🗺️ <strong>Map Visuals</strong></td> <td>Explore geographical sales performance</td> </tr> </tbody> </table>

---
**<p align="center">🎛️ Interactive Reporting**

A key part of the project was creating reports that allowed users to interact with and explore the data.

**The dashboards included:**

🎛️ Slicers for dynamic filtering

🔎 Filters for targeted analysis

🛍️ Category-level exploration

📅 Time-period analysis

🌍 Regional analysis

🔍 Drill-down functionality

📊 Interactive visualisations

These features allow users to move beyond static reporting and investigate the data from different perspectives.


---
**<p align="center">🚀 Publishing & Sharing**

The reports were published to Power BI Service to explore online reporting and sharing functionality.

**This provided practical experience with:**
☁️ Publishing reports | 📊 Viewing reports online | 🤝 Sharing dashboards | 💬 Gathering feedback | 🔄 Improving report design | 📁 Building a professional data portfolio

Publishing the project also provided an opportunity to consider how dashboards can be shared with users and stakeholders in a real-world environment.

---
**<p align="center">🧰 Tools & Technologies**

<p align="center">

<img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />

<img src="https://img.shields.io/badge/Power%20Query-217346?style=for-the-badge&logo=microsoft&logoColor=white" alt="Power Query" />

<img src="https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" alt="DAX" />

<img src="https://img.shields.io/badge/Power%20BI%20Service-742774?style=for-the-badge&logo=powerbi&logoColor=white" alt="Power BI Service" />

</p>

---
📚 Learning Outcomes

Through this project, I gained hands-on experience with:

💻 Power BI Desktop |☁️ Power BI Service | 🧹 Power Query | 🧮 DAX | 🗄️ Data modelling | 📊 Data visualisation | 🎛️ Interactive dashboard development | 📖 Data storytelling | 💡 Business-focused analysis

The project strengthened my understanding of how technical data skills can be combined with effective visual communication to make data more accessible and impactful.

---
**<p align="center">🌱 What's Next?**

As I continue developing my data analytics skills, I plan to:

📊 Build more advanced Power BI dashboards

🧮 Develop more complex DAX measures

🗄️ Strengthen data modelling skills

☁️ Expand my knowledge of Power BI Service and Azure

🐍 Apply Python to real-world data analysis

🗄️ Develop more advanced SQL skills

💼 Continue building a portfolio of business-focused analytics projects
