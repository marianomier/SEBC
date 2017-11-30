Preinstallation Labs
                                
Checking vm.swappiness 

<code>echo "vm.swappiness = 1" >> /etc/sysctl.conf </code>

<code>echo 1 > /proc/sys/vm/swappiness</code>

![image](https://user-images.githubusercontent.com/34034752/33442178-23208068-d5ba-11e7-8f9b-08ee3f3c76b1.png)
![image](https://user-images.githubusercontent.com/34034752/33287653-f8395b8c-d37e-11e7-9cf0-06395e6622b2.png)


Mounting disks

<code>sudo lsblk -fs </code>

![image](https://user-images.githubusercontent.com/34034752/33283865-cb0dba10-d372-11e7-93f1-9d20112b22ff.png)

<code> sudo parted /dev/xvdb mklabel gpt </code>

![image](https://user-images.githubusercontent.com/34034752/33284024-3c072440-d373-11e7-9dc0-21a60e69ae28.png)

<code>sudo parted -a opt /dev/xvdb mkpart primary ext4 0% 100</code>

![image](https://user-images.githubusercontent.com/34034752/33284230-f8f9e556-d373-11e7-8366-80b7a316b2cb.png)

<code>sudo mkfs.ext4 -L datapartition /dev/xvdb</code>

![image](https://user-images.githubusercontent.com/34034752/33284493-e5b96d44-d374-11e7-8310-da9fcdf54b18.png)

<code>vi /etc/fstab </code>

/dev/xvdb               /data00                 ext4    defaults,noatime 1 2

/dev/xvdc               /data01                 ext4    defaults,noatime 1 2

![image](https://user-images.githubusercontent.com/34034752/33285186-27e7d2da-d377-11e7-9bd2-5981b3f37a12.png)

<code>sudo mount -o defaults /dev/xvdb /data00</code>

<code>sudo mount -o defaults /dev/xvdc /data01</code>

![image](https://user-images.githubusercontent.com/34034752/33285413-d84b3d92-d377-11e7-984c-541d4d6adc5d.png)

Disabling Transparent Huge Pages

<code>echo never > /sys/kernel/mm/transparent_hugepage/defrag</code>

<code>echo never > /sys/kernel/mm/transparent_hugepage/enabled</code

<code>vi /etc/rc.local</code>

Adding to rc.local

 /sys/kernel/mm/transparent_hugepage/defrag

 /sys/kernel/mm/transparent_hugepage/enabled

![image](https://user-images.githubusercontent.com/34034752/33289478-4d193a72-d385-11e7-94a8-1fe9bada68ff.png)

Network Configuration

![image](https://user-images.githubusercontent.com/34034752/33444579-4af3f6fa-d5c0-11e7-90ea-edf5c6e220d8.png)

<code>nslookup ip-172-31-63-6</code>

![image](https://user-images.githubusercontent.com/34034752/33444664-893906b2-d5c0-11e7-85fd-c547b5fe3ec8.png)

<code>dig -x 172.31.63.6</code>

![image](https://user-images.githubusercontent.com/34034752/33444753-b8f53042-d5c0-11e7-980d-56c6eedb7f72.png)

Showing ntpd service 

![image](https://user-images.githubusercontent.com/34034752/33287887-d3377aac-d37f-11e7-98ef-0847f6fd026e.png)

Installing MariaDB Database

<code>yum install mariadb-server</code>

![image](https://user-images.githubusercontent.com/34034752/33298569-b80578b0-d3ac-11e7-9baa-f298be36f69c.png)



![image](https://user-images.githubusercontent.com/34034752/33298579-c3497cda-d3ac-11e7-8cda-39302fcbff15.png)

![image](https://user-images.githubusercontent.com/34034752/33298601-e4f06e48-d3ac-11e7-92de-94e51a65ea64.png)

![image](https://user-images.githubusercontent.com/34034752/33298665-38aae400-d3ad-11e7-80f4-28013936e417.png)

![image](https://user-images.githubusercontent.com/34034752/33298894-9855831e-d3ae-11e7-9dfc-533df0c58167.png)



