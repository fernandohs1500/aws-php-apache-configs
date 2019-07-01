# aws-php-apache-configs
ebextensions for elasticbeanstalk - environment PHP

Some of my configurations to work with elasticbeanstalk in PHP environment.

# 1 - Prefork MPM

By default, Apache comes preconfigured to serve a maximum of 256 clients simultaneously. 
This particular configuration setting can be found in the file /etc/httpd/conf/httpd.conf. If you need to tuning your server to work with many connections you can do that with elasticbeanstalk extensions.

# 2 - Redirect 80 -> 443

Configuration file configures Apache for PHP environments to redirect HTTP requests on
port 80 to HTTPS on port 443 after you have configured your environment to support HTTPS
onnections.

# 3 - Timezone and other php.ini configuration

Ajust time zone to Brazil time.
Ajust max filesize
Ajust post max_size.
