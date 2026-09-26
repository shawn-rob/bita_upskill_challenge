# Day Three: New User #

Day three is where I am having a field day in trying to figure this out. I was attempting to make a new user, and i believe I did successfully but when trying to login to the sudo user i get an access denied. 

I am currently trying to redo the process and I get a warn: waiting for lock to become available. I think I didn't finish installing the new user before it timed out. Doing this at work. Did a reset of the server back to the default without destroying it altogether. I finally got it. I have number 1 'Kungfu' taking the forefront. Thank goodness this isn't live at work environment. 

The thing that took me forever to do though was get the ssh key login for Kungfu and so I would get an access denied. It took a bit of googling but I was able to get my new created user to login via ssh. I changed the PW for the user I should do the same for the root. I switched from Kungfu to root with sudo -i successfully and changed the name of the server successfully.

## UPDATE ##

Did not know that there was assessments, so here I am back again. 