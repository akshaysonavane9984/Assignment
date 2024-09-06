
# Assignment

1. Write a Python function that takes a list of records, where each record is a dictionary containing the name of a city and various types of weather data (e.g., temperature, humidity). The function should aggregate this data to provide insights such as the average temperature and humidity for each city. However, each record may not contain all types of data. The solution should gracefully handle missing data.


### Explanation:
The function iterates through the list of records and aggregates the total temperature and humidity for each city.

It keeps a count of how many times temperature or humidity data is available for each city to calculate averages.

It handles missing data by skipping over missing values and ensuring cities without any data have None for the averages.


2. Write a Python function to perform prime factorization of a given integer. The function should return a list of tuples, where each tuple contains a prime factor and its corresponding exponent. For example, given the integer 60, the function should return [(2, 2), (3, 1), (5, 1)] since 60 = 2^2 * 3^1 * 5^1. 

### Explanation:
First, the function divides out the factor of 2 (the only even prime) as many times as it can and records how many times this happens.

It then checks for odd prime factors starting from 3, dividing out the factor and counting how many times each prime divides the number.

The function continues this process until all factors are found or the remaining number is itself a prime larger than 2.

Finally, if there is any remaining prime factor (greater than 2), it is added to the result with an exponent of 1.

In the case of 60, the output shows that:

60 = 2^2 * 3^1 * 5^1.

3.Data Manipulation Challenge:

Scenario: A table named products contains columns id, name, and price.

Task: Write a SQL query to increase the price of all products by 10% and display the new prices along with the product names

SELECT 
    name, 
    price * 1.10 AS new_price
FROM 
    products;


### Explanation:
The SELECT clause fetches the name of the products.

The price is multiplied by 1.10 to increase it by 10%, and the result is aliased as new_price.

The data is retrieved from the products table.
