# CCNA 200-301 [Notekeeping]

## 1 Client-Server Model
![alt text](https://github.com/NashoNightmare/CCNA-200-301-NoteKeep/blob/master/server-client.png)

## 2 Ethernet Cable vs Crossover Cable
![alt text](https://github.com/NashoNightmare/CCNA-200-301-NoteKeep/blob/master/2021-02-26%2010_03_40-Cisco%20CCNA%20200-301%20Exam_%20Complete%20Course%20with%20practical%20labs%20_%20Udemy.png)

## 3 Networking Devices
- **Switch (Layer 2 Device)** - Learn mac address much more quickly using hardware ASICS (Application Specific Integrated Circuits).
- **Ethernet Cable / Hubs (Layer 1 Devices)**
- **Router (Layer 3 Device)** - Routing the transmissions.
- **Bridge (Layer 2 Device)** - Learns mac addresses in software.

## 4 Firewalls
Physical firewalls rely between switch and router because router should deal with ISP (Because router supports various technologies such as ADSL / Wireless capability (4G, 3G).

## 5 IPS and IDS
- **IPS (Intrusion Prevention System)** - Blocks if  malicious activity alerts. Resides within the network flow.
- **IDS (Intrusion Detection System)** - Taking copies from network flow and warns.

## 6 Protocols
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
	- 3389 - rdp
	- `System ports : 0-1023` `User ports : 1024-49151` `Dynamic/Private ports : 49152-65535`
	- More about ports : [Link](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml)

## 7 OSI Layer Model
- **Application Layer** - Providing networking options to programs running on a computer.
- **Presentation Layer** - Translates data into standardised format, as well as handling encryption, compression, or other transformations to data.
- **Session Layer** - Making and logging a session to a connection.
- **Transport Layer** - Choose protocol from TCP or UDP. Divides the transmision data into byte sized pieces. `TCP - Segments` `UDP - Datagrams`
- **Networking Layer** - Decides the best route to take by looking at the IP (Logical addressing). (Still controllable by softwares).
- **Data-Link Layer** - Stamping the receiving MAC address (endpoint's) by looking at IP. Also checks corruptions and formatting. `NB : Actually physical address is used to transmit data across networks. Which can spoofed and act as a client`
- **Physical Layer** - Electric pulses make up data transfer over a network `Binary data -> Signals (Transmitting)` `(Receiving) Signals -> Binary data`

## 8 Encapsulation

![alter text](https://github.com/NashoNightmare/Advent-Of-Cyber/blob/master/Encapsulation%20process.png)

## 9 TCP/IP Model

![alter text](https://github.com/NashoNightmare/Advent-Of-Cyber/blob/master/tcp-ip-model.png)

## 10 Three-Way handshake (Building a stable connection over TCP)

![alter text](https://github.com/NashoNightmare/Advent-Of-Cyber/blob/master/handhshake.png)

## 11 NIC (Network Interface Card)
NIC is used to connect to a digital network. Basically this means it allows your computer to speak in bits like it would talk to any other part of itself.

## 12 HTTP

![alter text](https://github.com/NashoNightmare/Advent-Of-Cyber/blob/master/http%20image%201.png)

![alter text](https://github.com/NashoNightmare/Advent-Of-Cyber/blob/master/http%20image%202.png)


## 13 ARP (Address Resolution Protocol)
Used to find the MAC address of another device. Basically a broadcast sent over the network saying "who has this IP address?".

> `arp -a` - To view ARP entries (Windows)

![alt text](https://github.com/NashoNightmare/CCNA-200-301-NoteKeep/blob/master/arp_table.png)

## 14 IP Addressing

### 14.1 Overview

- Layer 3 logical address assigned by an administrator
- Resides at Layer 3 of OSI model
- Used to identify specific devices on a network
- Every device on the internet has a uniques IP address

- RFC1918 Addresses 
	- If a private address `10.1.1.1` is NAT(Network Address Translate)ed to the public ip address `12.1.1.1` , The public ip address `12.1.1.1` must be unique in the internet.

#### 14.1.1 IPv4
- Layer 3 network layer protocol
- Connectionless protocol. Higher layer protocol needed for a reliable connection.
	- TCP connection oriented (Three-way handshake)
	- UDP 
- Packets treated independently.(May take different paths, best paths)
- Hierarchial addressing structure.(Network and Host portion of the address)
- Best effort delivery. There is no guarantee of packet delivery.
- No data recovery features

- **Details**
	- Address size - 32 bit
	- Two main portions 
		- Network Address Portion (Network ID)
			- identifies a specific network
			- routers maintain routing tables that contain network ids
			- routers look at the destination ip address and match to the network address portion
		- Host Address Portion (Host ID)
			- identifies a specific endpointor or nod on a network
			- 

### 14.2 Address Classes


### 14.3 Special Addresses
- **Loopback address** -
- **Local broadcast address** -

### 14.4 Network Masks
