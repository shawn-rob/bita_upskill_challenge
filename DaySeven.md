# What Else Can I Do? - The Server and Its Services #

## Installing a web server ## 

Today I am installing Apache2 web server. Apache2 is a Hyper Text Transport Protocol Daemon. What that means is it a server for a website's stored files. It in turns packages all the files into the user interfaced webpage.

Using systemctl status apache2 wil tell you the status of the server. It is currently active.

Doing sudo systemctl start or stop apache2 turns the server on or off. The default page tells you that you are indeed in the right place. Turning apache2 off creates an error when attempting to connect. 

I switched up the page with a simple html page with a couple lines.

