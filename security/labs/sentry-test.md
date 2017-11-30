
```
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20171129232222_eae94826-7e0c-416c-90ac-039d8fc69aaf): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171129232222_eae94826-7e0c-416c-90ac-039d8fc69aaf); Time taken: 0.58 seconds
INFO  : Executing command(queryId=hive_20171129232222_eae94826-7e0c-416c-90ac-039d8fc69aaf): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129232222_eae94826-7e0c-416c-90ac-039d8fc69aaf); Time taken: 0.072 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (2.035 seconds)



0: jdbc:hive2://ip-172-31-48-156:10000/defaul> CREATE ROLE chingon;
INFO  : Compiling command(queryId=hive_20171129234040_327571b3-88b0-46db-9e70-ac7b8592914a): CREATE ROLE chingon
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129234040_327571b3-88b0-46db-9e70-ac7b8592914a); Time taken: 0.078 seconds
INFO  : Executing command(queryId=hive_20171129234040_327571b3-88b0-46db-9e70-ac7b8592914a): CREATE ROLE chingon
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129234040_327571b3-88b0-46db-9e70-ac7b8592914a); Time taken: 0.496 seconds
INFO  : OK
No rows affected (0.59 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> GRANT ALL ON SERVER server1 to role chingon;
INFO  : Compiling command(queryId=hive_20171129234141_3443f53f-d6c6-44e8-ae77-7f3dd590bb7b): GRANT ALL ON SERVER server1 to role chingon
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129234141_3443f53f-d6c6-44e8-ae77-7f3dd590bb7b); Time taken: 0.095 seconds
INFO  : Executing command(queryId=hive_20171129234141_3443f53f-d6c6-44e8-ae77-7f3dd590bb7b): GRANT ALL ON SERVER server1 to role chingon
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129234141_3443f53f-d6c6-44e8-ae77-7f3dd590bb7b); Time taken: 0.074 seconds
INFO  : OK
No rows affected (0.184 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> grant role chingon to group chingon;
INFO  : Compiling command(queryId=hive_20171129234141_2876464d-7e77-4fa4-8f3d-4b0eaa0c6144): grant role chingon to group chingon
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129234141_2876464d-7e77-4fa4-8f3d-4b0eaa0c6144); Time taken: 0.09 seconds
INFO  : Executing command(queryId=hive_20171129234141_2876464d-7e77-4fa4-8f3d-4b0eaa0c6144): grant role chingon to group chingon
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129234141_2876464d-7e77-4fa4-8f3d-4b0eaa0c6144); Time taken: 0.065 seconds
INFO  : OK
No rows affected (0.171 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> show tables;
INFO  : Compiling command(queryId=hive_20171129234141_2138cedd-3dea-4196-8c9b-13c375106850): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171129234141_2138cedd-3dea-4196-8c9b-13c375106850); Time taken: 0.069 seconds
INFO  : Executing command(queryId=hive_20171129234141_2138cedd-3dea-4196-8c9b-13c375106850): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129234141_2138cedd-3dea-4196-8c9b-13c375106850); Time taken: 0.203 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.335 seconds)

[root@ip-172-31-63-6 ~]# sudo groupadd selector
[root@ip-172-31-63-6 ~]# sudo groupadd inserters
[root@ip-172-31-63-6 ~]# sudo useradd -u 1100 -g selector george
[root@ip-172-31-63-6 ~]# sudo useradd -u 1200 -g inserters ferdinand
[root@ip-172-31-63-6 ~]# kadmin.local
Authenticating as principal marianomier/admin@MARIANO.COM with password.
kadmin.local:  add_principal george
WARNING: no policy specified for george@MARIANO.COM; defaulting to no policy
Enter password for principal "george@MARIANO.COM":
Re-enter password for principal "george@MARIANO.COM":
Principal "george@MARIANO.COM" created.
kadmin.local:  kadmin.local: add_principal ferdinand
kadmin.local: Unknown request "kadmin.local:".  Type "?" for a request list.
kadmin.local:  add_principal ferdinand
WARNING: no policy specified for ferdinand@MARIANO.COM; defaulting to no policy
Enter password for principal "ferdinand@MARIANO.COM":
Re-enter password for principal "ferdinand@MARIANO.COM":
Principal "ferdinand@MARIANO.COM" created.
kadmin.local:


0: jdbc:hive2://ip-172-31-48-156:10000/defaul> CREATE ROLE reads;
INFO  : Compiling command(queryId=hive_20171129234949_8f7b1faf-c024-49bd-8343-186cb59c2c20): CREATE ROLE reads
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129234949_8f7b1faf-c024-49bd-8343-186cb59c2c20); Time taken: 0.058 seconds
INFO  : Executing command(queryId=hive_20171129234949_8f7b1faf-c024-49bd-8343-186cb59c2c20): CREATE ROLE reads
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129234949_8f7b1faf-c024-49bd-8343-186cb59c2c20); Time taken: 0.041 seconds
INFO  : OK
No rows affected (0.115 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> CREATE ROLE writes;
INFO  : Compiling command(queryId=hive_20171129234949_001ee6bf-bb9d-4306-ba38-2320721b39f2): CREATE ROLE writes

INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129234949_001ee6bf-bb9d-4306-ba38-2320721b39f2); Time taken: 0.058 seconds
INFO  : Executing command(queryId=hive_20171129234949_001ee6bf-bb9d-4306-ba38-2320721b39f2): CREATE ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129234949_001ee6bf-bb9d-4306-ba38-2320721b39f2); Time taken: 0.026 seconds
INFO  : OK
No rows affected (0.098 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> GRANT SELECT ON DATABASE default TO ROLE reads;

INFO  : Compiling command(queryId=hive_20171129235050_13fdd325-80b9-4cb9-8317-f69eedccff44): GRANT SELECT ON DATABASE default TO ROLE reads
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129235050_13fdd325-80b9-4cb9-8317-f69eedccff44); Time taken: 0.063 seconds
INFO  : Executing command(queryId=hive_20171129235050_13fdd325-80b9-4cb9-8317-f69eedccff44): GRANT SELECT ON DATABASE default TO ROLE reads
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129235050_13fdd325-80b9-4cb9-8317-f69eedccff44); Time taken: 0.031 seconds
INFO  : OK
No rows affected (0.108 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> GRANT ROLE reads TO GROUP selector;
INFO  : Compiling command(queryId=hive_20171129235050_8851d49f-c8b8-4f21-a079-47449269f59c): GRANT ROLE reads TO GROUP selector
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129235050_8851d49f-c8b8-4f21-a079-47449269f59c); Time taken: 0.057 seconds
INFO  : Executing command(queryId=hive_20171129235050_8851d49f-c8b8-4f21-a079-47449269f59c): GRANT ROLE reads TO GROUP selector
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129235050_8851d49f-c8b8-4f21-a079-47449269f59c); Time taken: 0.027 seconds
INFO  : OK
No rows affected (0.099 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> REVOKE ALL ON DATABASE default FROM ROLE writes;
INFO  : Compiling command(queryId=hive_20171129235050_c1d697cb-908a-4df7-a152-3876853dbedb): REVOKE ALL ON DATABASE default FROM ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129235050_c1d697cb-908a-4df7-a152-3876853dbedb); Time taken: 0.059 seconds
INFO  : Executing command(queryId=hive_20171129235050_c1d697cb-908a-4df7-a152-3876853dbedb): REVOKE ALL ON DATABASE default FROM ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129235050_c1d697cb-908a-4df7-a152-3876853dbedb); Time taken: 0.082 seconds
INFO  : OK
No rows affected (0.155 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> GRANT SELECT ON default.sample_07 TO ROLE writes;
INFO  : Compiling command(queryId=hive_20171129235151_1c29340e-4c84-424d-957e-8e55c8fdc932): GRANT SELECT ON default.sample_07 TO ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129235151_1c29340e-4c84-424d-957e-8e55c8fdc932); Time taken: 0.06 seconds
INFO  : Executing command(queryId=hive_20171129235151_1c29340e-4c84-424d-957e-8e55c8fdc932): GRANT SELECT ON default.sample_07 TO ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129235151_1c29340e-4c84-424d-957e-8e55c8fdc932); Time taken: 0.031 seconds
INFO  : OK
No rows affected (0.104 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> GRANT ROLE writes TO GROUP inserters;
INFO  : Compiling command(queryId=hive_20171129235151_e59b0b66-557c-4b50-b5c9-e0bfde1a695c): GRANT ROLE writes TO GROUP inserters
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20171129235151_e59b0b66-557c-4b50-b5c9-e0bfde1a695c); Time taken: 0.055 seconds
INFO  : Executing command(queryId=hive_20171129235151_e59b0b66-557c-4b50-b5c9-e0bfde1a695c): GRANT ROLE writes TO GROUP inserters
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171129235151_e59b0b66-557c-4b50-b5c9-e0bfde1a695c); Time taken: 0.027 seconds
INFO  : OK
No rows affected (0.096 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul>


[root@ip-172-31-63-6 ~]# kadmin.local

Authenticating as principal marianomier/admin@MARIANO.COM with password.
kadmin.local:  xst -norandkey -k george.keytab george
Entry for principal george with kvno 1, encryption type aes256-cts-hmac-sha1-96 added to keytab WRFILE:george.keytab.
Entry for principal george with kvno 1, encryption type aes128-cts-hmac-sha1-96 added to keytab WRFILE:george.keytab.
Entry for principal george with kvno 1, encryption type des3-cbc-sha1 added to keytab WRFILE:george.keytab.
Entry for principal george with kvno 1, encryption type arcfour-hmac added to keytab WRFILE:george.keytab.
Entry for principal george with kvno 1, encryption type camellia256-cts-cmac added to keytab WRFILE:george.keytab.
Entry for principal george with kvno 1, encryption type camellia128-cts-cmac added to keytab WRFILE:george.keytab.
Entry for principal george with kvno 1, encryption type des-hmac-sha1 added to keytab WRFILE:george.keytab.
Entry for principal george with kvno 1, encryption type des-cbc-md5 added to keytab WRFILE:george.keytab.
kadmin.local:  exit

[root@ip-172-31-63-6 ~]# ls
anaconda-ks.cfg  george.keytab  marianomier.keytab  oracle-j2sdk1.7-1.7.0+update67-1.x86_64.rpm  original-ks.cfg
[root@ip-172-31-63-6 ~]# kinit -k -t george.keytab george@MARIANO.COM
[root@ip-172-31-63-6 ~]#

[root@ip-172-31-63-6 ~]# klist
Ticket cache: FILE:/tmp/krb5cc_0
Default principal: george@MARIANO.COM

Valid starting       Expires              Service principal
11/29/2017 23:56:59  11/30/2017 23:56:59  krbtgt/MARIANO.COM@MARIANO.COM
        renew until 12/06/2017 23:56:59
[root@ip-172-31-63-6 ~]# beeline
Beeline version 1.1.0-cdh5.10.2 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-48-156:10000/default;principal=hive/ip-172-31-48-156.ec2.internal@MARIANO.COM
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-48-156:10000/default;principal=hive/ip-172-31-48-156.ec2.internal@MARIANO.COM
Connected to: Apache Hive (version 1.1.0-cdh5.10.2)
Driver: Hive JDBC (version 1.1.0-cdh5.10.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> show tables;
INFO  : Compiling command(queryId=hive_20171130002323_6f349ab0-15bc-4550-a81e-e639a244dabd): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171130002323_6f349ab0-15bc-4550-a81e-e639a244dabd); Time taken: 0.066 seconds
INFO  : Executing command(queryId=hive_20171130002323_6f349ab0-15bc-4550-a81e-e639a244dabd): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171130002323_6f349ab0-15bc-4550-a81e-e639a244dabd); Time taken: 0.142 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.303 seconds)
0: jdbc:hive2://ip-172-31-48-156:10000/defaul>

Authenticating as principal george/admin@MARIANO.COM with password.
kadmin.local:  xst -norandkey -k ferdinand.keytab ferdinand
Entry for principal ferdinand with kvno 1, encryption type aes256-cts-hmac-sha1-96 added to keytab WRFILE:ferdinand.keytab.
Entry for principal ferdinand with kvno 1, encryption type aes128-cts-hmac-sha1-96 added to keytab WRFILE:ferdinand.keytab.
Entry for principal ferdinand with kvno 1, encryption type des3-cbc-sha1 added to keytab WRFILE:ferdinand.keytab.
Entry for principal ferdinand with kvno 1, encryption type arcfour-hmac added to keytab WRFILE:ferdinand.keytab.
Entry for principal ferdinand with kvno 1, encryption type camellia256-cts-cmac added to keytab WRFILE:ferdinand.keytab.
Entry for principal ferdinand with kvno 1, encryption type camellia128-cts-cmac added to keytab WRFILE:ferdinand.keytab.
Entry for principal ferdinand with kvno 1, encryption type des-hmac-sha1 added to keytab WRFILE:ferdinand.keytab.
Entry for principal ferdinand with kvno 1, encryption type des-cbc-md5 added to keytab WRFILE:ferdinand.keytab.

[root@ip-172-31-63-6 ~]# kinit -k -t ferdinand.keytab ferdinand@MARIANO.COM
[root@ip-172-31-63-6 ~]# klist
Ticket cache: FILE:/tmp/krb5cc_0
Default principal: ferdinand@MARIANO.COM

Valid starting       Expires              Service principal
11/30/2017 00:33:00  12/01/2017 00:33:00  krbtgt/MARIANO.COM@MARIANO.COM
        renew until 12/07/2017 00:33:00
[root@ip-172-31-63-6 ~]#

[root@ip-172-31-63-6 ~]# beeline
Beeline version 1.1.0-cdh5.10.2 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-48-156:10000/default;principal=hive/ip-172-31-48-156.ec2.internal@MARIANO.COM
scan complete in 1ms
Connecting to jdbc:hive2://ip-172-31-48-156:10000/default;principal=hive/ip-172-31-48-156.ec2.internal@MARIANO.COM
Connected to: Apache Hive (version 1.1.0-cdh5.10.2)
Driver: Hive JDBC (version 1.1.0-cdh5.10.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-48-156:10000/defaul> show tables;
INFO  : Compiling command(queryId=hive_20171130003434_599c3ef4-88d2-4b24-943d-5484b1158676): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171130003434_599c3ef4-88d2-4b24-943d-5484b1158676); Time taken: 0.067 seconds
INFO  : Executing command(queryId=hive_20171130003434_599c3ef4-88d2-4b24-943d-5484b1158676): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171130003434_599c3ef4-88d2-4b24-943d-5484b1158676); Time taken: 0.143 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (0.306 seconds)


```
