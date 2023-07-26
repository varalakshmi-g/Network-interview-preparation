# Network-interview-preparation
A collection of my learning notes, practice questions to prepare for network-related interviews and sharpening my knowledge on networking concepts.

Question 1:  What is Network? What are the types of network?

Ans: Network is a group of computers, servers, network devices which are connected together to share the data.

Types of network are:

1.PAN(Personal Area Network): PAN is the most basic type of computer network for interconnecting electronic devices within an individual person's workspace. The size of PAN ranges from a few centimeters to a few meters. A common example of PAN is the connection between a bluetooth earpiece and a smartphone.

2.LAN(Local Area Network): LAN is a privately owned computer network covering a small networks geographical area like a home, office, or groups of buildings. The size of LAN is usually small. The various devices in LAN are connected to central devices called HUB or switch using a cable.

3.WAN(Wide Area Network): A WAN is a telecommunication network. Simply WAN is network of networks. WANs connect LANs that may be on opposite sides of a building, across the country or around world. WANs are characterized by the slowest data communication rates and the largest distances. WANs are of two types, they are an Enterprise WAN and Global WAN. CComputers connected to a WAN are often connected through public networks such as telephonic system.

4.MAN(Metropolitan Area Networks): MAN is a new class of network. MAN is larger than a local area network and as its name implies, it covers the area of single city.MAN is rarely extend beyond 100 KM  and frequently comprise a combination of different hardware and transmission media. It is a means of connecting a number of LANs into a larger network so that resources can be shared LAN to LAN as well as device to device.

Question 2: What is OSI model?

Ans: The OSI(Open Systems Interconnection) model is a conceptual framework that standardizes the functions of a computing system into seven distinct layers. The OSI model was developed by International Organization for Standardization(ISO) to promote interoperability and facilitate communication between different systems and network devices.

The seven layers of OSI model are as follows:

1.Physical layer: This is the lowest layer of the model and deals with the physical transmission of data over a medium, such as cables,electrical signals or wireless transmission. It defines the hardware and physical characteristics of the network.

2.Data Link layer: The data layer is responsible for the reliable transfer of data frames between two devices over a physical link. It performs functions like framing, error detection and flow control.

3. Network layer: This layer handles the routing of data packets from the source to the destination across multiple networks. It deals with logical addressing and provides services like routing, forwarding and traffic control.

4. Transport layer: This layer is responsible for ensuring end to end communication and data flow control between applications on different devices. It can break large data into smaller segments and reassemble them at the destination.

5. Session layer: The session layer establishes, manages and terminates communication sessions between applications. It enables synchronization and keeps track of different conversations or sessions between networked devices.

6. Presentation layer: The presentation layer is responsible for data translation,encryption and compression, ensuring that data is presented in a format that the application layer can understand.

7. Application layer: This layer is the topmost layer and represents the interface between the user and network. It provides network services directly to end users and applications, enabling functions like email,file transfer and remote access.

The OSI model provides a systematic approach to designing and understanding network communication. Each layer performs specific functions and the interactions between these layers allow for seamless communication across diverse systems and networks.

Question 3: What is TCP/IP model?

Ans: The TCP/IP (Transmission Control Protocol/Internet Protocol) model is a set of networking protocols and standards that form the basis of the modern internet and most networks used today. TCP/IP was originally designed to enable communication and data exchange between different types of computers and networks. It is not a strict layered model like the OSI model but can be roughly mapped to the OSI layers. 

The TCP/IP model is composed of four main layers, each responsible for specific aspects of data transmission and communication:

1. Application Layer: This layer corresponds to the application layer in the OSI model. It is the top most layer and handles communication between applications or software running on different devices. It provides various network services directly to end-users, such as HTTP for web browsing, SMTP for email, FTP for file transfer, and DNS for domain name resolution.

2. Transport Layer: This layer corresponds to both the transport and session layers in the OSI model. It is responsible for end-to-end communication and data flow control between applications. The two primary protocols at this layer are TCP (Transmission Control Protocol) and UDP (User Datagram Protocol). TCP provides reliable and connection-oriented communication with error-checking and retransmission of lost data. UDP, on the other hand, is connectionless and provides faster, but less reliable, communication.

3. Internet Layer: This layer corresponds to the network layer in the OSI model. It handles the routing of data packets from the source to the destination across multiple networks. The main protocol at this layer is the Internet Protocol (IP), which is responsible for logical addressing, packet forwarding, and fragmentation of data.

4. Link Layer: This layer corresponds to the data link and physical layers in the OSI model. It deals with the physical transmission of data over a local network and includes protocols for error detection and correction, as well as addressing at the hardware level. Ethernet is a common example of a link layer protocol.

Question 4: What is IP address and what are the types in it?

An IP address(Internet Protocol), is a unique numerical label assigned to each device connected to a computer network that uses the Internet Protocol for communication. IP addresses are used to identify and locate devices on a network, enabling data transmission between them. They serve a crucial role in the routing of data packets over the internet and local networks.IP addresses are typically represented as a series of four numbers separated by periods, such as "192.168.1.1." Each number in the address can range from 0 to 255, allowing for a vast number of possible combinations.

There are mainly two types of IP address: 

