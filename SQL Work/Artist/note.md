INSERT INTO artist
(name)
VALUES
('The Weeknd'),
('Future'),
('Bazzi');

SELECT * FROM artist ORDER BY name DESC LIMIT 10;
SELECT * FROM artist ORDER BY name ASC LIMIT 5;

SELECT * FROM artist WHERE name LIKE 'Black%';
///Use % when finding words that start with the word ""\\\

SELECT * FROM artist WHERE name LIKE '%Black%';
///User %'word'% when finding words that contain with the word ""\\\
