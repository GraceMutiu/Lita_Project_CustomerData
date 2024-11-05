# Lita_Project_CustomerData
This is where the customer data for my final project is documented at the end of Lita training

### Project Overview
This project demonstrates the workflow for analyzing a dataset that contains customer data for a subscription service using Microsoft Excel, SQL Server and PowerBi. The goal of the project is to showcase how the data can be analyzed, and visualized to identify segments and trends in order to understand the behaviour of subscribers with the final aim of creating an interactive PowerBi dashboard that represents the analysis.

### Data Source
The customer data for the subscription service was provided by the facilitators for the final project of the training. The dataset contains the customerid, customer name, region, subscription type, subscription start and end date, canceled subscription and revenue.

### Tools and Techniques
- Microsoft Excel: This was used for the initial data cleaning, creation of pivot tables and to perform basic analysis like avaerage, count etc.
- SQL Server: This was used for querying and manipulating the dataset. Most of the analysis was performed using SQL.
- Power BI: This was used to create interactive visualizations and dashboards that provide a summary of the data analysis results.

### Steps Taken
1. Data Cleaning
- Removing Duplicates: The data was cleaned using excel to remove duplicates. There were 75,000 rows before the duplicates were removed resulting in 33,788 rows left.
- Pivot Tables: The data was summarized using pivot tables to find the subscription pattern. In order to get the subscription pattern, the subscription frequency was found to know which of the plans was subscribed to the most. The image shows that the basic plan was subscribed to the most.
  
  ![image](https://github.com/user-attachments/assets/6f096e83-be1e-48ed-83b4-2958076c45da)

2. Data Analysis
- Microsoft Excel: Excel formulas were to used to find the average subscription duration and to identify the most popular subscription types.
  -Average subscription duration: The duration for each customer was calculated first by subtracting the start date from the end date, then the average was found.
``` Excel
=DAYS(F2,E2)

=AVERAGE(I2:I33788)
```
  -Most popular subcription type: The different subscription types were counted using the countif function and the highest was selected as the most popular.
``` Excel
=COUNTIF(D2:D33788, "basic")

=COUNTIF(D2:D33788, "premium")

=COUNTIF(D2:D33788, "standard")
```

#### Summary
From the analysis performed, it was discovered that the average subscription duration was 365 days which is a year. So the customers subscription usually run for an entire year before subscribing again. The most popular subscription plan is the basic plan.

- SQL 

  


  
