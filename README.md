# Web Hosting By Apache Httpd

## Install Apache Httpd in your system 

```
root@jarvis:~# yum install httpd -y
```

## Start and enable Apache Httpd

```
root@jarvis:~# systemctl enable --now httpd 
```
Now for checking that httpd server is working or not , type your ip in browser <br> and if you see this page then your httpd is working !!

![httpd](httpd.png)

## Now for hosting a web page on your server 
### change directory to /var/www/html

Now open any text editor like vim , nano and write your html code under ``` "index.html"  ```

## Configuration of Httpd

The main configuration file of httpd is ``` /etc/httpd/conf/httpd.conf ``` 


### To change document root , edit in httpd.conf 
``` 
<Directory "/var/www/html">
   
```
### Restart httpd service
```
root@jarvis:~# systemctl restart httpd
```
### To check status of httpd 
```
root@jarvis:~# systemctl status httpd
```

