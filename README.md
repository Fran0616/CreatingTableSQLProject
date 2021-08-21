# CreatingTableSQLProject
Objective
=
In this project, you will create your own “Friends” table and add/delete data from it. 


1. Create a table named friends with three columns:

- `id` that stores INTEGER

- `name` that stores TEXT

- `birthday` that stores DATE
```
CREATE TABLE friends (
 id INTEGER,
 name TEXT,
 birthday DATE
);
```

2. Beneath your current code, add Ororo Munroe to friends. Her birthday is May 30th, 1940.

```
INSERT INTO friends (id, name, birthday)
VALUES (1, "Ororo Munroe","05/30/40");
```

3. Add two of your friends to the table. 

- Insert an `id`,
- `name`, and
- birthday for each of them.

```
INSERT INTO friends (id, name, birthday)
VALUES (2, "Francisco", "03/23/90");
INSERT INTO friends (id, name, birthday)
VALUES (3, "Stefanie", "09/28/02");
```

4. Ororo Munroe just realized that she can control the weather and decided to change her name. Her new name is “Storm”. Update her record in `friends`.

```
UPDATE friends
SET name = "Storm"
WHERE id = 1;
```

5. Add a new column named `email`.

```
ALTER TABLE friends
ADD email VARCHAR;
```

6. Update the email address for everyone in your table. 

- Storm’s email is storm@codecademy.com.

```
UPDATE friends
SET email = "storm@codeacademy.com"
WHERE id = 1;
```

7. Wait, Storm is fictional… 
- Remove her from friends.

```
DELETE FROM friends
WHERE id = 1;
```

8. Let’s take a look at the result one last time

```
SELECT *
FROM friends;
```



Final Table
=
__________

|id  |name     |birthday  |email|


|2|
|Francisco|
03/23/90|


|3
|Stefanie
|09/28/02|

___________





