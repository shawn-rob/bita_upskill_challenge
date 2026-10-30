# New User, Who Dis? #

## Users and Groups Assessment ##

We're rolling now. In this module I am creating new users and groups. I created two users: **keem** and **schoolboyq**. Since I started without documenting, I will add a new user. 
 Using ***sudo adduser***, I added Sza to the mix. 

 <!-- 
 Insert img about the users
 -->

 There are four groups: sudo, users, groups, _ssh. All the users are in the users groups. The user kungfu is the only _ssh user. When attempting to log in with any other users, it errors. Only kungfu is able to login to ssh. There are only two sudo users: kungfu and schoolboyq. Also keem and schoolboyq are the current users in developer. keem doesn't have full sudo, but is about to sudo reboot.

 ---

 ### Credential Databases ###

 * /etc/passwd <br> 
    * Contains user account information. Does not contain passwords despite the name. 
    * (kungfu - UID 1001 - dir /home/kungfu: bin/bash)
    * Can be viewed by all users
    <br>

* /etc/shadow <br>
    * Stores passwords for the users in a hashed format.
    * Can only be read by sudo users (kungfu, schoolboyq)


* /etc/group <br>
    * Lists the groups and users listed with the groups

    ----

    ## Practical Challenge ##

    Sza is the current employee who now has the ability to check the server, the available disk space, and the ability to reboot the server without full root privilege. 
    <!-- 
    Insert screenshot of sza new permissions here
    -->