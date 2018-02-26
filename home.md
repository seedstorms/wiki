<!-- TITLE: Home -->
<!-- SUBTITLE: Homepage -->

# Welcome

Welcome to the commuity wiki


```sh
#!/bin/bash -ex
yum -y update
yum -y install httpd php mysql php-mysql
chkconfig httpd on
/etc/init.d/httpd start
if [ ! -f /var/www/html/lab-app.tgz ]; then
cd /var/www/html
wget https://us-west-2-tcprod.s3.amazonaws.com/courses/AWS-100-ESS/v4.2.8/lab-1-build-a-web-server/scripts/lab-app.tgz
tar xvfz lab-app.tgz
chown apache:root /var/www/html/rds.conf.php
fi
```

1. Then this: 

`wget https://us-west-2-tcprod.s3.amazonaws.com/courses/AWS-100-ESS/v4.2.8/lab-1-build-a-web-server/scripts/lab-app.tgz
`
