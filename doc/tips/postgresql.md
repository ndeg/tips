# PostgreSQL

## Executes SQL queries from a given file

```bash
psql --host=[host] --user=[user] [dbaname] -f [/path/to/file.sql]
```

## Disk storage information and optimization

### Size of a table including indexes

```bash
SELECT pg_table_size('tablename');
```
### Vacuum a table

```bash
VACUUM (VERBOSE, FULL) [tablename];
```

[Back to index](../../README.md)
