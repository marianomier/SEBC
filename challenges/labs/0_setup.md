
[root@ip-172-31-4-213 ec2-user]# usermod -G saturn planets
Provider

<code>AWS</code>

IP Addresses

![image](https://user-images.githubusercontent.com/34034752/33489665-26679494-d67a-11e7-8f75-16dde95684a5.png)

Linux Release

![image](https://user-images.githubusercontent.com/34034752/33489794-86fb3a72-d67a-11e7-94ca-956210a0bbdb.png)

Filesystem 

![image](https://user-images.githubusercontent.com/34034752/33489822-abed1cf6-d67a-11e7-972e-02bc378ce04c.png)

Repolist

![image](https://user-images.githubusercontent.com/34034752/33489878-e36a1bde-d67a-11e7-8d03-5b07ad8b835d.png)

Users & Groups

```
[root@ip-172-31-4-213 ec2-user]# useradd -u 2800 saturn
[root@ip-172-31-4-213 ec2-user]# useradd -u 2900 haley
[root@ip-172-31-4-213 ec2-user]# groupadd comets
[root@ip-172-31-4-213 ec2-user]# groupadd planets
[root@ip-172-31-4-213 ec2-user]# usermod -G saturn planets
usermod: user 'planets' does not exist
[root@ip-172-31-4-213 ec2-user]#
[root@ip-172-31-4-213 ec2-user]# usermod -G planets saturn
[root@ip-172-31-4-213 ec2-user]# usermod -G comets haley
[root@ip-172-31-4-213 ec2-user]# id saturn
uid=2800(saturn) gid=2800(saturn) groups=2800(saturn),2902(planets)
[root@ip-172-31-4-213 ec2-user]#
[root@ip-172-31-4-213 ec2-user]# id haley
uid=2900(haley) gid=2900(haley) groups=2900(haley),2901(comets)
```



```
[root@ip-172-31-4-213 ec2-user]# cat /etc/passwd | grep saturn
saturn:x:2800:2800::/home/saturn:/bin/bash
[root@ip-172-31-4-213 ec2-user]# cat /etc/passwd | grep haley
haley:x:2900:2900::/home/haley:/bin/bash
[root@ip-172-31-4-213 ec2-user]# cat /etc/group | grep comets
comets:x:2901:haley
[root@ip-172-31-4-213 ec2-user]# cat /etc/group | grep planets
planets:x:2902:saturn

```
