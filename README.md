# proyectohtml
Proyecto Final
-- This is the first query:

SELECT DISTINCT year from population_years;

-- Populations of Gabon:

SELECT country, population FROM population_years 
WHERE country = 'Gabon'
ORDER BY country DESC
LIMIT 1;

-- Smallest 2005 countries by population:

SELECT country FROM population_years
WHERE year = 2015
ORDER BY population ASC
LIMIT 10;

-- Countries with >100M population in 2010

SELECT DISTINCT country FROM population_years 
WHERE year = 2010 AND population > 100;

-- Countries containing "islands"

SELECT country FROM population_years
WHERE country LIKE '%Islands%';

-- Difference in population in Indonesia:

SELECT year, population FROM population_years
WHERE country = 'Indonesia'
AND year = 2000
OR country = 'Indonesia'
AND year = 2010;