1. IPv4(Internet Protocol Version 4): This is the older and most widely used version of IP addresses. IPv4 addresses are 32-bit long and represented in decimal format, as mentioned earlier. However, due to the rapid growth of the internet, the number of available IPv4 addresses has been exhausted. As a result, there has been a transition to IPv6 to address this limitation.

2. IPv6 (Internet Protocol version 6): IPv6 was developed to replace IPv4 and overcome its address space limitations. IPv6 addresses are 128-bit long and are represented in hexadecimal format, with eight groups of four characters. An example of an IPv6 address is "2001:0db8:85a3:0000:0000:8a2e:0370:7334." IPv6 provides an astronomically larger pool of unique addresses, ensuring that we won't run out of IP addresses for a very long time.

In the transition from IPv4 to IPv6, many devices and networks now support both versions, which is known as "dual-stack" operation. This allows for a gradual migration to IPv6 while still ensuring compatibility with existing IPv4 infrastructure.

Question 5: What is routing?

Ans: Routing is the process of selecting the best path or route for data packets to travel from the source to the destination across a network. In computer networks data is broken into smaller units called packets.

The main purpose of routing is to ensure that data packets reach their destinations efficiently and reliably. When a device sends data to another device on the same network, the routing process is relatively starightforward as the devices are directly connected. However, when the destination is on a different network, routing comes into play.

When a router receives a data packet, it checks the destination IP address against its routing table to determine the next hop or the next router to which it should send the packet. The router repeats this process at each hop along the route until the packet reaches its final destination.

Question 6: What is subnet?

Ans: Subnet is short for subnetwork. It is a logical division of an IP network. It was created by partitioning a single large network into smaller, more manageable segments to improve network performance, security and efficiency.In a typical IP network, each device is assigned an IP address, which consists of two parts: the network portion and the host portion. 

The subnet mask is a 32-bit value used to determine the boundary between the network and host portions of an IP address.For example, consider the IP address "192.168.1.100" with a subnet mask of "255.255.255.0." In this case, the first three octets (192.168.1) represent the network portion, and the last octet (100) represents the host portion. The subnet mask "255.255.255.0" indicates that the first 24 bits (3 octets) are used for the network part, and the remaining 8 bits (1 octet) are used for the host part.

Question 7: What is the difference between Authentication and Authorization?

Ans: Authentication and authorization are two fundamental concepts in computer security and access control, while they are related, they serve distinct purposes.

Authentication:

Authentication is the process of verifying the identity of a user, device or system attempting to access a particular resource or service. Some common methods of authentication includes username and password, Biometric authentication, Two factor authentication or multifactor authentication. Once the authentication process is successful and the system confirms the user's identity, the user is granted access to the system or resource.

Authorization:

Authorization is the process of determining what actions or operations an authenticated user , device or system is allowed to perform once access has been granted.  It involves setting and enforcing access rights and permissions based on the user's identity and the security policies of the system.

In other words, while authentication confirms who you are, authorization determines what you are allowed to do.

For example, after a user is authenticated (by providing the correct credentials), the authorization process determines whether the user has read-only access, read-write access, or no access at all to specific files, folders, or resources.

Question 8: What is gateway?

Ans: In computer networking, a gateway is a network device or software component that serves as an entry or exit point for data traffic between different networks.It acts as an intermediary that facilitates communication and data exchange between networks with different protocols, addressing schemes, or architectures.Gateways are essential for connecting networks that are not directly compatible with each other, allowing them to communicate and exchange data seamlessly. They perform protocol translation, address translation, and other functions to enable data transfer across network boundaries.

Question 9: What is the difference between broad casting and multicasting?

Ans: Broadcasting and multicasting are two methods of transmitting data across a computer network, and they differ in their scope and the number of recipients they target:

Broadcasting: 

Broadcasting is a data transmission method in which a single sender sends a message to all devices on the network and every device connected to the network receives and process the message.

Charateristics of broadcasting:

* Broadcast messages are sent to the network's broadcast address, which is special address that encompasses all devices on the network.
* In modern networks, broadcasting is typically limited to the local network segment or LAN(Local Area Network).
* Broadcasting can be useful for certain network management tasks or for disseminating time-sensitive information, but it can also create unnecessary network traffic and pose security risks if not used judiciously.

  Multicasting:

Multicasting is a data transmission method  in which a single sender sends a message to a specific group of recipient devices that have expressed interest in receiving that message. It is a "one-to-many" communication method, where the sender sends the data to a predetermined group of devices, rather than broadcasting to the entire network.

Characteristics of multicasting:

* Multicast messages are sent to a special group address, called a multicast group address. Devices that wish to receive the multicast data must join the multicast group by registering their interest with the network.
* Multicasting is efficient and scalable as it avoids unnecessary data transmission to devices that are not interested in receiving the data.
* Multicasting is commonly used for multimedia streaming, video conferencing, software updates, and other applications that require data distribution to a specific group of recipients.
* Unlike broadcasting, multicasting requires network support (such as multicast-capable routers) to ensure that the multicast data is correctly forwarded to the devices that have joined the multicast group.

In summary, broadcasting is a method where a single message is sent to all devices on the network, while multicasting is a method where a single message is sent to a specific group of devices that have expressed interest in receiving that message. 


