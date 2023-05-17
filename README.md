# Computer Network Lab Work Notes
## Lab 1
1. Test TCP/IP Protocol Stack
For Windows:
C:\>ping 127.0.0.1 (For IPV4)
C:\>ping ::1 (For IPV6)

For Linux
# ping 127.0.0.1
# ping ::1

2. check the Mac Address
C:\> ipconfig /all
			24bit		  24bit
physical address:  OUI		Device ID
			 6Hex	    	  6Hex


3. check the IPAddress Details
C:\> ipconfig /all
#ifconfig
Output:
IPv4 Address. . . . . . . . . . . : 172.16.0.44(Preferred)
Subnet Mask . . . . . . . . . . . : 255.255.255.0   
Default Gateway . . . . . . . . . : 172.16.0.1                                                                         
DHCP Server . . . . . . . . . . . : 172.16.0.1 

4. Test the internet connectivity
C:\> ping 8.8.8.8
C:\> ping 1.1.1.1

5. Check the DNS
C:\> ping google.com.np
				(If address is translated => ok)
6. Trace Path/ Route
C:\>tracert google.com.np
# traceroute google.com.np
# tracepath google.com.np
	It does maximum 30Hops

7. Identify the name server
C:\> nslookup google.com.np

IP Details:
Non-authoritative answer:                                                                                               
Name:    google.com.np                                                                                                  
Addresses:  2404:6800:4007:820::2003                                                                                              
          142.250.193.131     

Also,
nslookup facebook.com

Output:
Server:  dns.google                                                                                                     
Address:  8.8.8.8                                                                                                                                                                                                                               Non-authoritative answer:                                                                                               Name:    facebook.com                                                                                                   Addresses:  2a03:2880:f12f:183:face:b00c:0:25de                                                                                   31.13.79.35 

Reverse Lookup
nslookup <ipaddress>


Identify the IP Details
steps:
1. Go to google search 
2. Enter whois <address>
then it will show you necessary details about the IP
example:
whois 103.96.32.1
