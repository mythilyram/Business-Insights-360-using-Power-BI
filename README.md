# Business-Insights-360-using-Power-BI

## Table of contents

- [Problem Statement](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#problem-statement)
- [Objective](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#Objective)
- [Report features](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#report-features)
- [Project Charter](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#project-charter-)
- [Data Collection and Exploration](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#data-collection-and-exploration)
  
## Problem Statement:

AtliQ Hardware, a global consumer electronics company, is experiencing significant growth in its operations across multiple countries. However, the company's current reliance on Excel files for data analytics is proving to be inadequate. Excel files are challenging to work with, especially when dealing with large datasets, and they fall short in extracting valuable insights. This deficiency in effective analytics has resulted in substantial losses for the company in certain regions.

## Objective: 
The primary objectives are to:

- Integrate data analytics to foster data-driven decision-making practices across all market segments.
- Enhance transparency in data processes and outcomes.
- Achieve a measurable quantitative improvement, with the goal of a 10% increase in profit margin.
## Report features: 
![Report features given by the product owner](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/2.report%20feautures.png)

Every individual Power BI dashboard or view serves a distinct purpose by addressing specific types of questions. Each component of the report is designed to provide insights tailored to its intended audience and objectives.

## Project Charter : 
![Project Charter link](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/3.%20project-charter.pdf)
- During the project kickoff meeting, we delved into a comprehensive discussion of the report features and addressed any lingering questions or concerns.

- In this process, I gained a deeper understanding of the significance of a 'Project Charter' in the context of corporate operations. A 'Project Charter' serves as a concise but comprehensive document encapsulating the entirety of the project.

- We employed a collaborative tool called Mural to facilitate this process. In doing so, we covered several critical aspects of the project, including the project's objectives, key stakeholders, expectations, concerns, and potential risks.

This approach provides a structured foundation to guide our project's journey towards success.
 
### Success measures: 
- Implementation of a fully operational dashboard.
-Implementation of a fully operational dashboard. including
   - Customer Negotiations
   - New product launches
   - Marketing promotions
   - Finance budgeting.
- Widespread deployment across the entire organization, encompassing all market segments.
### Timeline: 
- Week 4: Deliver the Minimum Viable Product (MVP) for Unit Acceptance Testing (UAT).
- Subsequent weeks: Perform data validations, gather feedback, and implement necessary improvements.
- Week 8: Deliver the final product.

### Data correctness and completeness:
For the assurance of data accuracy and completeness, we implement multi-level validation processes: 
- Initial validation against the benchmark numbers within the received database,
- Subsequent validation within Power BI once the data is integrated,
- Further validation during User Acceptance Testing (UAT), and lastly,
- Validation involving input from departmental stakeholders."

### Requested for Benchmark Numbers and Mockup dashboard

## Data Collection and Exploration:

- **Data Catalog Review**: As a data analyst, I begin by browsing the data catalog to gain an understanding of the available databases within the organization. This step helps identify potential data sources.

- **Identifying Required Datasets**: Following a thorough review of the Data Catalog, the necessary datasets are identified. Subsequently, access requests are submitted to the Data Engineering team to obtain the required data. The organization's data warehouse is established on the MySQL platform.

- Data Warehousing: Data warehousing is the stage where data is prepared and structured for the purpose of analysis.

- **Data Import**: Once the required data files are obtained as dump files, they are imported using MySQL, a relational database management system.

- **SQL Data Exploration**: SQL, a powerful database querying language, is utilized to conduct the initial exploration of the data. This includes performing queries to gather insights and uncover patterns in the data.

- **Dimension and Fact Tables**: Dimension tables are created to represent attributes related to customers, markets, and products. Fact tables are established to store data on monthly sales and sales forecasts. These tables encompass important metrics such as freight costs, gross prices, manufacturing costs, and post-pre-invoice deduction percentages.

- **Denormalization**: It is noted that the sales and forecast tables are denormalized. Denormalization simplifies data analysis and querying by reducing the complexity associated with retrieving information from multiple tables.

- **Sales forecasting**: This process serves a crucial role in optimizing inventory, reducing storage costs, and enhancing customer satisfaction by preventing out-of-stock situations.

### Power BI
 The datasets are loaded into Power BI from MySQL and transformed in Power Query

 Column distribution & profile in the view tab show a quick summary of data and data validation. particularly in dimension tables check for primary key data if distinct 7 UNIQUE VALUES ARE equal.
 Create a date table using M language .
 new source - blank query - google "create date table in power query" and follow steps given in [microsoft fabric community](https://community.fabric.microsoft.com/t5/Desktop/Creating-Date-Tables/m-p/553980) our data is between Sept 2017 and Aug 2022.
  We were informed that Atliq follows a Fiscal year that starts from September-August.
To get the Fiscal year for the corresponding dates, In the date table, use add column to get start of the month. Use a custom column to get the FY using the formula Date.Year(Date.AddMonths([Month],4)). Convet col type to text. Save file 





