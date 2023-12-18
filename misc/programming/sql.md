# SQL

## Databases

```
CREATE DATABASE [name];
DROP DATABASE [name];
USE [name];
SHOW DATABASES;
```

## Tables

```
CREATE TABLE [name] (…);
  PRIMARY KEY
  NOT NULL
  DEFAULT …
  AUTO_INCREMENT
DROP TABLE [name];
SHOW TABLES;
ALTER TABLE [name] AUTO_INCREMENT = 1;
DESC [name];
```

## Rows

```
INSERT INTO [name] VALUES (…);
UPDATE [name] SET … WHERE …; 
DELETE FROM [name] WHERE …;
```

## Queries

```
SELECT … FROM [name] WHERE …;
  ORDER BY … ASC
  ORDER BY … DESC
  LIMIT [amount]
  GROUP BY …
```
