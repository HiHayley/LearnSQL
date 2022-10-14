# LearnSQL
Cases study and some learning notes on this course.

## Multiple Tables

### 1. With

**`SELECT customer_id,
   COUNT(subscription_id) AS 'subscriptions'
FROM orders
GROUP BY customer_id;`**

This query is good, but a `customer_id` isn't terribly useful for our marketing department.

**`WITH previous_results AS (
  SELECT ...
   ...
   ...
   ...
)
SELECT *
FROM previous_results
JOIN customers
  ON _____ = _____;`**
