# &#x09;				OSI Model







* ###### It is set of rules that explains how different computer systems communicate over network.
* ###### developed by ISO (International Organization for Standardization).
* ###### It makes easier for different devices and technologies to work together.
* ###### It helps professionals understand where attacks occur and how to defend against them. Each of the 7 layers has its own security risks and controls.











+---------------------------+

| 7. Application Layer      |

|    (HTTP, FTP, Email)     |

| 🔴 Attacks: SQLi, XSS    |

| 🛡️ Defense: WAF, Auth    |

+---------------------------+

| 6. Presentation Layer     |

|    (Encryption, Encoding) |

| 🔴 Attacks: Weak crypto  |

| 🛡️ Defense: SSL/TLS      |

+---------------------------+

| 5. Session Layer          |

|    (Session management)   |

| 🔴 Attacks: Hijacking    |

| 🛡️ Defense: Tokens, MFA  |

+---------------------------+

| 4. Transport Layer        |

|    (TCP/UDP, Ports)       |

| 🔴 Attacks: SYN flood    |

| 🛡️ Defense: Filtering    |

+---------------------------+

| 3. Network Layer          |

|    (IP, Routing)          |

| 🔴 Attacks: IP spoofing  |

| 🛡️ Defense: Firewalls    |

+---------------------------+

| 2. Data Link Layer        |

|    (MAC, Switching)       |

| 🔴 Attacks: ARP poison   |

| 🛡️ Defense: VLAN, DAI    |

+---------------------------+

| 1. Physical Layer         |

|    (Cables, Hardware)     |

| 🔴 Attacks: Wiretapping  |

| 🛡️ Defense: Physical sec |

+---------------------------+









##### 

##### **Layer 1: Physical Layer** :-



* ###### responsible for the actual physical connection between the devices.
* ###### contains information in the form of bits. 
* ###### responsible for transmitting individual bits from one node to the next.



###### **Devices:-** Hub, Repeater, Modem and Cables.

###### 

###### **Functions:-** Bit Synchronization, Bit Rate Control, Physical Topologies, Transmission Mode













##### **Layer 2: Data Link Layer :-**



* ###### **responsible for the node-to-node delivery of the message.**
* ###### **make sure data transfer is error-free from one node to another, over the physical layer**
* ###### **responsible to transmit it to the Host using its MAC address.** 

###### 

* ###### **Devices: Switches \& Bridges.**



###### **Sublayers of Data Link Layer :**

###### 

* ###### Logical Link Control (LLC)
* ###### Media Access Control (MAC)



###### **Functions :** Framing, Physical Addressing, Error Control, Flow Control, Access Control.













##### **Layer 3: Network Layer :-**



* ###### transmission of data from one host to receivers.
* ###### Chooses shortest path to transmit the packet, from the number of routes available.



* ###### **Devices:** Routers \& Switches.

###### 

* ###### sender's and receiver's IP address are placed in the header by the network layer.
* ###### Segments in network layer known as packets.

###### 

* ###### **Functions :** Routing, Logical Addressing.















##### **Layer 4: Transport Layer :-**



* ###### provides services to the application layer and takes services from the network layer
* ###### responsible for the end-to-end delivery of the complete message.
* ###### acknowledgment of the successful data transmission and re-transmits the data if an error is found. 
* ###### It also adds Source and Destination port number in its header and forwards the segmented data to the Network Layer.
* ###### 
* ###### **Protocols :** TCP, UDP, NetBIOS, PPTP.



* ###### **Functions** **:** Segmentation and Reassembly, Service Point Addressing.













##### **Layer 5: Session Layer :-**



* ###### responsible for the establishment of connections, management of connections, terminations of sessions between two devices.

###### 

* ###### **Protocols :** NetBIOS, PPTP.



* ###### **Functions :** Session Establishment, Maintenance, and Termination, Synchronization, Dialog Controller.













##### **Layer 6: Presentation Layer (Translation layer):-** 



* ###### Data from the application layer is extracted here and manipulated as per the required format to transmit over the network.

###### 

* ###### **Protocols :** TLS, SSL. 

###### 

* ###### **formats used for encoding data** JPEG, MPEG, GIF. 



* ###### **Functions :** Translation, Encryption(cyphertext) / Decryption(Plain text), Compression.

##### 











##### **Layer 7: Application Layer :-**



* ###### produce the data to be transferred over the network. 

###### 

* ###### **Protocols :** SMTP, FTP, DNS.

###### 

* ###### **Functions** : Network Virtual Terminal(NVT), File Transfer Access and Management(FTAM), Mail Services, Directory Services.











