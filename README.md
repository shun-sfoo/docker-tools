# docker-tools

## Postgres

查询时区

```sql
SHOW TIMEZONE;
```

## Mysql

查询设置的字符集

```sql
SHOW VARIABLES  WHERE variable_name LIKE '%character%'  OR  variable_name  LIKE '%collation%'
```
