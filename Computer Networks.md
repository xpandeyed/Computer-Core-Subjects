# Computer Networks

https://whimsical.com/networking-cheatsheet-by-love-babbar-XXLEegnxTNu6oUX7eepX5Y

Open System Interconnection Model

![Untitled](Computer%20Networks%20f33970938f0f4c168434db44d8047ad8/Untitled.png)

| OSI Layer | Function/Responsibilities | Devices Used | Protocols Used | Addressing | Endpoints |
| --- | --- | --- | --- | --- | --- |
| Physical Layer | Defines the electrical, mechanical, and procedural means to connect and transmit data between two network nodes. | Network adapters, cables, connectors, repeaters, hubs | Ethernet, Token Ring, FDDI, PPP, SLIP | MAC address | Physical devices |
| Data Link Layer | Provides error detection and correction, flow control, and addressing. | Bridges, switches | Ethernet, Token Ring, PPP, SLIP | MAC address | Physical devices |
| Network Layer | Provides routing and forwarding of data packets between nodes on different networks. | Routers | IP, IPX, AppleTalk | IP address | Network nodes |
| Transport Layer | Provides reliable data transfer between two hosts. | Firewalls, NAT devices | TCP, UDP, SPX | Port number | Transport layer sockets |
| Session Layer | Establishes, manages, and terminates communication sessions between two applications. | - | NetBIOS, RPC, SQLNet | Session ID | Session layer sockets |
| Presentation Layer | Translates data between different formats so that it can be understood by the application layer. | - | ASCII, EBCDIC, JPEG, MPEG | - | Application layer sockets |
| Application Layer | Provides services to applications, such as file transfer, email, and web browsing. | Web browsers, email clients, file transfer clients | HTTP, FTP, SMTP, POP3 | - | Application layer sockets |

TCP/IP Model has 5 layers. Presentation and Session layer are integrated in Application layer.

**What Happens When You Type www.google.com in Your Browser and Press Enter?**

