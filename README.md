# Disney-s-Cinematic-Success
Analyzing Profitability vs. Production Focus

-------Customer Section-------------------------------------------------------------
CREATE Table Customer_statistics (
    invoice_id VARCHAR (50),
    city TEXT,
    customer_type TEXT,
    gender TEXT,
    product_line VARCHAR,
    quantity int,
    total_bill DECIMAL,
    payment_method VARCHAR,
    rating DECIMAL
);

Copy Customer_statistics  
    FROM 'F:\STUDY\Data Analysis\projects\Sales of a Supermarket\Customers Data.csv'
    DELIMITER ',' csv HEADER

Select * 
FROM Customer_statistics
--------------Products Data-----------------------------------------------------------------

CREATE Table product_statistics(
    invoice_id VARCHAR (50),
    gender VARCHAR,
    product_lice VARCHAR,
    unit_price DECIMAL,
    quantity INT,
    total_bill DECIMAL,
    date DATE,
    gross_income DECIMAL,
    rating DECIMAL
);

copy product_statistics 
    FROM 'F:\STUDY\Data Analysis\projects\Sales of a Supermarket\Product Data.csv'
    DELIMITER ',' CSV HEADER

SELECT * FROM product_statistics;

-----------------Brunchs Data-----------------------------------------------------

CREATE TABLE branches_statistics(
    invoice_id VARCHAR(50),
    branch VARCHAR,
    city VARCHAR,
    product_line VARCHAR,
    quantity DECIMAL,
    total_bill DECIMAL,
    cogs DECIMAL,
    gross_income DECIMAL
);
Copy branches_statistics 
    from 'F:\STUDY\Data Analysis\projects\Sales of a Supermarket\Brunches Data.csv'
    DELIMITER ',' CSV HEADER
SELECT *
FROM branches_statistics;
-------------------------------------------------------------------------------------
