# Competitor-Sales-Analysis-Using-Power-BI
**Requirements:**
<p align="center">
  <img src="https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/requiremetns.png" />
</p>
This Power BI project tackles a comprehensive sales and market share analysis, focusing not only the company's perfomannce internally, reflectiing on how well the product sell, but also externally analyzing how well we are doing against the competing manufactures. It leverages the power of ETL (Extract, Transform, Load) and data visualization to provide valuable insights for informed decision-making.

## Step 1. Data Importing & Tranforiming
Before diving into Power BI, I like to get a feel for the data first.  In this case, we have several data files:
- Sales (US data): This file holds sales information specifically for the United States.
- bi_dimensions (master data): This file acts like a reference point, containing details about Geography, Manufacturers, and Products.
- International Sales (separate files): Five separate files provide sales data for individual countries: Canada, Germany, Japan, Mexico, and Nigeria.

<p align="center">
  <img src="https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/pbi1.png" alt="Image" />
</p>

To analyze sales across all countries, I combined the "Sales" table (containing US data) with the individual "International Sales" files. This created a single, unified table for comprehensive sales insights.

To optimize the Power BI model's performance, I disabled the loading of the separate "International Sales" tables after the merge. This ensures the model uses the combined table for analysis while keeping the original data readily available if needed. 

![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/Screenshot%202024-05-01%20171016.png)


## Step 2. Data Modelling
To create meaningful connections between our data, I implemented the following data modeling steps:
- Sales & Geography Relationship: A calculated column was created in the "Sales" table, likely combining existing columns, to establish a clear relationship with the "Geography" table. This allows Power BI to understand how these tables connect.
- Dedicated Date Table: A separate "Date" table was created. This table likely contains date dimensions (year, month, day, etc.) and was then connected to the "Sales" table. This dedicated structure helps with time-based analysis of sales data.

![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/pbi2.png)

## Step 3. Data Visualization

**Reporting - Overview: Competior Sales**
![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/BI1.png)


**Reporting: Advanced Insights**
![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/BI2.png)


**Reporting - By Product(Category/Segment/Product)**
![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/BI3.png)

**Reporting - By Area(State/City) in United States**
![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/BI4.png)