[https://www.linkedin.com/pulse/what-happens-when-you-type-wwwgooglecom-your-browser-press-kalaghe/](https://www.linkedin.com/pulse/what-happens-when-you-type-wwwgooglecom-your-browser-press-kalaghe/)

| Protocol | OSI Layer | Function |
| --- | --- | --- |
| Ethernet | Physical Layer, Data Link Layer | Ethernet is a widely used networking technology that allows devices to communicate and share data over a local area network (LAN). It uses a set of protocols and standards to establish a reliable and efficient connection between devices.
The typical range is 100 metres.
Ethernet is NOT wireless technology but improvements have been made to tackle that. |
| ARP | Data Link Layer | Finds MAC address using IP Address |
| RARP | Data Link Layer | Find IP address using MAC Address |
| BOOTP | Data Link Layer | Bootstrap Protocol BOOTP is primarily used to assign IP addresses and other network configuration parameters to devices during their boot process |
| HDLC
 | Data Link Layer | HDLC (High-Level Data Link Control) is a data link layer protocol that provides reliable and efficient communication by framing data, detecting errors, managing flow control, and ensuring data integrity in computer networks. |
| DHCP | Network Layer | DHCP, or Dynamic Host Configuration Protocol, is a networking protocol widely used in TCP/IP networks to automatically assign and manage IP addresses and other network configuration parameters to devices. |
| IP | Network Layer | Provides routing and addressing of data packets. |
| TCP | Transport Layer | Transmission Control Protocol
Provides reliable data transfer between two hosts. |
| UDP | Transport Layer | User Datagram Protocol
Provides unreliable data transfer between two hosts. |
| HTTPS | Transport Layer |  |
| HTTP | Application Layer | Used for transferring hypertext documents, such as web pages, over the Internet. |
| SMTP | Application Layer | Used for sending email messages. |
| POP | Application Layer | Used for receiving email messages. |
| IMAP | Application Layer | Used for accessing email messages on a mail server. |
| DNS | Application Layer | Used for translating domain names into IP addresses. |
| SNMP | Application Layer | Used for managing network devices. |
| TELNET | Application Layer |  |
| SSH | Application Layer |  |
| FTP | Application Layer |  |
| TFTP | Application Layer |  |
| NFS | Application Layer |  |
| MIME | Application Layer |  |

| Term | Explanation |
| --- | --- |
| Client | A device or application that requests services or resources from a server. |
| Server | A device or application that provides services or resources to clients. |
| Peer | A device or entity at the same level or in a peer-to-peer network with equal status. |
| Host | A general term for any device connected to a network, which can be a client, server, or both. |
| Bandwidth | The maximum data transfer rate of a network or communication channel, typically measured in bits per second (bps). |
| Jitter | Variability in the delay between data packets, often causing disruptions in real-time communication. |
| Packet | A small unit of data transmitted over a network, including both the data payload and control information. |
| Frame | A data unit at the data link layer, containing a packet along with control information such as source and destination addresses. |
| Local Host | The device or computer you are using directly, often referred to as "localhost" or "127.0.0.1." |
| Bit Rate | The rate at which bits (binary digits) are transmitted or processed per unit of time. |
| Noise | Unwanted electrical or electromagnetic interference that can disrupt data transmission or reception. |
| Attenuation | The reduction in signal strength as it travels over a distance or through a medium, often due to resistance or absorption. |
| Distortion | Alteration or corruption of a signal or data during transmission, typically caused by interference or noise. |
| Congestion | A state occurring in network layer when the message traffic is so heavy that it slows down network response time. |
|  |  |

| Device | Common Use | OSI Layer |
| --- | --- | --- |
| Hub | Connect devices in a network segment, but they do not intelligently filter or forward data. All devices in a hub share the same collision domain. | Physical |
| Switch | Efficiently forward data frames to specific devices based on MAC addresses, reducing network collisions and segmenting traffic. | Data Link |
| Router | Connect and route data between different networks or subnets, making forwarding decisions based on IP addresses. | Network |
| Bridge | Connect and filter traffic between two or more network segments based on MAC addresses. Helps reduce collision domains and manage network traffic. | Data Link |
| Gateway | Translate between different communication protocols or data formats to enable communication between networks that use different technologies. | Application |
| Modem | Convert digital data from a computer or network into analog signals for transmission over analog communication lines (e.g., telephone lines) and vice versa. | Physical and Data Link |
| Node | Fundamental building block of the network. It can be any device or point on the network that can send, receive, or forward data. Nodes can include computers, servers, routers, switches, printers, |  |
| Firewall | A firewall is a network security device or software that acts as a interface between a trusted internal network and untrusted external networks, such as the internet. Its primary function is to control and monitor incoming and outgoing network traffic, allowing or blocking traffic based on predefined security rules. Firewalls are crucial for protecting networks and devices from unauthorized access, cyber threats, and malicious activities. | Transport Layer and Network Layer |

Difference Between web and internet:

These concise definitions should provide a clear understanding of each term.

![Untitled](Computer%20Networks%20f33970938f0f4c168434db44d8047ad8/Untitled%201.png)

**IP:**

IP stands for "Internet Protocol." It is a set of rules and conventions that govern how data packets should be formatted, addressed, transmitted, routed, and received over a network, particularly the internet.

| Characteristic | IPv4 | IPv6 |
| --- | --- | --- |
| Address Length | 32 bits (4 bytes) | 128 bits (16 bytes) |
| Address Notation | Decimal with periods | Hexadecimal with colons |
| Address Format Example | 192.168.1.1 | 2001:0db8:85a3:0000:0000:8a2e:0370:7334 |
| Address Space | Approximately 4.3 billion | Approximately 340 undecillion |
| Address Allocation | Static and DHCP | Stateless Address Autoconfiguration (SLAAC) and DHCPv6 |
| Broadcast | Supports broadcast addresses | No broadcast, replaced with multicast |
| Multicast | Limited multicast support | Built-in support for multicast |
| Header Length | Fixed header length | Variable header length (simpler and more efficient) |
| Header Fields | 20 fields | 8 fields |
| Checksum | Includes a checksum in the header | No header checksum (handled by lower layers) |
| Network Address Translation (NAT) | Commonly used to conserve IPv4 addresses | Less need for NAT, as more addresses are available |
| Routing | IPv4 uses Broadcast and ARP for neighbor discovery | IPv6 uses ICMPv6 and Neighbor Discovery Protocol (NDP) |
| Address Resolution Protocol (ARP) | ARP is used to map IP addresses to MAC addresses | ARP is replaced by NDP (Neighbor Discovery Protocol) |

An IP address is a string of numbers separated by periods. IP addresses are expressed as a set of four numbers — an example address might be 192.158.1.38. Each number in the set can range from 0 to 255. So, the full IP addressing range goes from 0.0.0.0 to 255.255.255.255.

IP addresses are not random. They are mathematically produced and allocated by the [Internet Assigned Numbers Authority](https://www.iana.org/) (IANA), a division of the [Internet Corporation for Assigned Names and Numbers](https://www.icann.org/) (ICANN).

| Class | Network ID bits | Host ID bits | Range | Default subnet mask | Fixed bits in network ID |
| --- | --- | --- | --- | --- | --- |
| Class A | 8 | 24 | 0.0.0.0 to 127.255.255.255 | 255.0.0.0 | 0 (first bit) |
| Class B | 16 | 16 | 128.0.0.0 to 191.255.255.255 | 255.255.0.0 | 01 (first two bits) |
| Class C | 24 | 8 | 192.0.0.0 to 223.255.255.255 | 255.255.255.0 |  |
| Class D | 4 | - | 224.0.0.0 to 239.255.255.255 | N/A |  |
| Class E | 4 | - | 240.0.0.0 to 255.255.255.255 | N/A |  |

Classful addressing was the original method of IP address allocation. However, it has since been superseded by classless addressing, which allows for more flexibility in the allocation of IP addresses.

Classless addressing, also known as Classless Inter-Domain Routing (CIDR), is a more flexible and efficient method of IP address allocation and routing compared to the older classful addressing scheme.

**Prefix Notation:** CIDR notation represents IP addresses and their associated subnet masks using a prefix length, often denoted as "/X," where X is the number of bits in the subnet mask. For example, "192.168.1.0/24" indicates that the first 24 bits of the IP address are the network portion, and the remaining 8 bits are for host addresses.

To get default subnet mask, make all the network id bits as one and host id bits as zero.

**Private IP Address / Non Routable Address Space:**
A private IP address is an IP address used within a private network, such as a home, office, or organization's internal network. These addresses are not directly accessible from the internet and are meant for local communication within the private network. Private IP addresses help conserve the limited pool of available IP addresses in the IPv4 system.

- IPv4: 10.0.0.0 to 10.255.255.255
- IPv4: 172.16.0.0 to 172.31.255.255
- IPv4: 192.168.0.0 to 192.168.255.255

Although there is a technology called NAT that allows private IPs to connect to internet.

**Public IP Address:**
A public IP address is a globally unique IP address assigned to a device that is accessible over the internet. It is used to identify a specific device on the public internet and allows other devices to establish connections with it. Public IP addresses are allocated by Internet Service Providers (ISPs) and are used to route data between devices across different networks.

**TCP:**

![Untitled](Computer%20Networks%20f33970938f0f4c168434db44d8047ad8/Untitled%202.png)

Roles/functionalities/responsibilities of TCP:

Transmission Control Protocol (TCP) is a core protocol of the Internet Protocol (IP) suite.

1. **Connection Establishment and Termination:**
    - TCP ensures that a reliable connection is established between a sender and a receiver before data transmission begins.
    - It uses a three-way handshake (SYN, SYN-ACK, and ACK) to establish a connection and a four-way handshake to gracefully terminate it.
2. **Reliable Data Transfer:**
    - TCP provides reliable data transfer by ensuring that data is transmitted accurately and without errors.
    - It uses sequence numbers to order packets and acknowledgments to confirm the receipt of data.
    - If data packets are lost or corrupted during transmission, TCP retransmits them to ensure delivery.
3. **Flow Control:**
    - TCP employs flow control mechanisms to prevent congestion and manage the rate of data transfer.
    - It uses window sizes to determine the amount of data that can be sent before waiting for acknowledgments.
    - Flow control helps ensure that the sender does not overwhelm the receiver with data.
4. **Error Detection and Correction:**
    - TCP includes error-checking mechanisms, such as checksums, to detect errors in transmitted data.
    - When errors are detected, TCP requests the retransmission of the affected packets.
5. **Ordered Data Delivery:**
    - TCP guarantees that data sent from one end will be received in the same order by the other end.
    - It uses sequence numbers to reorder packets if they arrive out of order.
6. **Full-Duplex Communication:**
    - TCP supports full-duplex communication, allowing data to be sent in both directions simultaneously.
    - This means that a TCP connection can transmit data from the sender to the receiver and from the receiver to the sender independently.
7. **Acknowledgments:**
    - TCP uses acknowledgment messages (ACKs) to confirm the receipt of data packets.
    - These ACKs help the sender determine which packets need to be retransmitted in case of loss.
8. **Port Numbers:**
    - TCP uses port numbers to identify specific services or applications on a device.
    - Port numbers, along with IP addresses, help route data to the correct application or service on the destination device.
9. **Multiplexing:**
    - TCP allows multiple applications on a single device to use the network simultaneously by using different port numbers for each application.
    - This enables the mixing of multiple data streams on the same network connection.
10. **Timeout and Retransmission:**
    - TCP uses timeout values to determine when a packet or acknowledgment is considered lost.
    - If an acknowledgment is not received within a certain time, TCP retransmits the corresponding data packet.
11. **Congestion Control:**
    - TCP monitors network congestion and adjusts its sending rate to alleviate congestion.
    - It uses various algorithms, such as TCP congestion control and avoidance, to prevent network congestion collapse.
12. **Segmentation and Reassembly:**
    - TCP segments large amounts of data into smaller packets for transmission and reassembles them at the receiver.
    - This segmentation ensures that data can be efficiently transmitted over networks with different Maximum Transmission Unit (MTU) sizes.
13. **Support for Multiple Operating Systems and Platforms:**
    - TCP is designed to be platform-independent, allowing devices and operating systems from different vendors to communicate with one another.

**TCP is used:**

1. **Web Browsing (HTTP)**
2. **Email (SMTP, IMAP, POP3)**
3. **File Transfer (FTP, SFTP)**
4. **Remote Access (SSH, Telnet)**
5. **Database Communication (MySQL, PostgreSQL, Oracle)**
6. **VoIP (Voice over IP)**
7. **Instant Messaging (XMPP)**
8. **Virtual Private Networks (VPN)**
9. **Secure Data Transfer (HTTPS, FTPS)**
10. **Network Printing (IPP)**
11. **Network File Sharing (SMB, NFS)**
12. **Network Management (SNMP)**

**UDP:**

- UDP is used when acknowledgement of data does not hold any significance.
- UDP is good protocol for data flowing in one direction.
- UDP is simple and suitable for query based communications.
- UDP is not connection oriented.
- UDP does not provide congestion control mechanism.
- UDP does not guarantee ordered delivery of data.
- UDP is stateless.
- UDP is suitable protocol for streaming applications such as VoIP, multimedia streaming.

Here are few applications where UDP is used to transmit data:

- Domain Name Services
- Simple Network Management Protocol
- Trivial File Transfer Protocol
- Routing Information Protocol

**P2P (Peer to Peer File Sharing):**

A peer-to-peer network allows computer hardware and software to communicate without the need for a server. Unlike client-server architecture, there is no central server for processing requests in a **[P2P architecture](https://www.geeksforgeeks.org/what-is-p2ppeer-to-peer-process/)**. The peers directly interact with one another without the requirement of a central server.

**ARP:**

**The Problem**: When a device on a network wants to communicate with another device using its IP address, it needs to know the MAC address of the target device. The device uses this MAC address to frame and deliver the data to the right destination on the local network. However, it doesn't always have this information readily available.

**Address Resolution**: This is where ARP comes into play. ARP allows a device to discover the MAC address associated with a specific IP address within its local network segment. Here's how the process generally works:

- **ARP Request**: The device wanting to discover the MAC address of another device sends an ARP request (an ARP broadcast) to the local network. This request includes the IP address it's looking for.
- **ARP Reply**: The device with the corresponding IP address receives the ARP request, recognizes its IP address in the request, and responds with its MAC address in an ARP reply. This reply is sent directly to the requesting device.

**Network:**
A network refers to a collection of interconnected devices, such as computers, servers, printers, and other devices, that can communicate and share resources with each other. Networks are designed to facilitate the exchange of data and information between devices, allowing them to work together efficiently. Networks can be categorized based on their geographical scope:

1. **Local Area Network (LAN):** A LAN is a network that covers a relatively small geographic area, such as a single building, office, or home. LANs are used to connect devices within a close proximity to each other.
2. **Wide Area Network (WAN):** A WAN spans a larger geographic area, often connecting multiple LANs together. The internet itself is the largest example of a WAN. WANs are used to connect devices that are geographically separated, often across cities or even countries.

**Internet:**
The internet is a global network of networks. It is a vast interconnected network infrastructure that allows millions of computers and devices around the world to communicate with each other. The internet enables various services such as web browsing, email, online gaming, file sharing, and more. It's not owned by any single entity, but rather consists of a decentralized collection of interconnected networks operated by various organizations, ISPs (Internet Service Providers), and governments.

**Difference between Network and Internet:**

1. **Scope:**
    - A network refers to the interconnected devices within a specific area, such as a home, office, or data center.
    - The internet refers to the vast global network that connects millions of networks and devices worldwide.
2. **Geographical Reach:**
    - A network's geographical reach can be limited to a single building or a small area.
    - The internet spans the entire globe and connects networks across different continents.
3. **Ownership and Infrastructure:**
    - Networks can be privately owned by individuals, companies, or organizations.
    - The internet is a decentralized network of networks without a single owner. It consists of a collaborative effort involving various entities.
4. **Purpose:**
    - Networks facilitate communication and resource sharing among devices within a confined area.
    - The internet enables communication, information sharing, and services on a global scale.
5. **Example:**
    - A company's internal network connecting its computers and printers is an example of a network.
    - When you access a website or send an email using a web browser, you're utilizing the internet.

In summary, a network is a localized collection of interconnected devices, while the internet is a global network of networks that allows worldwide communication and information sharing.

**Network Topology:**
Network topology refers to the physical or logical arrangement of devices, links, and nodes within a computer network. It outlines how devices are connected and the paths through which data flows in the network. Network topology plays a crucial role in determining how efficiently data can be transmitted, the network's reliability, and its scalability.

![Untitled](Computer%20Networks%20f33970938f0f4c168434db44d8047ad8/Untitled%203.png)

**Bandwidth:**
Bandwidth refers to the **maximum data transfer rate of a network or a communication channel.** It represents how much data can be transmitted from one point to another in a given amount of time. Bandwidth is usually measured in bits per second (bps) or its multiples, such as kilobits per second (Kbps), megabits per second (Mbps), or gigabits per second (Gbps). A higher bandwidth allows for faster data transmission and better performance in network communication.

**Node:**
In the context of computer networks, a node is a **fundamental building block of the network. It can be any device or point on the network that can send, receive, or forward data. Nodes can include computers, servers, routers, switches, printers,** and any other devices that are part of the network. Nodes are interconnected to enable communication and data exchange within the network.

**Link:**
A link, also known as a communication link or network link, is a **physical or logical connection that allows data to flow between nodes in a network. It represents the pathway through which data travels from one node to another.** Links can be wired or wireless and can take various forms, such as Ethernet cables, fiber-optic cables, Wi-Fi connections, or even satellite links in wide area networks (WANs). The quality and capacity of links influence the speed and efficiency of data transmission between nodes.

In summary, bandwidth refers to the data transfer rate of a network, node is a device or point on a network, and link is the connection that enables data to flow between nodes. These concepts are fundamental to understanding how computer networks function and how data is transmitted within them.

**DNS (Domain Name System):**
The Domain Name System (DNS) is a fundamental component of the internet that translates human-friendly domain names (like [www.example.com](http://www.example.com/)) into the IP addresses that computers use to identify and communicate with each other. DNS serves as a sort of "phonebook" of the internet, allowing users to access websites and services using easy-to-remember domain names instead of numerical IP addresses.

A MAC address, short for "Media Access Control" address, is a unique identifier assigned to a network interface card (NIC) of a network device. This address is assigned by the manufacturer and is embedded into the hardware of the device during its production. MAC addresses are used primarily at the data link layer of the OSI (Open Systems Interconnection) model to uniquely identify devices on a local network, such as an Ethernet or Wi-Fi network.

Here are some key points about MAC addresses:

1. **Uniqueness:** Every network device has a globally unique MAC address. No two devices should have the same MAC address. This uniqueness is important for ensuring that network communication functions properly.
2. **Format:** A MAC address is usually represented as a sequence of six pairs of hexadecimal digits (0-9 and A-F), separated by colons or hyphens. For example, "00:1A:2B:3C:4D:5E."
3. **Organization:** The first three pairs of digits in a MAC address are known as the Organizationally Unique Identifier (OUI). These identify the manufacturer or vendor of the device. The remaining three pairs are assigned by the manufacturer and provide a unique identifier for the specific device.
4. **Role:** MAC addresses are used in Ethernet networks to uniquely identify network devices. They are used to determine the source and destination of data frames on a local network.
5. **MAC Filtering:** Some network routers and access points allow administrators to set up MAC address filtering as a security measure. This means only devices with specific MAC addresses are allowed to connect to the network.
6. **Layer 2 Addressing:** MAC addresses operate at the data link layer (Layer 2) of the OSI model. They are used for communication within a local network segment. IP addresses, on the other hand, operate at the network layer (Layer 3) and are used for communication across different networks.
7. **Changing MAC Addresses:** In some cases, MAC addresses can be changed or "spoofed" by modifying software settings. This can be useful for privacy or security reasons, but it's important to note that the original hardware-assigned MAC address remains unchanged.
8. **Switching and Forwarding:** Switches and bridges use MAC addresses to forward data frames within a local network. They maintain MAC address tables to keep track of which devices are connected to which ports.

In summary, a MAC address is a unique identifier assigned to a network device's network interface card. It is used for communication within local networks and plays a crucial role in ensuring that data frames are directed to the correct destination on the network.

**Gateway:**
A gateway is a device or software that connects two or more different networks that use different protocols or technologies. It serves as an interface between networks, translating data from one network's format to another, allowing communication between otherwise incompatible networks. 

**Router:**
A router is a networking device that operates at the network layer of the OSI model (or the Internet layer of the TCP/IP model). Its **primary function is to forward data packets between different networks, making decisions about the most efficient path for data to travel**. Routers use routing tables and routing protocols to determine where to send packets based on their destination IP addresses.

Routers are commonly used in local area networks (LANs) and wide area networks (WANs) to connect devices and networks and ensure that data reaches its intended destination efficiently.

**Difference between Gateway and Router:**

1. **Function:**
    - A gateway translates between different network protocols or technologies.
    - A router forwards data packets between networks based on IP addresses.
2. **Translation vs. Forwarding:**
    - A gateway's primary role is protocol translation and data format conversion.
    - A router's primary role is to determine the best path for data to travel between networks.
3. **Networks Connected:**
    - A gateway connects networks that use different protocols or technologies.
    - A router connects networks and facilitates data routing between them.
4. **Layer:**
    - A gateway can operate at different layers of the OSI model, depending on its purpose.
    - A router operates at the network layer (Layer 3) of the OSI model or the Internet layer of the TCP/IP model.
5. **Example:**
    - A protocol converter that allows communication between a traditional phone network and a VoIP network is a type of gateway.
    - A home router that connects the local network to the internet and routes data between devices is an example of a router.

In summary, a gateway is a protocol translator that connects networks with different protocols, while a router is a networking device that forwards data packets between networks based on IP addresses. While they serve distinct purposes, they often work together in complex network setups to ensure effective communication.

**Subnet:** 

A subnet is a network inside a network achieved by the process called subnetting which helps divide a network into subnets. It is used for getting a higher routing efficiency and enhances the security of the network. It reduces the time to extract the host address from the routing table.

**Firewall:**

**Unicast:**
Unicast is a communication method in networking where data is sent from a single sender to a specific recipient device. It is a one-to-one communication model. In unicast communication, the sender and receiver have a direct and unique connection. Unicast is commonly used for most types of internet communication and is the default mode for many networking protocols.

**Example of Unicast:**
When you access a website in your web browser, your computer sends a unicast request to the web server hosting the website. The web server responds with the requested web page, and this communication is between your computer (sender) and the web server (receiver), forming a direct one-to-one connection.

**Multicast:**
Multicast is a communication method in networking where data is sent from a single sender to a group of recipients who have expressed interest in receiving the data. It is a one-to-many communication model. Multicast is particularly useful for distributing data to a specific group of devices without having to send individual copies of the data to each recipient.

**Example of Multicast:**
Imagine a video streaming service that wants to broadcast a live event to multiple subscribers. Instead of sending separate unicast streams to each subscriber, the service can use multicast. The video is sent once from the streaming server, and routers on the network replicate and forward the data only to the subscribers who have subscribed to the multicast group. This efficient approach reduces network congestion and saves bandwidth.

**Broadcast:**
Broadcast is a communication method in networking where data is sent from a single sender to all devices within a network segment or domain. It is a one-to-all communication model. Broadcast is less common in modern networks due to its potential to cause network congestion and security risks, and it's often restricted to specific network scenarios.

**Example of Broadcast:**
In the past, early local area networks (LANs) used broadcast extensively. For instance, in an Ethernet LAN, if a device wanted to discover the MAC address of a target device on the same LAN segment, it could send a broadcast message asking for the MAC address of that target. This message would be received by all devices on the segment, but only the target device would respond.

In summary:

- Unicast: One-to-one communication between a sender and a specific receiver.
- Multicast: One-to-many communication, where data is sent to a group of interested recipients.
- Broadcast: One-to-all communication within a specific network segment or domain, reaching all devices.

**Server Side Load Balancing:**

Server-side load balancing is a technique used to distribute incoming network traffic across multiple servers or backend resources to ensure efficient utilization of resources, improve performance, and prevent overload on individual servers. In this approach, a load balancer is placed between the client and the group of servers. The load balancer receives incoming requests, analyzes the current load on the servers, and forwards the requests to the server with the least load or according to a predefined algorithm.

Advantages of server-side load balancing:

- Simple client configuration: only need to know the load-balancer address.
- Clients can be untrusted: all traffic goes through the load-balancer where it can be looked at. Clients are not aware of the backend servers.

**Hubs:**
A hub is a basic networking device that operates at the physical layer (Layer 1) of the OSI model. It is designed to connect multiple devices in a network and transmit data to all connected devices. When a hub receives data from one device, it broadcasts the data to all other devices connected to the hub. Hubs do not perform any intelligent data forwarding or filtering; they simply regenerate and amplify the electrical signal to ensure that it reaches all devices.

Hubs are inefficient in terms of network bandwidth utilization because they send data to all devices, even if the data is intended for a specific recipient. As a result, they lead to network congestion and reduced overall network performance.

**Switches:**
A switch is a more advanced networking device that operates at the data link layer (Layer 2) of the OSI model. Unlike hubs, switches are intelligent devices that examine the data frames they receive and make decisions about where to forward those frames based on MAC addresses. Switches maintain a MAC address table that associates MAC addresses with specific switch ports, allowing them to send data only to the intended recipient rather than broadcasting it to all devices.

Switches offer several benefits over hubs, including improved network performance, reduced collision domains (since devices communicate directly without interfering with each other), and the ability to segment and isolate traffic within different virtual LANs (VLANs).

| HTTP | HTTPS |
| --- | --- |
| HTTP stands for HyperText Transfer Protocol. In HTTP, the URL begins with “http://”. | HTTPS stands for HyperText Transfer Protocol Secure. In HTTPS, the URL starts with “https://”. |
| HTTP uses port number 80 for communication. | HTTPS uses port number 443 for communication. |
| Hyper-text exchanged using HTTP goes as plain text i.e. anyone between the browser and server can read it relatively easily if one intercepts this exchange of data and due to which it is Insecure. | HTTPS is considered to be secure but at the cost of processing time because Web Server and Web Browser need to exchange encryption keys using Certificates before actual data can be transferred. |
| HTTP Works at the https://www.geeksforgeeks.org/application-layer-in-osi-model/. | HTTPS works at https://www.geeksforgeeks.org/transport-layer-responsibilities/. |
| HTTP does not use encryption, which results in low security in comparison to HTTPS. | HTTPS uses Encryption which results in better security than HTTP. |
| HTTP speed is faster than HTTPS. | HTTPS speed is slower than HTTP. |
| HTTP does not use data hashtags to secure data. | HTTPS will have the data before sending it and returning it to its original state on the receiver side. |
| HTTP is used to transfer text, video, and images via web pages. | HTTPS is used to transfer data securely via a network. |

The anatomy of a domain name:

- Fully Qualified Domain Name: **[www.example.com](http://www.example.com/)**
- Subdomain: www
- Second-Level Domain: example
- Top-Level Domain: .com

Collision Domain:

A collision domain refers to a segment of a network in which data collisions can occur. In Ethernet or other shared-medium networks, such as older versions of Wi-Fi (802.11b/g), collisions happen when multiple devices attempt to transmit data over the same communication channel simultaneously. This can lead to data corruption and inefficiencies in the network.