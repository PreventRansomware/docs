---
sidebar_position: 6
---

Firewalls filter traffic that travels in and out of a network. In an ideal world your firewall should allow nothing in and only the bare minimum out. Unfortunately, this isn’t how the real world works. System administrators need to open ports for various business reasons; attackers know this and scour the internet for open ports with which they can breach a network.

 Remote Desktop (RDP for short) runs on port 3389; it’s used for remote system administration and user access which increased during the COVID-19 outbreak. Thanks to this increase and plain bad firewall administration, many networks have exposed RDP directly to the open internet. At the time of writing, [Shodan ][1]shows [over ￼three million systems with Remote Desktop exposed to the internet.][2]
  
This is bad because it means an attacker could exploit a [vulnerability in Microsofts RDP protocol][3] or guess a working username and password combination to have instant, persistent access to a victim network. The latter has become popular with [ransomware operators.][4]

Having RDP open to the internet is akin to leaving the front door wide open. You should ensure that **administrative ports like 3389 are not allowed inbound.**   
Other common sensitive management ports which are often left open are:  

- 22 - SSH
- 23 (Telnet)
- 443 - Management consoles that shouldn’t be accessible from the outside
- 445 - SMB
- 137 - RPC

As earlier mentioned and regardless of the above list, you should aim to **block** all ports inbound, only allowing what is absolutely necessary to enable your business to function **however,** forcing ports closed on a business that legitimately has a need for them isn’t good practice either. Security risk must be balanced with usability. If your business does require an inbound port to be open you should aim to restrict traffic to a particular source IP address (such as a service provider who needs access) and, if possible, only allowed at particular expected times, such as during working hours. 

Auditing firewall rules can be a difficult task because administrators have to juggle many rules which can be handled by different teams or even staff that have moved on. There are tools on the market that can help but our favourite is Shodan, it scans the entire internet and documents its findings in a searchable database. You can input your public IPs into its search bar which will show open ports, vulnerabilities and more.   
If RDP or SSH are shown as below you should aim to close them as soon as possible. 
![][image-1]
  


Often significant security progress can be made only to be undone by someone else with entirely good intentions who is troubleshooting, implementing or trying to fix a problem. It’s possible that after reading this guide, a system administrator will go and close or restrict inbound RDP only to find (once it’s too late) that somebody else reopened the port at a later date, thus re-exposing the network to attack. [Shodan Monitor][5] allows administrators to receive alerts when ports are open, which shouldn’t be or if new ports are opened. Adding an IP address to a Shodan account and configuring notifications is a simple and cost-effective way of monitoring for unexpected edge of network configuration changes. Signing up for the basic freelancer package provides sufficient capabilities for most organisations.









[1]:	https://help.shodan.io/the-basics/what-is-shodan
[2]:	https://www.shodan.io/search?query=Remote+Desktop+Protocol
[3]:	https://nvd.nist.gov/vuln/detail/CVE-2019-0708
[4]:	https://www.varonis.com/blog/darkside-ransomware/
[5]:	https://monitor.shodan.io

[image-1]:	/img/DocImages/openportexample.png