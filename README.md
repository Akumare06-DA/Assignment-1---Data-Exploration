# Assignment-1---Data-Exploration
Need to Find out following Details From the Data Set ;
Total Product Price 
Total Number of Products
Average Price
Minimum Price
Maximum Price
The count of products with a price less than $100 using the COUNTIF function.
The total price for products in the 'Electronics' category using the SUMIF function.
 Using an IF function, create a new column named Price Range to categorize products with a price greater than or equal to $500 as 'High Price' and others as 'Standard Price'.
 Text Formatting - LEFT, RIGHT, MID:	
	• Create a new column named Day with the first 2 characters of each 'Product ID' using the LEFT function.
	• Create a new column named Country Code by extracting the last 2 characters from the 'Product ID' column using the RIGHT function.
	• Create a new column named Month by extracting 4th to 6th characters from the 'Product ID' column using the MID function

 Excel Functions Used

`SUM` – Calculated the total price of all products - 
=SUM(D2:D35)
* `COUNT` – Counted the number of products -
*  =COUNT(F2:F35)
* `AVERAGE` – Calculated the average product price -
* =ROUND(AVERAGE(D2:D35),2)
* `MIN` – Found the minimum product price -
*  =MIN(D2:D35)
* `MAX` – Found the maximum product price -
*  =MAX(D2:D35)

 Logical Function

* `IF` – Categorized products as:
* =IF(D2>=500,"High Price","Standard Price")

  * **High Price** – Price ≥ $500 
  * **Standard Price** – Price < $500

 Conditional Functions

* `SUMIF` – Calculated the total price of products in the Electronics category --
*  =SUMIF(G2:G35,G2,D2:D35)
* `COUNTIF` – Counted products with a price below $100--
*  =COUNTIF(D2:D35,"<100")

Text Functions

* `LEFT` – Extracted the first two characters from Product ID to create the Day column--
*  =LEFT(A2,2)
* `RIGHT` – Extracted the last two characters to create the Country Code column --
=RIGHT(A2,2)
* `MID` – Extracted the month from the Product ID --
* =MID(A2,4,3)

Key Results

| Analysis                |  Result |
| ----------------------- | ------: |
| Total Product Price     | $10,100 |
| Number of Products      |      34 |
| Average Price           | $297.06 |
| Minimum Price           |     $30 |
| Maximum Price           |  $1,000 |
| Electronics Total Price |  $8,050 |
| Products Below $100     |      11 |
