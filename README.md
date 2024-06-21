# Nestle Sales Analysis



![image](https://github.com/PerfectAnny/Analysis-on-Nestle-Sales/assets/151845494/6a320976-73a6-46f1-b940-4da6449e6d69)



## Introduction

This is an excel sales analysis carried out on  Nestle products. The project is aimed at analyzing anderiving insights which show the performances of current products and help the company to make data driven decisions.


## Problem statement

1. What is the trend of the total revenue per product in the last 3 years?
2. What is the monthly revenue trend?
3. Compare the different products based on the maximum and minimum revenue generated
4. Which location had the highest and lowest sales? 5.Generate insights from the sales medium to help the head of growth take a decision.


## Skills/ Functions demonstrated;
   
 The following Excel functions were used in this analysis:

. Power Pivot

. Vlookup Function

. If Function

. Max and Min Function

. Date Function





## Trend of Total Sales Per Products

![image](https://github.com/PerfectAnny/Analysis-on-Nestle-Sales/assets/151845494/f38c04d2-ad78-456e-b06f-7118d08d60c6)



This section provides an overview of the company's sales performance. To analyze revenue per product, no special functions are needed. Simply create a pivot table with products in the rows and revenue in the values. The results can be visualized with a column chart and filtered by the desired years.


## Monthly Revenue Trend 
![image](https://github.com/PerfectAnny/Analysis-on-Nestle-Sales/assets/151845494/3025e7e7-944f-4840-8dcd-1e051f1ba76b)


<div style="text-align: center;">
  To extract the month from the dates, the TEXT function (`=TEXT([@Date], "mmm")`) is used. A pivot table is then created with the month in the rows and revenue in the values box. This setup provides a visual representation of revenue generated each month, allowing us to observe monthly revenue trends.
</div>

## Max                                                 
![image](https://github.com/PerfectAnny/Analysis-on-Nestle-Sales/assets/151845494/61181e8a-5183-4538-9518-5effcde5cdfa)
## Min
![image](https://github.com/PerfectAnny/Analysis-on-Nestle-Sales/assets/151845494/fcdf13a7-b130-4859-a896-2e877df7d38e)
<div style="text-align: center;">
  The maximum and minimum revenue are determined by creating a pivot table with product in the rows and revenue in the values. The value field settings are then adjusted to display the maximum and minimum revenue. This provides the company with a clear understanding of the revenue performance of each product.
</div>

## Location with the highest and lowest revenue
![image](https://github.com/PerfectAnny/Analysis-on-Nestle-Sales/assets/151845494/800ad070-ff06-466e-ba4e-95371e7df089)
<div style="text-align: center;">
  To analyze the locations with the highest and lowest sales, we created a pivot table summarizing the required data (revenue and location). To identify these locations, a VLOOKUP function (`=VLOOKUP(L57, L57:M63, 2, FALSE)`) was used to create a table from the pivot table, containing columns for location and revenue. Next, the IF, MAX, and MIN functions (`=IF([@Sales]=MAX([Sales]), [@Sales], "NA")`) were employed. The results were then visualized using a column chart with distinct colors highlighting the locations with the highest and lowest sales.
</div>









