# Patikadev-Kodluyoruz-Homeworks-blob-main-SQL-hw7-GROUPBY-HAVING.sql

--1. SORU

SELECT rating, COUNT(*) FROM film
GROUP BY rating;

--2. SORU

SELECT replacement_cost, COUNT(*) FROM film
GROUP BY replacement_cost
HAVING COUNT(*) > 50
ORDER BY replacement_cost DESC;

--3. SORU

SELECT store_id, COUNT(*) FROM customer
GROUP BY store_id;

--4. SORU

SELECT country_id, COUNT(city)FROM city
GROUP BY country_id
ORDER BY COUNT(city) DESC
LIMIT 1;
