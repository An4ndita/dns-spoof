# dns-spoof
Program to Spoof the Domain Name Server

This is a Man-in-the middle attack so there will be three entities :

   1.  The victim
   2.  The attacker
   3.  The Access Point/Gateway

The victim sends requests to the Access Point, the attacker sniffs them and modifies them and send the modified malicious request to the Access Point on behalf of the victim. The attacker does this by creating a queue of packets, storing all the requests, modifying them using a program and then sending them to the Access Point.

The elaborated description of the usage of this tool is available in the following blog, please visit this link for more details.

https://an4ndita.medium.com/writing-your-own-dns-spoofer-program-coding-for-cyber-security-program-4-6d8d1b30f6fd


# DEPENDENCIES :

$ sudo apt-get install python3-scapy

$ sudo pip install netfilterqueue


# USAGE :

$ sudo git clone https://github.com/An4ndita/dns-spoof.git

$ cd dns-spoof

$ sudo mousepad dns.py

Edit the hosts {} part and enter the domains that you intend to spoof parallel to your IP address and save it.

$ sudo python3 dns.py
