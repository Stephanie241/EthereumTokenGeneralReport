# Power BI Report - Cryptocurrency Transaction Analysis

## Overview 
This Power BI report offers insights into cryptocurrency transaction data extracted from the Ethereum blockchain. It leverages an ETL (Extract, Transform, Load) project that collects transaction data for various ERC-20 tokens, processes it for analysis, and stores it in a SQL Server Management Studio (SSMS) database. This README focuses on the Power BI report and its capabilities for visualizing and analyzing the processed data.  

Below is a screenshot showcasing the Power BI report's visualizations:  
![image](https://github.com/Stephanie241/ERC20TokenGeneralReport/assets/144491602/47578833-aa45-4cf2-8da0-0c8cae7fdd32)

## Key Features of the Power BI Report  
### 1. Total Value by Token Symbol (Pie Chart)  
- This visualization provides a clear breakdown of the total transaction values by different token symbols. It allows you to quickly identify which tokens dominate the transaction value.

### 2. Median of Total Value by Token Name and Token Symbol (Bar Chart)  
- This chart offers a deeper analysis by presenting the median transaction values categorized by both token name and token symbol. It helps you understand the distribution of transaction values within each token.  

### 3. Average of Gas Used by Token Symbol (Bar Chart)  
- Gas usage is a crucial metric in cryptocurrency transactions. This bar chart displays the average gas used for transactions, allowing you to compare the efficiency of different tokens.  

### 4. Count of Transactions by Token Symbol (Pie Chart)  
- Transaction volume is an essential aspect of cryptocurrency analysis. This pie chart visualizes the count of transactions grouped by token symbol, giving you insights into token popularity and usage.  

## Interacting with the Report  
To fully harness the capabilities of this Power BI report and explore cryptocurrency transaction data effectively, follow these steps:  

1. **Open the Power BI report file:** Launch Power BI Desktop and open the report file.  

2. **Ensure Data Sources and Connections:** Make sure that the data sources and connections are correctly configured. Verify that the ETL process has successfully populated the SQL Server database.  

3. **Utilize Interactive Features:** Interact with the report's visualizations by using filters, slicers, and drill-through options. You can filter data by specific tokens, time periods, or other relevant criteria to gain deeper insights.  

## Database Schema
The underlying data for this report is stored in a SQL Server database table named `ERC_Tokens`. The table schema includes essential fields such as `blockNumber`, `hash`, `value`, `tokenName`, `tokenSymbol`, and more. Below is a brief overview of the schema:

- `blockNumber` (int)
- `hash` (varchar(MAX))
- `nonce` (int)
- `blockHash` (varchar(MAX))
- `from` (varchar(MAX))
- `contractAddress` (varchar(MAX))
- `to` (varchar(MAX))
- `value` (float)
- `tokenName` (varchar(MAX))
- `tokenSymbol` (varchar(MAX))
- `tokenDecimal` (int)
- `transactionIndex` (int)
- `gas` (float)
- `gasPrice` (nvarchar(MAX))
- `gasUsed` (float)
- `cumulativeGasUsed` (float)
- `input` (varchar(MAX))
- `confirmations` (int)
- `dateTime` (datetime)
- `amount_flag` (varchar(MAX))

## Example Usage
Here's a hypothetical example of how to use this Power BI report:

1. **Objective:** Analyze the transaction data for the "Shiba Inu" token.

2. **Open the Report:** Launch Power BI Desktop and open the report file.

3. **Apply Filters:** Use the filter functionality to select the "Shiba Inu" token.

4. **Analyze Data:** Explore the pie chart to see the percentage of total transaction value attributed to Shiba Inu, check the median transaction values, and gain insights into gas usage.
