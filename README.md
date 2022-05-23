# IT_system_test
**Implement a basic web application infrastructure using Docker**

The basic configuration of docker is:
1) Nginx Reverse Proxy 
2) PHP version 7.4 through FPM 
3) MariaDB version 10.6  
4) Redis server

### Requirment
1) Installing docker 20.10.14 to up
2) Altering Ip 127.0.0.1 in the host files to myservice.local following this directory /etc/hosts in linux OS or C:\Windows\System32\drivers\etc\hosts in windows OS such as below:

```
#localhost is used to configure the loopback interface
when the system is booting.  Do not change this entry.

127.0.0.1	localhost
127.0.0.1 myservice.local
```
### Executing program
First, Git clone this code to your machine running Docker(it is nessery to rub docker befor these steps):
```
git clone https://github.com/zahra4fact/IT_system_test.git
cd IT_system_test
```
secondly, run this code to read docker-compose.yml file
```
docker-compose up
```

Now you can acsses to run the compose file and display the PHPInfo page just typing https://myservice.local on the local browser.
Don't forget to clean up after you're done!
```
docker-compose down
```
