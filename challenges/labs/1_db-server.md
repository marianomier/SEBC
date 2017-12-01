DB Server

Hostname Information
```
MariaDB [(none)]> select @@HOSTNAME;
+------------------------------+
| @@HOSTNAME                   |
+------------------------------+
| ip-172-31-4-213.ec2.internal |
+------------------------------+
1 row in set (0.00 sec)
```

Database Engine Version
```
MariaDB [(none)]> select @@VERSION;
+----------------+
| @@VERSION      |
+----------------+
| 5.5.56-MariaDB |
+----------------+
1 row in set (0.01 sec)
```

Database Information
```
MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
+--------------------+
8 rows in set (0.00 sec)
```
