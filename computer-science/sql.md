# SQL

#### Data types

|           |
| --------- |
| Text      |
| Character |
| Boolean   |
| Integer   |
| Real      |
| Date/time |


#### Comparison

|      |                          |
| ---- | ------------------------ |
| `=`  | equal to                 |
| `<`  | less than                |
| `<=` | less than or equal to    |
| `>`  | greater than             |
| `>=` | greater than or equal to |
| `<>` | not equal to             |

#### Boolean

`AND` &emsp; `OR`

<br>

![Parts of a SQL table](images/parts-of-a-sql-table.gif)

## `SELECT ... FROM`

```
SELECT <field>
FROM <table>;

SELECT <field1>, <field2>, ...
FROM <table>;
```

### `WHERE`

```
SELECT <field>
FROM <table>
WHERE <condition>;
```

### `ORDERBY`

|        |            |
| ------ | ---------- |
| `ASC`  | ascending  |
| `DESC` | descending |

```
SELECT <field>
FROM <table>
ORDERBY <order>;

SELECT <field>
FROM <table>
WHERE <condition>
ORDERBY <order>;
```

## `SUM`

```
SUM(<field>)
```

## `COUNT`

```
COUNT(<field>)
```
