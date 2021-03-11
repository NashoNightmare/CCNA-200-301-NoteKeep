# CCNA 200-301 [Notekeeping]

## 1.0 Client-Server Model
![alt text](https://github.com/NashoNightmare/CCNA-200-301-NoteKeep/blob/master/server-client.png)

## 2.0 Ethernet Cable vs Crossover Cable
![alt text](https://github.com/NashoNightmare/CCNA-200-301-NoteKeep/blob/master/2021-02-26%2010_03_40-Cisco%20CCNA%20200-301%20Exam_%20Complete%20Course%20with%20practical%20labs%20_%20Udemy.png)

## 3.0 Networking Devices
- **Switch (Layer 2 Device)** - Learn mac address much more quickly using hardware ASICS (Application Specific Integrated Circuits).
- **Ethernet Cable / Hubs (Layer 1 Devices)**
- **Router (Layer 3 Device)** - Routing the transmissions.
- **Bridge (Layer 2 Device)** - Learns mac addresses in software.

## 4.0 Firewalls
Physical firewalls rely between switch and router because router should deal with ISP (Because router supports various technologies such as ADSL / Wireless capability (4G, 3G).

## 5.0 IPS and IDS
- **IPS (Intrusion Prevention System)** - Blocks if  malicious activity alerts. Resides within the network flow.
- **IDS (Intrusion Detection System)** - Taking copies from network flow and warns.

## 6.0 Protocols
Preceding layer decides what version or type the layer should use.

- **Layer 2 --- Type (Ether type) --- What kind of data the frame carries?**
	- 0x0806 - ARP 
	- 0x0800 - IPv4
	- 0x86DD - IPv6
	- More about types : [Link](https://en.wikipedia.org/wiki/EtherType)

- **Layer 3 --- PRO --- Which protocol used in layer 4?**
	- 0x06 - TCP
	- 0x11 - UDP
	- More about protocols : [Link](https://www.iana.org/assignments/protocol-numbers/protocol-numbers.xhtml)

- **Layer 4 ---Destination Port --- What service should accessed from the server (Application Layer Protocol)?**
	- 80 - http
	- 22 - ssh
	- 23 - telnet
	- 443 - https
	- 21 - ftp
	- 69 - tftp
	- 25 - smtp
	- 110 - pop3
	- `System ports : 0-1023` `User ports : 1024-49151` `Dynamic/Private ports : 49152-65535`
	- More about ports : [Link](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml)

## 7.0 ARP (Address Resolution Protocol)
Used to find the MAC address of another device. Basically a broadcast sent over the network saying "who has this IP address?".

> `arp -a` - To view ARP entries (Windows)

![alt text](https://github.com/NashoNightmare/CCNA-200-301-NoteKeep/blob/master/arp_table.png)


