SM Networks is a network solutions company primarily having 2 LANs.

Given Network Information
-------------------------------
IPv4:	172.16.0.0/20


User LAN has 520 Hosts whereas Server LAN has 12 hosts.

IPv4
-----
Subnet the given network and assign the first usable subnet to User LAN while wasting the fewest addresses.
Subnet further the third usable subnet and assign the fourth usable subnet to Server LAN.
- IPv4 gateway for both User and Server LAN should use the last usable IP address of the corresponding subnet.
- Assign the 1st usable IP address of the corresponding subnet to User PC1
- Assign the 260th usable IP address of the corresponding subnet to User PC2
- Assign the 1st usable IP address of the corresponding subnet to www.salsabil.net web server
- Assign the 2nd usable IP address of the corresponding subnet to DNS and TFTP Server


Configurations
-----------------
- Configure the router hostname: SM
- Protect device configurations from unauthorized access with the encrypted password. Set the password to enpa$$word
- Secure all the ways to access the router. Set the passwords to smpa$$word
- Prevent all passwords from being viewed in clear text in device configuration files
- Set IP domain-name to sm.net
- Configure SSH version 2. Use the value 1024 for encryption key strength. Set time out to 60 seconds and limit authentication retries to 5
- Create an user having username: admin and encrypted password: adminpa$$. Configure user authentication for in-band management connections.
- Configure the two Gigabit Ethernet interfaces using the IPv4 values you calculated. Use description for both interfaces. Set interface descriptions to 'User LAN' and 'Server LAN' respectively.
- Backup the running configuration of router to the TFTP Server. Use the default file name.

Testing
--------
At the end of the configuration
- You should be able to remotely login to Router using SSH.
- You should be able to browse www.salsabil.net using web browser from any User PC.
