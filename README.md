# LinuxServerConfiguration

## IP and SSH  
The project is at IP address 35.165.77.203, and the ssh port is 2200  

## URL  
The URL is simply the IP address  

## Software installed   
I installed python's pip, flask, and sqlalchemy modules. As well as apache2, and the wsgi-mod.  
I configured the wsgi mod's .conf file, made a new user (with sudo privileges), created an ssh  
key for the user, and configured the firewall.  

## Third Party Resources  
The only Third Party resources used for this project were Google searches, and various Stack  
Overflow, and Ubuntu articles used for troubleshooting, and debugging.

## Configuration  
To configure the server, I added the new user, and gave it sudo privilege.  
Then I created an ssh key for the new user. Next was configuring the ufw,  
configuring default settings for incoming and outgoing, selecting the ports  
on which I wanted it listen, and activating it. After that was configuring  
apache2, which included altering the 000-default.conf file in the sites-enabled  
directory, to send web requests to the file I'd written, instead of the default  
apache file. Finally, I cloned a copy of my categories project into the server,  
set it up to host the database, and debugged the inevitable issues.
