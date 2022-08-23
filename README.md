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


## Waiting and timeouts

The resulting value is in seconds.
MariaDB [(none)]> show variables like 'wait%';

+---------------+-------+
| Variable_name | Value |
+---------------+-------+
| wait_timeout  | 28800 |
+---------------+-------+
