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

## Docker command

```bash
docker container ls -a |awk 'NR > 2{print $1} END{print $1}'|xargs docker container rm # rm container
docker rmi $(docker images -a -q) # rm images
docker volume ls -f dangling=true
docker volume prune
```
