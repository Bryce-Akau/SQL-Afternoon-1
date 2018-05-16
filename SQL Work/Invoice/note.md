SELECT COUNT(*) FROM invoice WHERE BillingCountry = 'USA';
SELECT max(total) FROM invoice;
SELECT min(total) FROM invoice;
SELECT * FROM invoice WHERE total > 5;
SELECT COUNT(*) FROM invoice WHERE total < 5;
SELECT * FROM invoice WHERE BillingState IN ('CA', 'TX', 'AZ');
SELECT AVG(total) FROM invoice;
SELECT SUM(total) FROM invoice;
