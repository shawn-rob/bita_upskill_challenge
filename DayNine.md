# Day Nine #
## Diving Into Netwrking ##

I did a little readover on the objectives of this module and did a bit of day 9 on day 8. Insert Prince meme lol. Getting ahead of yourself.

This day is about open ports and firewalls. 

##

### Which Ports Are Open? ###

According to the Nmap, I currently have three ports open: 22, 80, and 9090. I don't know of the zeus-admin service that is running on tcp/9090. **UPDATE** The 9090 is the Ubuntu web console.

Funny story: I went to ny browser to find out what the 9090 port takes me to. Nothing was loading. Gateway errors, time outs, etc kept happening. I check my wifi, I'm not on the VPN am I? Yes on the browser lol. The firewall is definitely working. 

But I realized it works too well cause now, if I want to login with my phone, but it's not connected to the wifi, or login with a vpn, then I'd be stuck pretty much so I think it needs to get changed up a bit.

I removed the rule from the ufw only allowing my wifi's ip address. I still was having the issue to where I couldn't login through
other ip addresses like with my phone. 

So I flushed the iptables as I thought that would get rid of  the rule I put on the firewall, but egads!

I locked myself out of the server essentially. Luckily there is a recovery console. I disabled the ufw and applied the rule to allow ssh logins and deny html logins and I am now able to login with my vpn. 
But I am unable to view my server on the browser when putting in the IP.
When I reenable I still had the same issue. The problem was that the 9090 port was not in the firewall rules. 

## **Security Inventory** ##

| Port | Protocol | Service | Process | Intentionally Exposed? |
| :----: | :----: | :-----: | :-----: | :-----: |
| 22 | tcp | ssh | sshd-session | yes |
| 80 | tcp | http | apache2 | yes |
| 9090 | tcp | zeus-admin | * | yes |
