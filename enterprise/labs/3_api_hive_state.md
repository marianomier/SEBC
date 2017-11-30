```
[root@ip-172-31-63-6 ec2-user]# curl -X POST -u marianomier:mariano123 'http://localhost:7180/api/v1/clusters/Mariano/services/hive/commands/stop'
{
  "id" : 1103,
  "name" : "Stop",
  "startTime" : "2017-11-30T21:13:17.397Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}[root@ip-172-31-63-6 ec2-user]# curl -X POST -u marianomier:mariano123 'http://localhost:7180/api/v1/clusters/Mariano/services/hive/ommands/start'
{
  "id" : 1109,
  "name" : "Start",
  "startTime" : "2017-11-30T21:14:28.878Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}[root@ip-172-31-63-6 ec2-user]# curl -X POST -u marianomier:mariano123 'http://localhost:7180/api/v1/clusters/Mariano/services/hive/ommands/status'
[root@ip-172-31-63-6 ec2-user]# curl -X POST -u marianomier:mariano123 'http://localhost:7180/api/v1/clusters/Mariano/services/hive/commands/status'
[root@ip-172-31-63-6 ec2-user]# curl -u marianomier:mariano123 http://localhost:7180/api/v1/clusters/Mariano/services/hive'
> ^C
[root@ip-172-31-63-6 ec2-user]# curl -u marianomier:mariano123 'http://localhost:7180/api/v1/clusters/Mariano/services/hive'
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-63-6.ec2.internal:7180/cmf/serviceRedirect/hive",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD"
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD"
  } ],
  "configStale" : false

```
