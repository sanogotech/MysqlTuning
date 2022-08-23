# MysqlTuning
Mysql Tuning


## Docs
- https://geekflare.com/mysql-performance-tuning/
- https://geekflare.com/fr/mysql-performance-tuning/


## Optimize the MySQL query cache

MariaDB [(none)]> SHOW VARIABLES LIKE 'have_query_cache';

+------------------+-------+
| Variable_name    | Value |
+------------------+-------+
| have_query_cache | YES   |
+------------------+-------+


MariaDB [(none)]> SHOW VARIABLES LIKE 'query_cache_type';

+------------------+-------+
| Variable_name    | Value |
+------------------+-------+
| query_cache_type | ON    |
+------------------+-------+


MariaDB [(none)]> SET GLOBAL query_cache_type = ON;


MariaDB [(none)]> SHOW VARIABLES LIKE 'query_cache_size';

+------------------+----------+
| Variable_name    | Value    |
+------------------+----------+
| query_cache_size | 16777216 |
+------------------+----------+



## Waiting and timeouts

The resulting value is in seconds.
MariaDB [(none)]> show variables like 'wait%';

+---------------+-------+
| Variable_name | Value |
+---------------+-------+
| wait_timeout  | 28800 |
+---------------+-------+
