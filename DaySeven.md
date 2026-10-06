# What Else Can I Do? - The Server and Its Services #

## Installing a web server ## 

Today I am installing Apache2 web server. Apache2 is a Hyper Text Transport Protocol Daemon. What that means is it a server for a website's stored files. It in turns packages all the files into the user interfaced webpage.

Using systemctl status apache2 wil tell you the status of the server. It is currently active.

Doing sudo systemctl start or stop apache2 turns the server on or off. The default page tells you that you are indeed in the right place. Turning apache2 off creates an error when attempting to connect. 

I switched up the page with a simple html page with a couple lines.

***

#### The Access File ####

In the access file, it shows all the times an ip accesses the site. I refreshed the site while on and off the vpn to see if it coincides with the times and ip in the access files. There is more about access files in day 8.

***
### Break and Restore Web Server Challenge ### 

In this challenge, there is a server that is failing to connect to the local host. 

Using **systemctl status Nginx**, the status seems to be failed. In the errors this was shown ***Oct 01 21:27:37 ip-10-1-13-96 nginx[569]: nginx: [emerg] unexpected ";" in /etc/nginx/sites-enabled/default***.
There is indeed a semicolon in the default. I remove that. There are still issues. In the scenario it states too many files running at the same time in the error logs. Commenting out the **LIMITNOFILE**, restarting the system after reloading the daemon is now OK and running the server. 

Curl transfers data to and from servers, and is used to test and debug web content.