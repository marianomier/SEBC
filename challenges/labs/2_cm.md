Repo

```
[root@ip-172-31-12-196 ec2-user]# ls /etc/yum.repos.d
Cloudera-manager.repo  redhat.repo  redhat-rhui-client-config.repo  redhat-rhui.repo  rhui-load-balancers.conf

```

db.properties

```
[root@ip-172-31-12-196 ec2-user]# /usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-4-213.ec2.internal -utemp -ptemp --scm-host ip-172-31-12-196.ec2.internal scm scm scm_password
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
[                          main] DbCommandExecutor              INFO  Successfully connected to database.
All done, your SCM database is configured correctly!
[root@ip-172-31-12-196 ec2-user]#
```
