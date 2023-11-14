# Business-Insights-360-using-Power-BI

## Table of contents

- [Problem Statement](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#problem-statement)
- [Objective](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#Objective)
- [Report features](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#report-features)
- [Project Charter](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#project-charter-)
    - [Success measures](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#success-measures)
    - [Timeline](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#timeline)
    - [Data correctness and completeness](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#data-correctness-and-completeness)
    - [Mockup dashboard](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#requested-for-benchmark-numbers-and-mockup-dashboard)
- [Data Collection and Exploration](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#data-collection-and-exploration)


Power BI 
- [Data Loading and Transformation in Power Query](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#power-bi---data-loading-and-transformation-in-power-query)
   - [Column Distribution and Profile](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#column-distribution-and-profile)
   - [Creating a Date Table](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#creating-a-date-table)
   - [Establishing Fiscal Year](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#establishing-fiscal-year)
   - [Data Validation Against Benchmark Numbers](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#data-validation-against-benchmark-numbers)
   - [Scope the work](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#scope-the-work)
   - [More data transformations](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#more-data-transformations)
   - [Power Query-best practices](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#power-query--best-practices)
- [Data Modelling and Calculated Columns](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/tree/main#data-modelling-and-calculated-columns)
    - [New table using DAX](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#new-fiscal-year-fy-table-using-dax)
    - [Building Data Model Relationships](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#building-data-model-relationships)
    - [Calculated Columns](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#calculated-columns)
- [Optimize report and reduce file size by 25%](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/README.md#optimize-report-and-reduce-file-size)
- [Building actual metrics and visuals](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/tree/main#building-actual-metrics-and-visuals)
  
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
 
#### Success measures: 
- Implementation of a fully operational dashboard.
-Implementation of a fully operational dashboard. including
   - Customer Negotiations
   - New product launches
   - Marketing promotions
   - Finance budgeting.
- Widespread deployment across the entire organization, encompassing all market segments.
#### Timeline: 
- Week 4: Deliver the Minimum Viable Product (MVP) for Unit Acceptance Testing (UAT).
- Subsequent weeks: Perform data validations, gather feedback, and implement necessary improvements.
- Week 8: Deliver the final product.

#### Data correctness and completeness:
For the assurance of data accuracy and completeness, we implement multi-level validation processes: 
- Initial validation against the benchmark numbers within the received database,
- Subsequent validation within Power BI once the data is integrated,
- Further validation during User Acceptance Testing (UAT), and lastly,
- Validation involving input from departmental stakeholders."

#### Requested for Benchmark Numbers and Mockup dashboard
![Mockup dashboard provided](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/4.Rough%20sketch%20of%20Dashboard.png)

## Data Collection and Exploration:

- **Data Catalog Review**: As a data analyst, I begin by browsing the data catalog to gain an understanding of the available databases within the organization. This step helps identify potential data sources.

- **Identifying Required Datasets**: Following a thorough review of the Data Catalog, the necessary datasets are identified. Subsequently, access requests are submitted to the Data Engineering team to obtain the required data. The organization's data warehouse is established on the MySQL platform.

- Note: Data Warehousing is the stage where data is prepared and structured for the purpose of analysis.

- **Data Import**: Once the required data files are obtained as dump files, they are imported using MySQL, a relational database management system.

- **SQL Data Exploration**: SQL, a powerful database querying language, is utilized to conduct the initial exploration of the data. This includes performing queries to gather insights and uncover patterns in the data.

- **Dimension and Fact Tables**: Dimension tables are created to represent attributes related to customers, markets, and products. Fact tables are established to store data on monthly sales and sales forecasts. These tables encompass important metrics such as freight costs, gross prices, manufacturing costs, and post-pre-invoice deduction percentages.

- Sales forecasting: This process serves a crucial role in optimizing inventory, reducing storage costs, and enhancing customer satisfaction by preventing out-of-stock situations.

## Power BI - Data Loading and Transformation in Power Query: 
The datasets are loaded into Power BI from MySQL, and the transformation process is conducted using Power Query. This step allows for cleaning and structuring the data as needed.

#### Column Distribution and Profile: 
The "View" tab is used to provide a quick summary of data, offering insights into data distribution and profile. This is particularly useful for data validation. In the dimension tables, it's essential to check for primary key data, ensuring that distinct and unique values align.

#### Creating a Date Table: 
A date table is created using the M language in Power Query. To do this, a new source is added, and a blank query is initiated. By searching "create date table in Power Query" and following the steps provided in the [microsoft fabric community](https://community.fabric.microsoft.com/t5/Desktop/Creating-Date-Tables/m-p/553980), a date table is established. Our data spans from September 2017 to August 2022.

#### Establishing Fiscal Year: 
AtliQ follows a fiscal year that begins in September and ends in August. To obtain the fiscal year corresponding to the dates, a new column is added to the date table. This column calculates the start of the month, and a custom column is utilized to determine the fiscal year using the formula: **Date.Year(Date.AddMonths([Month], 4))**. The column type is converted to text, and the file is saved.

#### Data Validation Against Benchmark Numbers:
Before creating full-fledged dashboards, it is essential to conduct primary data validation in Power BI. This step ensures that the data is accurate and aligned with benchmark numbers.

It can be seen that our numbers match with the benchmark provided. 
![Data Validation Against Benchmark Numbers](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/6.Validating%20against%20Benchmark.png)

##### Tip: Make sure to pull data from dimension tables.

#### Scope the work: 
> Performing data transformations in advance in Power Query can significantly benefit the development of all four different dashboards.
> It saves a substantial amount of development time by preparing the data for immediate use in creating visuals and reports.

For building the "Performance Over Time" dashboard based on the mockup, the following steps are essential:
1. YTD (Year to Date) and YTG (Year to Go): To calculate these metrics, you need to find the last sales month from the current sales table. A reference table to the sales table is created, and a formula is applied to identify the last sales month. This reference table is then named "LastSalesMonth" and serves as a dynamic variable for the last sales month.
2. YTG Sales Forecast: Create a reference to the forecast table, naming it "remaining_forecast." Filter this table using "> LastSalesMonth"  date
3. YTD Calculation: The Year to Date (YTD) metric is obtained directly from the current sales table.
4. Landing Estimate: To calculate the Landing Estimate, append queries by selecting the current sales table and the remaining forecast table. Name this new table "fact_actuals_estimate."

#### More data transformations 
- Creating reference tables(to find last sales month)
- Append queries (actual sales and forecast tables),
- Merge queries (left join tables to get gross price,pre_invoice_disc_pct),
- Creating custom columns (Gross Sales, Pre_invoice_discount_amount and Net_invoice_sales_amount)

#### Power Query- best practices:
- Gave meaningful names to query steps
- Grouped tables into logical categories
- Disabled loading of tables that are not going to be used outside - helps with performance
- Used consistent naming conventions for tables and measures
- Performed Query folding -choose only the required columns in PQ

## Data Modelling and Calculated Columns:

### New Fiscal Year (fy) table using DAX 
To avoid ambiguity of many-to-many relationships in the data model, built a fiscal_year table that gives unique values of fiscal_Year


![FY](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/7.1%20%20FY%20Table.png)


### Building Data Model Relationships:
Relationships are established between different tables to construct a cohesive data model.

![Data Model](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/7.%20Data%20model.png)


###  Calculated Columns:

We have calculated Gross Sales(GS), Pre_invoice_discount_amount(PreIDA) and Net_invoice_sales_amount(NIS amt) in Power Query

#### Computed further components of the P&L Statements using Calculated Columns 
- post_invoice_deductions_amount (PoID amt), post_invoice_other_deductions_amount (PoIOD amt) from percentages.
- PoID amt = [NIS]*[PoID%], PoIOD amt = [NIS]*[PoIOD%]
- net_sales_amount (NS amt) = NIS - PoID - PoIOD
- manufacturing_cost by multiplying with [qty], frieght_cost & other_cost from percentages*NS
- total_cogs_amt (COGS) = [manufacturing_cost]+[frieght_cost]+[other_cost]
- gross_margin_amount (GM amt) = [NS amt]-[COGS]

## Optimize report and reduce file size by 25%

The file size now is 265MB
![](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/8.2%20space%20analysis.png)

we analyze using an external tool called DAX Studio. The show metrics option in DAX Studio shows the amount of space occupied by each table and each column.
![](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/8%20space%20analysis.png)
We can remove any intermediate columns in Power query or in Power BI without affecting the performance. Power BI will dynamically calculate these values as needed. 

The new reduced file size is 195MB
![](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/8.2%20space%20analysis%20after%20removing%20few%20calculated%20columns.png)

**Thus effectively reducing the file size by 26%**
>(265-195)/265

## Building actual metrics and visuals

> Create all the measures needed for the visuals.

![](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/blob/main/9%20Measures.png)

More measures were created as needed.

> Create a static table called P&L rows and input values as needed to be displayed in the P&L Statement.

![image](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/assets/123518126/937e4108-f0a8-4d94-839c-e8122b120b70)

> Building Visuals: All the visuals are built according to the mock-up dashboard provided. To create visuals and reports, data is pulled from the dim tables.

### Finance View:
    - Used Matrix to build the P&L Structure
    - Line Chart to display Performance over time
    - Matrix for market analysis
    - Built Top product, Market & region visuals

### Sales View: 
    - Top customers & performance matrix visual for NS, GM & GM %
    - Scatter plot for quadrant analysis with NS denoted by the size of the bubble and GM% in the tooltip
    - Product performance analysis from Tree-level breakdown of Segment, Category, and product
    - Unit economics visual
 The focus is on customers and Gross Margin. For sales teams that deal with customers. Each team has its own customer, focus on customer relationship, their sales, and make sure the business is growing per customer.

### Marketing View: 
    - Top Segment, category and product matrix visual for NS, GM & NP
    - Scatter plot for quadrant analysis with NS denoted by the size of the bubble and GM% in the tooltip
    - Product performance analysis from Tree-level breakdown of region and market (countries)
    - Unit economics visual - Waterfalls and donut chart
The focus is on Products and Net Profit. The marketing team is focused on running ads, promotions,  and doing marketing for the products.
Marketing manager in Canada

### Supply Chain Basics: 
    - The supply chain team`s job is to make sure, their manufacturing plant produces enough inventory to satisfy the demands of the customer.
    - Manufacturing plant produces hardware - stored in a warehouse - inventory sent to customers.
    - When the forecast does not match actual sales, there is a problem of excess inventory and cost 
    associated with storing and maintaining it or an Out-of-stock situation which results in lost business.
    - Absolute error needs to be calculated on a monthly and product level granularity.
    -Key metrics 
        - Net Error           = Forecast Qty - Sales Qty
        - Net Error %         = Net Error / Forecast Qty
        - Absolute Error      = Sumx(Abs(Net Error)) for each product code for each date.
        - Absolute Error %    = Absolute Error / Forecast Qty
        - Forecast Accuracy % = 1 - Absolute Error %
    
### Implementing Stakeholder`s Feedback and Suggestions:

- Added Footers showing the Date of Refresh, Last Sales Month, and currency type.
     - Date of Refresh: Initialize a blank Queru in PQ and get DateTime.LocalNow(). Convert it to a table and format it as Date/Time.
     - Last Sales Month Formatted as MMM YY for readability.
- Replaced GM with GM% in Sales and Marketing View.
- Include Targets for the FY 2022 given as an Excel file. Display blank values for previous years.

#### Create a dynamic switch between Targets and LY in the Finance View:

- Use Enter Data in Home page to enter the details of Toggle switch.
- ![image](https://github.com/mythilyram/Business-Insights-360-using-Power-BI/assets/123518126/bdf7b285-2647-41f8-b022-a0d01e5fe512)
- Use this table as a Slicer with a Single select option.
- Create a new measure for dynamic selection
NS BM $ = 
SWITCH(TRUE(),
SELECTEDVALUE('Set BM'[ID])= 1, [NS $ LY],
SELECTEDVALUE('Set BM'[ID])= 2, [NS $ Target]) and include this in the KPI Visual.














### Supply Chain view:  
     - 
      Market - country
      Region - like continent Asia, N/A

      Selected yr - shld be dark color
      "-1 - ligher version

