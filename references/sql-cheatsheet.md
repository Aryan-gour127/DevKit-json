# SQL cheat sheet

Examples use broadly familiar SQL; syntax varies across database products.

## Read and filter

```sql
SELECT name, created_at
FROM users
WHERE active = TRUE
ORDER BY created_at DESC
LIMIT 10;
```

## Join and aggregate

```sql
SELECT teams.name, COUNT(users.id) AS member_count
FROM teams
LEFT JOIN users ON users.team_id = teams.id
GROUP BY teams.name
HAVING COUNT(users.id) > 0;
```

## Change data

```sql
INSERT INTO users (name) VALUES ('Example');
UPDATE users SET active = FALSE WHERE id = 123;
DELETE FROM users WHERE id = 123;
```

Use a restrictive `WHERE` clause for `UPDATE` and `DELETE`. Prefer parameterized statements in applications; never build SQL by concatenating untrusted input. Use transactions where appropriate.

References: [PostgreSQL tutorial](https://www.postgresql.org/docs/current/tutorial.html), [SQLite SQL language](https://sqlite.org/lang.html).
