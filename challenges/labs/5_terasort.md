Terasort

```

[root@ip-172-31-12-196  ec2-user]# hadoop  jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort -Dmapred.map.tasks=300 -Dmapred.reduce.tasks=150 -Dmapred.reduce.tasks.speculative.execution=false /user/saturn/tgen/terasort-input /user/saturn/tsort/terasort-exit
17/12/01 20:10:21 INFO terasort.TeraSort: starting
17/12/01 20:10:23 INFO hdfs.DFSClient: Created token for saturn: HDFS_DELEGATION_TOKEN owner=saturn@MARIANOMIER.HQ, renewer=yarn, realUser=, issueDate=1512158483191, maxDate=1512763283191, sequenceNumber=11, masterKeyId=2 on 172.31.12.196 :8020
17/12/01 20:10:23 INFO security.TokenCache: Got dt for hdfs://ip-172-31-12-196 .ec2.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.12.196 :8020, Ident: (token for saturn: HDFS_DELEGATION_TOKEN owner=saturn@MARIANOMIER.HQ, renewer=yarn, realUser=, issueDate=1512158483191, maxDate=1512763283191, sequenceNumber=11, masterKeyId=2)
17/12/01 20:10:23 INFO input.FileInputFormat: Total input paths to process : 512
Spent 537ms computing base-splits.
Spent 8ms computing TeraScheduler splits.
Computing input splits took 546ms
Sampling 10 splits of 512
Making 150 from 100000 sampled records
Computing parititions took 559ms
Spent 1107ms computing partitions.
17/12/01 20:10:24 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-12-196 .ec2.internal/172.31.12.196 :8032
17/12/01 20:10:24 INFO mapreduce.JobSubmitter: number of splits:512
17/12/01 20:10:24 INFO Configuration.deprecation: mapred.reduce.tasks.speculative.execution is deprecated. Instead, use mapreduce.reduce.speculative
17/12/01 20:10:24 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/12/01 20:10:24 INFO Configuration.deprecation: mapred.reduce.tasks is deprecated. Instead, use mapreduce.job.reduces
17/12/01 20:10:24 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1512155084552_0011
17/12/01 20:10:24 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.12.196 :8020, Ident: (token for saturn: HDFS_DELEGATION_TOKEN owner=saturn@MARIANOMIER.HQ, renewer=yarn, realUser=, issueDate=1512158483191, maxDate=1512763283191, sequenceNumber=11, masterKeyId=2)
17/12/01 20:10:25 INFO impl.YarnClientImpl: Submitted application application_1512155084552_0011
17/12/01 20:10:25 INFO mapreduce.Job: The url to track the job: http://ip-172-31-12-196 .ec2.internal:8088/proxy/application_1512155084552_0011/
17/12/01 20:10:25 INFO mapreduce.Job: Running job: job_1512155084552_0011
17/12/01 20:10:32 INFO mapreduce.Job: Job job_1512155084552_0011 running in uber mode : false
17/12/01 20:10:32 INFO mapreduce.Job:  map 0% reduce 0%
17/12/01 20:10:42 INFO mapreduce.Job:  map 1% reduce 0%
17/12/01 20:10:44 INFO mapreduce.Job:  map 2% reduce 0%
17/12/01 20:10:52 INFO mapreduce.Job:  map 5% reduce 0%
17/12/01 20:10:59 INFO mapreduce.Job:  map 6% reduce 0%
17/12/01 20:11:00 INFO mapreduce.Job:  map 7% reduce 0%
17/12/01 20:11:02 INFO mapreduce.Job:  map 8% reduce 0%
17/12/01 20:11:04 INFO mapreduce.Job:  map 9% reduce 0%
17/12/01 20:11:06 INFO mapreduce.Job:  map 10% reduce 0%
17/12/01 20:11:11 INFO mapreduce.Job:  map 11% reduce 0%
17/12/01 20:11:13 INFO mapreduce.Job:  map 12% reduce 0%
17/12/01 20:11:16 INFO mapreduce.Job:  map 13% reduce 0%
17/12/01 20:11:17 INFO mapreduce.Job:  map 14% reduce 0%
17/12/01 20:11:20 INFO mapreduce.Job:  map 15% reduce 0%
17/12/01 20:11:27 INFO mapreduce.Job:  map 16% reduce 0%
17/12/01 20:11:28 INFO mapreduce.Job:  map 17% reduce 0%
17/12/01 20:11:29 INFO mapreduce.Job:  map 19% reduce 0%
17/12/01 20:11:35 INFO mapreduce.Job:  map 20% reduce 0%
17/12/01 20:11:38 INFO mapreduce.Job:  map 21% reduce 0%
17/12/01 20:11:40 INFO mapreduce.Job:  map 22% reduce 0%
17/12/01 20:11:42 INFO mapreduce.Job:  map 23% reduce 0%
17/12/01 20:11:46 INFO mapreduce.Job:  map 24% reduce 0%
17/12/01 20:11:48 INFO mapreduce.Job:  map 25% reduce 0%
17/12/01 20:11:52 INFO mapreduce.Job:  map 26% reduce 0%
17/12/01 20:11:53 INFO mapreduce.Job:  map 27% reduce 0%
17/12/01 20:11:55 INFO mapreduce.Job:  map 28% reduce 0%
17/12/01 20:11:56 INFO mapreduce.Job:  map 29% reduce 0%
17/12/01 20:12:04 INFO mapreduce.Job:  map 30% reduce 0%
17/12/01 20:12:05 INFO mapreduce.Job:  map 31% reduce 0%
17/12/01 20:12:06 INFO mapreduce.Job:  map 32% reduce 0%
17/12/01 20:12:10 INFO mapreduce.Job:  map 33% reduce 0%
17/12/01 20:12:13 INFO mapreduce.Job:  map 34% reduce 0%
17/12/01 20:12:17 INFO mapreduce.Job:  map 36% reduce 0%
17/12/01 20:12:21 INFO mapreduce.Job:  map 37% reduce 0%
17/12/01 20:12:23 INFO mapreduce.Job:  map 38% reduce 0%
17/12/01 20:12:28 INFO mapreduce.Job:  map 40% reduce 0%
17/12/01 20:12:31 INFO mapreduce.Job:  map 41% reduce 0%
17/12/01 20:12:33 INFO mapreduce.Job:  map 42% reduce 0%
17/12/01 20:12:39 INFO mapreduce.Job:  map 43% reduce 0%
17/12/01 20:12:41 INFO mapreduce.Job:  map 44% reduce 0%
17/12/01 20:12:42 INFO mapreduce.Job:  map 45% reduce 0%
17/12/01 20:12:45 INFO mapreduce.Job:  map 46% reduce 0%
17/12/01 20:12:47 INFO mapreduce.Job:  map 47% reduce 0%
17/12/01 20:12:52 INFO mapreduce.Job:  map 48% reduce 0%
17/12/01 20:12:53 INFO mapreduce.Job:  map 49% reduce 0%
17/12/01 20:12:54 INFO mapreduce.Job:  map 50% reduce 0%
17/12/01 20:12:59 INFO mapreduce.Job:  map 51% reduce 0%
17/12/01 20:13:00 INFO mapreduce.Job:  map 52% reduce 0%
17/12/01 20:13:04 INFO mapreduce.Job:  map 53% reduce 0%
17/12/01 20:13:05 INFO mapreduce.Job:  map 54% reduce 0%
17/12/01 20:13:09 INFO mapreduce.Job:  map 55% reduce 0%
17/12/01 20:13:14 INFO mapreduce.Job:  map 56% reduce 0%
17/12/01 20:13:17 INFO mapreduce.Job:  map 57% reduce 0%
17/12/01 20:13:18 INFO mapreduce.Job:  map 58% reduce 0%
17/12/01 20:13:19 INFO mapreduce.Job:  map 59% reduce 0%
17/12/01 20:13:21 INFO mapreduce.Job:  map 60% reduce 0%
17/12/01 20:13:27 INFO mapreduce.Job:  map 61% reduce 0%
17/12/01 20:13:28 INFO mapreduce.Job:  map 62% reduce 0%
17/12/01 20:13:29 INFO mapreduce.Job:  map 63% reduce 0%
17/12/01 20:13:33 INFO mapreduce.Job:  map 64% reduce 0%
17/12/01 20:13:35 INFO mapreduce.Job:  map 65% reduce 0%
17/12/01 20:13:42 INFO mapreduce.Job:  map 66% reduce 0%
17/12/01 20:13:43 INFO mapreduce.Job:  map 68% reduce 0%
17/12/01 20:13:46 INFO mapreduce.Job:  map 69% reduce 0%
17/12/01 20:13:49 INFO mapreduce.Job:  map 70% reduce 0%
17/12/01 20:13:54 INFO mapreduce.Job:  map 71% reduce 0%
17/12/01 20:13:55 INFO mapreduce.Job:  map 72% reduce 0%
17/12/01 20:13:56 INFO mapreduce.Job:  map 73% reduce 0%
17/12/01 20:14:00 INFO mapreduce.Job:  map 74% reduce 0%
17/12/01 20:14:03 INFO mapreduce.Job:  map 75% reduce 0%
17/12/01 20:14:06 INFO mapreduce.Job:  map 76% reduce 0%
17/12/01 20:14:07 INFO mapreduce.Job:  map 77% reduce 0%
17/12/01 20:14:10 INFO mapreduce.Job:  map 78% reduce 0%
17/12/01 20:14:13 INFO mapreduce.Job:  map 79% reduce 0%
17/12/01 20:14:18 INFO mapreduce.Job:  map 80% reduce 0%
17/12/01 20:14:19 INFO mapreduce.Job:  map 81% reduce 0%
17/12/01 20:14:20 INFO mapreduce.Job:  map 82% reduce 0%
17/12/01 20:14:25 INFO mapreduce.Job:  map 83% reduce 0%
17/12/01 20:14:27 INFO mapreduce.Job:  map 84% reduce 0%
17/12/01 20:14:30 INFO mapreduce.Job:  map 85% reduce 0%
17/12/01 20:14:35 INFO mapreduce.Job:  map 85% reduce 1%
17/12/01 20:14:36 INFO mapreduce.Job:  map 85% reduce 2%
17/12/01 20:14:38 INFO mapreduce.Job:  map 86% reduce 2%
17/12/01 20:14:39 INFO mapreduce.Job:  map 87% reduce 2%
17/12/01 20:14:45 INFO mapreduce.Job:  map 88% reduce 2%
17/12/01 20:14:50 INFO mapreduce.Job:  map 89% reduce 2%
17/12/01 20:14:54 INFO mapreduce.Job:  map 90% reduce 2%
17/12/01 20:14:56 INFO mapreduce.Job:  map 91% reduce 2%
17/12/01 20:15:01 INFO mapreduce.Job:  map 92% reduce 2%
17/12/01 20:15:06 INFO mapreduce.Job:  map 93% reduce 2%
17/12/01 20:15:11 INFO mapreduce.Job:  map 94% reduce 2%
17/12/01 20:15:16 INFO mapreduce.Job:  map 95% reduce 2%
17/12/01 20:15:18 INFO mapreduce.Job:  map 96% reduce 2%
17/12/01 20:15:24 INFO mapreduce.Job:  map 97% reduce 2%
17/12/01 20:15:27 INFO mapreduce.Job:  map 98% reduce 2%
17/12/01 20:15:32 INFO mapreduce.Job:  map 99% reduce 2%
17/12/01 20:15:34 INFO mapreduce.Job:  map 100% reduce 2%
17/12/01 20:15:42 INFO mapreduce.Job:  map 100% reduce 3%
17/12/01 20:15:43 INFO mapreduce.Job:  map 100% reduce 6%
17/12/01 20:15:44 INFO mapreduce.Job:  map 100% reduce 7%
17/12/01 20:15:47 INFO mapreduce.Job:  map 100% reduce 9%
17/12/01 20:15:50 INFO mapreduce.Job:  map 100% reduce 10%
17/12/01 20:15:52 INFO mapreduce.Job:  map 100% reduce 11%
17/12/01 20:15:53 INFO mapreduce.Job:  map 100% reduce 12%
17/12/01 20:15:55 INFO mapreduce.Job:  map 100% reduce 13%
17/12/01 20:15:56 INFO mapreduce.Job:  map 100% reduce 14%
17/12/01 20:15:58 INFO mapreduce.Job:  map 100% reduce 15%
17/12/01 20:15:59 INFO mapreduce.Job:  map 100% reduce 16%
17/12/01 20:16:00 INFO mapreduce.Job:  map 100% reduce 17%
17/12/01 20:16:01 INFO mapreduce.Job:  map 100% reduce 18%
17/12/01 20:16:04 INFO mapreduce.Job:  map 100% reduce 19%
17/12/01 20:16:05 INFO mapreduce.Job:  map 100% reduce 20%
17/12/01 20:16:07 INFO mapreduce.Job:  map 100% reduce 21%
17/12/01 20:16:08 INFO mapreduce.Job:  map 100% reduce 22%
17/12/01 20:16:09 INFO mapreduce.Job:  map 100% reduce 23%
17/12/01 20:16:10 INFO mapreduce.Job:  map 100% reduce 24%
17/12/01 20:16:11 INFO mapreduce.Job:  map 100% reduce 25%
17/12/01 20:16:12 INFO mapreduce.Job:  map 100% reduce 26%
17/12/01 20:16:15 INFO mapreduce.Job:  map 100% reduce 27%
17/12/01 20:16:16 INFO mapreduce.Job:  map 100% reduce 28%
17/12/01 20:16:17 INFO mapreduce.Job:  map 100% reduce 29%
17/12/01 20:16:18 INFO mapreduce.Job:  map 100% reduce 30%
17/12/01 20:16:20 INFO mapreduce.Job:  map 100% reduce 31%
17/12/01 20:16:22 INFO mapreduce.Job:  map 100% reduce 32%
17/12/01 20:16:24 INFO mapreduce.Job:  map 100% reduce 33%
17/12/01 20:16:26 INFO mapreduce.Job:  map 100% reduce 34%
17/12/01 20:16:27 INFO mapreduce.Job:  map 100% reduce 35%
17/12/01 20:16:28 INFO mapreduce.Job:  map 100% reduce 37%
17/12/01 20:16:29 INFO mapreduce.Job:  map 100% reduce 38%
17/12/01 20:16:30 INFO mapreduce.Job:  map 100% reduce 39%
17/12/01 20:16:31 INFO mapreduce.Job:  map 100% reduce 40%
17/12/01 20:16:34 INFO mapreduce.Job:  map 100% reduce 41%
17/12/01 20:16:36 INFO mapreduce.Job:  map 100% reduce 42%
17/12/01 20:16:37 INFO mapreduce.Job:  map 100% reduce 43%
17/12/01 20:16:40 INFO mapreduce.Job:  map 100% reduce 44%
17/12/01 20:16:43 INFO mapreduce.Job:  map 100% reduce 46%
17/12/01 20:16:44 INFO mapreduce.Job:  map 100% reduce 47%
17/12/01 20:16:45 INFO mapreduce.Job:  map 100% reduce 48%
17/12/01 20:16:46 INFO mapreduce.Job:  map 100% reduce 51%
17/12/01 20:16:47 INFO mapreduce.Job:  map 100% reduce 52%
17/12/01 20:16:48 INFO mapreduce.Job:  map 100% reduce 53%
17/12/01 20:16:49 INFO mapreduce.Job:  map 100% reduce 54%
17/12/01 20:16:55 INFO mapreduce.Job:  map 100% reduce 55%
17/12/01 20:16:57 INFO mapreduce.Job:  map 100% reduce 56%
17/12/01 20:16:58 INFO mapreduce.Job:  map 100% reduce 57%
17/12/01 20:17:00 INFO mapreduce.Job:  map 100% reduce 58%
17/12/01 20:17:01 INFO mapreduce.Job:  map 100% reduce 60%
17/12/01 20:17:02 INFO mapreduce.Job:  map 100% reduce 63%
17/12/01 20:17:03 INFO mapreduce.Job:  map 100% reduce 65%
17/12/01 20:17:07 INFO mapreduce.Job:  map 100% reduce 66%
17/12/01 20:17:08 INFO mapreduce.Job:  map 100% reduce 67%
17/12/01 20:17:15 INFO mapreduce.Job:  map 100% reduce 69%
17/12/01 20:17:17 INFO mapreduce.Job:  map 100% reduce 71%
17/12/01 20:17:18 INFO mapreduce.Job:  map 100% reduce 73%
17/12/01 20:17:19 INFO mapreduce.Job:  map 100% reduce 76%
17/12/01 20:17:20 INFO mapreduce.Job:  map 100% reduce 77%
17/12/01 20:17:21 INFO mapreduce.Job:  map 100% reduce 78%
17/12/01 20:17:22 INFO mapreduce.Job:  map 100% reduce 79%
17/12/01 20:17:29 INFO mapreduce.Job:  map 100% reduce 80%
17/12/01 20:17:30 INFO mapreduce.Job:  map 100% reduce 81%
17/12/01 20:17:32 INFO mapreduce.Job:  map 100% reduce 82%
17/12/01 20:17:33 INFO mapreduce.Job:  map 100% reduce 83%
17/12/01 20:17:34 INFO mapreduce.Job:  map 100% reduce 86%
17/12/01 20:17:35 INFO mapreduce.Job:  map 100% reduce 88%
17/12/01 20:17:36 INFO mapreduce.Job:  map 100% reduce 90%
17/12/01 20:17:39 INFO mapreduce.Job:  map 100% reduce 91%
17/12/01 20:17:40 INFO mapreduce.Job:  map 100% reduce 92%
17/12/01 20:17:45 INFO mapreduce.Job:  map 100% reduce 96%
17/12/01 20:17:46 INFO mapreduce.Job:  map 100% reduce 100%
17/12/01 20:17:47 INFO mapreduce.Job: Job job_1512155084552_0011 completed successfully
17/12/01 20:17:47 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=2904180754
                FILE: Number of bytes written=5836792659
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553677312
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=1986
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=300
        Job Counters
                Launched map tasks=512
                Launched reduce tasks=150
                Data-local map tasks=512
                Total time spent by all maps in occupied slots (ms)=4091676
                Total time spent by all reduces in occupied slots (ms)=2856396
                Total time spent by all map tasks (ms)=4091676
                Total time spent by all reduce tasks (ms)=2856396
                Total vcore-seconds taken by all map tasks=4091676
                Total vcore-seconds taken by all reduce tasks=2856396
                Total megabyte-seconds taken by all map tasks=4189876224
                Total megabyte-seconds taken by all reduce tasks=2924949504
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2848454951
                Input split bytes=77312
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2848454951
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =76800
                Failed Shuffles=0
                Merged Map outputs=76800
                GC time elapsed (ms)=56275
                CPU time spent (ms)=2428630
                Physical memory (bytes) snapshot=310924087296
                Virtual memory (bytes) snapshot=1062156935168
                Total committed heap usage (bytes)=338575228928
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=6553600000
        File Output Format Counters
                Bytes Written=6553600000
17/12/01 20:17:47 INFO terasort.TeraSort: done
[root@ip-172-31-12-196  ec2-user]# hadoop  jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort -Dmapred.map.tasks=300 -Dmapred.reduce.tasks=150 -Dmapred.reduce.tasks.speculative.execution=false /user/saturn/tgen/terasort-input /user/saturn/tsort/terasort-exitreduce.tasks.speculative.execution=false /user/saturn/tg  
```

