# sql_patika_odev_7   www.patika.dev
--answer 1
SELECT rating, COUNT(*) FROM film
GROUP BY rating;
--answer 2
SELECT replacement_cost, COUNT(*) FROM film
GROUP BY replacement_cost
HAVING COUNT(*) >50;
--answer 3
SELECT store_id, COUNT(customer_id) FROM customer
GROUP BY store_id;
--answer 4
SELECT country_id, COUNT(city_id) FROM city
GROUP BY country_id
ORDER BY COUNT(city_id) DESC
LIMIT 1;
