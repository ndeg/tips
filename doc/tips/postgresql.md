# PostgreSQL

## Databases

Gets all databases :

```sql
\l
```

## Exports

To get a SQL query result exported to CSV :

```sql
COPY (SELECT 1 AS col1, 2 AS col2) TO '/tmp/query.csv';
```

## Executes SQL queries from a given file

```bash
psql --host=[host] --user=[user] [dbaname] -f [/path/to/file.sql]
```

## Disk storage information and optimization

### Size of a table including indexes

```sql
SELECT pg_table_size('tablename');
```
### Vacuum a table

```sql
VACUUM (VERBOSE, FULL) [tablename];
```

[Back to index](../../README.md)
