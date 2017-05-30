DINOSAURSUS EXERCISES
*********************

1. SELECT COUNT(id) FROM dinos;

 count
-------
   331
(1 row)

2. SELECT name FROM dinos WHERE period = 'Jurassic';

92!!

Too many to list .

would also use SELECT * - to get all instances of Jurrasic DINOSAURSUS

3. SELECT SUM(length) FROM dinos WHERE period='Cretaceous';

   sum   
---------
 1366.45
(1 row)

4. SELECT * FROM dinos WHERE period = 'Jurassic' OR period = 'Cretaceous' ORDER BY species;

Too many to list, checked - worked

5. SELECT * FROM dinos WHERE t_order = 'Saurischia' AND diet = 'Herbivorous';

68 ROWS

6. UPDATE dinos SET name = 'Shortie' WHERE length = (SELECT MIN(length) FROM dinos);
UPDATE 1

Checked - SUCCESSFUL

7. SELECT MIN(name) FROM dinos;
   min    
----------
 Aardonyx
(1 row)

8. UPDATE dinos SET name='The Famous Five' WHERE name IN (SELECT name FROM dinos ORDER BY length DESC LIMIT 5);

UPDATE 5
