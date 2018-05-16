DROP TABLE IF EXISTS orders;

CREATE TABLE orders (
  person_id INTEGER,
  product_name TEXT,
  product_price FLOAT,
  quantity INTERGER
);

INSERT INTO orders
(person_id, product_name, product_price, quantity)
VALUES
(1, 'Spam', 3.50, 100),
(2, 'Corn Beef', 5.25, 50),
(3, 'Corona', 10, 2),
(4, 'Pizza', 6, 4),
(5, 'Coke', 10, 13);

SELECT * FROM orders;
SELECT SUM (quantity) FROM orders;
SELECT SUM (product_price * quantity) FROM orders;
SELECT SUM (product_price * quantity) FROM orders WHERE person_id = 1;