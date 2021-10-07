# SQL

**USE** - Database to be used ('USE store;' SQL commands will use store database)

**SELECT** - Mention columns to be selected ('SELECT price FROM product' It will select the price column from the table product)

**WHERE** - Conditions on columns ('SELECT * FROM product WHERE price > 50' It will select all the rows and all the columns where price is greater than 50)

**AND, OR and NOT** - Boolean operations ('SELECT * FROM product WHERE price > 50 AND quantity > 5' It will select rows with all columns where price and quantity matches the conditions)

**IN** - If certain value is there in the list ('SELECT * FROM product WHERE quantity IN (6,14,25)' It will select all the rows where quantity is either 6 or 14 or 25)

**BETWEEN** - Checking values in range ('SELECT * FROM product WHERE price BETWEEN 10 AND 100' It will select all the rows where price of the product is in between 10 and 100)

Date Format - Date is written in string as 'YYYY-MM-DD'

**LIKE** - Similar values ('SELECT * FROM customers WHERE last_name LIKE 'b%'' It will select customers whose last name starts with b, case-insensitive, % means any length of characters, _ means single character)

**REGEXP** - String pattern matching ('SELECT * FROM customers WHERE last_name REGEXP 'field'' It will select rows where customer last name contains 'field') ^ means start of the string and $ means end of the string. | used for or operator. [] to match multiple expressions. [gim]e means ge or ie or me. [a-h]e means ae, be, ce, de, ee, fe, ge or he. 

**IS NULL** - Returns rows with NULL values ('SELECT * FROM customers WHERE phone IS NULL' It will return all the customers whose phone number is null)

**ORDER BY** - Return results ordered by particular column ('SELECT * FROM customers ORDER BY state DESC, first_name' It will return customers in order by state and first name)
Use 'DESC' for descending order. 

**LIMIT** - Limits the rows in a query ('SELECT * FROM customers LIMIT 6,3' It will skip first 6 rows and return next 3 rows)

**JOIN** - Joins two tables ('SELECT * FROM orders JOIN customers ON orders.customer_id = customers.customer_id' It will return columns from both the tables matching customer ids.) For joining tables from different databases, just prefix the name of the database which is not current. 
