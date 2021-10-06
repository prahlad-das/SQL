# SQL

**USE** - Database to be used ('USE store;' SQL commands will use store database)

**SELECT** - Mention columns to be selected ('SELECT price FROM product' It will select the price column from the table product)

**WHERE** - Conditions on columns ('SELECT * FROM product WHERE price > 50' It will select all the rows and all the columns where price is greater than 50)

**AND, OR and NOT** - Boolean operations ('SELECT * FROM product WHERE price > 50 AND quantity > 5' It will select rows with all columns where price and quantity matches the conditions)

**IN** - If certain value is there in the list ('SELECT * FROM product WHERE quantity IN (6,14,25)' It will select all the rows where quantity is either 6 or 14 or 25)

**BETWEEN** - Checking values in range ('SELECT * FROM product WHERE price BETWEEN 10 AND 100' It will select all the rows where price of the product is in between 10 and 100)

Date Format - Date is written in string as 'YYYY-MM-DD'

**LIKE** - Similar values ('SELECT * FROM customers WHERE last_name LIKE 'b%'' It will select customers whose last name starts with b, case-insensitive, % means any length of characters, _ means single character)
