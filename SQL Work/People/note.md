DROP TABLE IF EXISTS persons;

CREATE TABLE persons (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  name TEXT,
  age INTEGER,
  height INTEGER,
  city TEXT,
  favorite_color TEXT	
);

INSERT INTO persons
(name, age, height, city, favorite_color)
VALUES
('Bryson', 27, 175, 'Honolulu', 'Yellow'),
('Paul', 18, 178, 'Pheonix', 'Blue'),
('Iron Man', 42, 180, 'New York', 'Red'),
('HULK', 38, 213, 'Planet Hulk', 'Green'),
('Bran', 26, 170, 'Provo', 'Orange');

SELECT * FROM persons ORDER BY height DESC;
SELECT * FROM persons ORDER BY height ASC;
SELECT * FROM persons ORDER BY age DESC;
SELECT * FROM persons ORDER BY age ASC;
SELECT * FROM persons WHERE age > 20;
SELECT * FROM persons WHERE age = 18;
SELECT * FROM persons WHERE age < 20 OR age > 30;
SELECT * FROM persons WHERE age != 27;
SELECT * FROM persons WHERE favorite_color != 'Red';
SELECT * FROM persons WHERE favorite_color != 'Red' AND favorite_color != 'Blue';
SELECT * FROM persons WHERE favorite_color = 'Orange' OR favorite_color = 'Green';
SELECT * FROM persons WHERE favorite_color IN ('Orange', 'Green', 'Blue');
SELECT * FROM persons WHERE favorite_color IN ('Yellow', 'Purple');