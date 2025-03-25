# Friends Database Project

This project demonstrates basic SQL operations to manage a simple "friends" table using SQLite or any SQL-based system. It covers the fundamental operations of **creating**, **inserting**, **updating**, **altering**, and **deleting** data in a relational database.

## 🗂️ Table Structure

We start by creating a `friends` table with the following columns:

- `id` (INTEGER): Unique identifier for each friend.
- `name` (TEXT): Name of the friend.
- `birthday` (DATE): Friend's birthdate.

Later, we alter the table to add:

- `email` (TEXT): Friend's email address.

## 📥 Data Insertion

Initial data entries include the following:

```sql
INSERT INTO friends (id, name, birthday) VALUES (1, 'Ororo Munroe', '1940-05-30');
INSERT INTO friends (id, name, birthday) VALUES (2, 'yash', '2001-06-06');
INSERT INTO friends (id, name, birthday) VALUES (3, 'Ororo Munroe', '2001-06-06');
```

## ✏️ Data Updates

We updated the name of the first record from `"Ororo Munroe"` to `"Storm"` and added email addresses to all records:

```sql
UPDATE friends SET name = 'Storm' WHERE id = 1;
UPDATE friends SET email = 'storm@codecademy.com' WHERE id IN (1, 2, 3);
```

## 🔧 Table Modification

The `email` column was added using:

```sql
ALTER TABLE friends ADD COLUMN email TEXT;
```

## ❌ Deleting Records

The record with `id = 1` was removed from the table:

```sql
DELETE FROM friends WHERE id = 1;
```

## 📊 Final Output

The final `SELECT` statement displays the remaining records in the `friends` table after the operations:

```sql
SELECT * FROM friends;
```

## ✅ Learning Objectives

Through this project, you practice:

- Creating tables
- Inserting data
- Updating values
- Altering tables to add columns
- Deleting records
- Running SELECT queries

This project is a great starting point for beginners learning SQL and relational database manipulation.
