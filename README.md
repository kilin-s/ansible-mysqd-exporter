# [Mysqld exporter](https://github.com/prometheus/mysqld_exporter)


1 Create user
```
CREATE USER 'exporter'@'localhost' IDENTIFIED BY 'XXXXXXXX' WITH MAX_USER_CONNECTIONS 3;
GRANT PROCESS, REPLICATION CLIENT, SELECT ON *.* TO 'exporter'@'localhost';
```
2 Define password in ansible vault file

```yml
mysqld_exporter_password: XXXXXXXX
```

