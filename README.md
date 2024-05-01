# Competitor-Sales-Analysis-Using-Power-BI
Requirements:
<p align="center">
  <img src="https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/pbi1.png" alt="Image" />
</p>

This Power BI project tackles a comprehensive sales and market share analysis, focusing not only the company's perfomannce internally, reflectiing on how well the product sell, but also externally analyzing how well we are doing against the competing manufactures. It leverages the power of ETL (Extract, Transform, Load) and data visualization to provide valuable insights for informed decision-making.

## Step 1. Data Importing & Tranforiming
Before diving into Power BI, I like to get a feel for the data first.  In this case, we have several data files:
- Sales (US data): This file holds sales information specifically for the United States.
- bi_dimensions (master data): This file acts like a reference point, containing details about Geography, Manufacturers, and Products.
- International Sales (separate files): Five separate files provide sales data for individual countries: Canada, Germany, Japan, Mexico, and Nigeria.

<p align="center">
  <img src="https://github.com/HuyQuangOP/QuangHuyDao.Portfolio/blob/main/image/Screenshot%202024-05-01%20164219.png" alt="Image" />
</p>

Append International table to Sales. I had to comnbine the Sales table and International Sale to create a single table that can be used to analyze sales of all country. next to imporve the performance of the model, I disabled the table load of International Sales. 
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
