# Day 8: grep and other text processors #

In this day's module I began with learning more about less and how to use commands to navigate through the file. The file in particular is that access log. I used **head** and **tail** to see the first and last lines in the file. 
Tail -f will show you in real time any changes. I used a browser vpn to see the ip added at every refresh.

## Auth.log Authentaction Results ##

In this /var/log/auth.log file there are many attackers! In my attacker.txt file, I have almost 360 separate IPs that attempted to login. 

Using ufw (an uncomplicated firewall), I can no longer log in by using my vpn. I feel a lot more secure.

I checked the tail of the auth log. Looks like the ninja is the only one attemped to login since the firewall was installed.