# MovieLens Part 1

Copy and paste you SQL query replacing the lines `<your SQL query here>` inside each question.

0. (Example) List all the columns of the `genres` table.

```SQL
SELECT * FROM genres;
```

1. List all the columns of the `movies` table.

```SQL
SELECT id, title, release_date FROM movies;
SELECT * FROM movies;
```

2. List the `title` and `release_date` of all the movies released in `1995-01-01`.

```SQL
SELECT title, release_date FROM movies WHERE release_date = '1995-01-01';
```

3. List the `title` and `release_date` of all the movies released between `1996-01-01` and `1998-01-01`.

```SQL
SELECT * FROM movies WHERE release_date BETWEEN DATE '1996-01-01' AND '1998-01-01';
```

4. List the `title` of all movies that begins with the letter 'F'.

```SQL
SELECT title FROM movies WHERE SUBSTRING (title, 1, 1) = 'F';
```

5. List the `title` of the oldest movie.

```SQL
SELECT title FROM movies ORDER BY release_date LIMIT 1;
```

6. List the `title` and `release_date` of all the movies from the newest to the oldest one.

```SQL
SELECT title, release_date FROM movies ORDER BY release_date;
```

7. List all release years in ascending order without having repeated values.

```SQL
SELECT DISTINCT release_date FROM movies ORDER BY release_date;
```

8. List the `age` and `gender` of users under 25, but instead of "M" and "F" show "Male" and "Female"

```SQL
<your SQL query here>
```

9. List all users including a "age_group" column that cointains:

- "Infant" when age is below 18
- "Young" when age is between 18 and 30
- "Adult" when age is between 31 and 50
- "Senior" whe age is greater than 50

```SQL
<your SQL query here>
```

10. Using the previous table, list all female users of the groups "Young" and "Adult".

```SQL
<your SQL query here>
```
