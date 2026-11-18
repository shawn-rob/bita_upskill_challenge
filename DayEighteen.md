# Logs and Rotating Them #

Logs are used essentially in system administration. Unfortunately having a plethora of unnecessary logs can clog disk space, and that's why log rotation comes in.

Using logrotate to automate removing older files, saves time and the ability to focus on other tasks.

The first step is to locate the logs. In the module the logs focused on is apache. Apache logs are located in /var/log/apache2 directory . 

<!-- This pic shows what all the access and error logs are-->

As you can see, the logs append and make new backups everyday. 
I used Yaak to make http requests streamlined. It entered into the access log. After forcing the logrotation manually, it appends to access.log.1 and so on afterwards. 

<!-- This is the area for the photos of the access logs-->