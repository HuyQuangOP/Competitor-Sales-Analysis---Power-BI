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
- Create relationship between Sales and Geography by creating a calcualted collum that combines 2 collumns to set a realtionship

![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/pbi2.png)

- Crate new Date table. Connect Date and Sales

## Step 3. Data Visualization

![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/BI1.png)

![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/BI2.png)

![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/BI3.png)

![image](https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/BI4.png)
