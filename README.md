# DDL exercise
Creating Tables:
Create a table named Movies with the following columns:
movie_id (integer)
title (varchar, maximum length 100)
director (varchar, maximum length 50)
release_year (integer)
genre (varchar, maximum length 50)

```SQL
CREATE TABLE movies(movie_id INT, title VARCHAR(100), director VARCHAR(50), release_year INT, genre VARCHAR(50));
```

Altering Tables:
Alter the Movies table to add a new column named rating of type decimal(3, 1).
```SQL
ALTER TABLE movies ADD COLUMN rating DECIMAL(3,1);
```

Dropping Tables:
Create a new table named Students with columns:

student_id (integer)
student_name (varchar, maximum length 50)
age (integer)
grade (varchar, maximum length 2)
Then, drop the Students table.
```SQL
CREATE TABLE students(student_id INT, student_name VARCHAR(50), age INT, grade VARCHAR(2));
DROP TABLE students;
```
Truncating Tables:
Create a table named Events with columns:

event_id (integer)
event_name (varchar, maximum length 100)
date (date)
location (varchar, maximum length 100)
Insert some sample data into the Events table. Once done, truncate the table to remove all records while keeping the table structure intact.

```SQL
CREATE TABLE events(event_id INT, event_name VARCHAR(100), date DATE, location VARCHAR(100));
INSERT INTO events VALUES(1,'EVENT','2023-12-13','online');
TRUNCATE events;
```

Renaming Tables:
Create a table named Restaurants with columns:

restaurant_id (integer)
name (varchar, maximum length 50)
cuisine (varchar, maximum length 50)
location (varchar, maximum length 100)
Rename the table to DiningSpots.

```SQL
CREATE TABLE restaurants(restaurant_id INT, name VARCHAR(50), cuisine VARCHAR(50), location VARCHAR(100));
ALTER TABLE restaurants RENAME TO diningspots;
```
