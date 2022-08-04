# OSI model

The Open Systems Interconnection model (OSI model) is a conceptual model that describes about how application communicate over a network.

OSI model was created by International Organization for Standardization (ISO).

# OSI 7 layers

![OSI seven layers](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9d/OSI_Model_v2.svg/476px-OSI_Model_v2.svg.png?20190104111417 "OSI 7 layers")

Fig-1: OSI seven layers

Data will flow down through the layers in the source computer and then up through the layers in the receiving computer.

# 7. Application layer

Layer where user applications with certain required protocols are used inorder to access the network. It proivides abstraction. Here communication partners are identified. We will get data here.

- PDU - Data
- User applications
- FTP, POP3, SMTP, IMAP, HTTP, DNS
- Electronic mail

# 6. Presentation layer

This layer is all about formatting in such a way that both parties will be able to read it. Application layer has given the data for network but the data is not in a format that the network can move. This layer is usually a part of an operating system (OS).

- PDU - Data
- Formatting, Data encryption/decryption, Compression/Expansion, Syntax
- Content translation
- System-specific translation
- Its like putting letter into an envelope

# 5. Session layer

This layer is responsible for negotiating the parameter and end of the communication. Bringing that session online. So, we can send that information, maintaining the session and tearing the session down once we no longer need them. This layer services include authentication and reconnection after an interruption.

- PDU - Data
- Communication establishment
- Synchronization of data flow
- Acknowledgments of data received during a session

# 4. Transport layer

Here in this layer we choose the protocol that are going to be responsible for actually moving our information throughout the network while maintaining the quality of service functions. This layer manages packetization of data, it breaks long data streams into smaller chunks called "segments".

- PDU - Segment
- Moves data along the network
- Segmenting and sequencing
- TCP, UDP
- Transmission-error detection

# 3. Network layer

This layer is responsible for forwarding our package. IP addresses get attached to network layer. \
Now we got that envelope from above but we cannot do anything with it because we donot know where its going. So we gonna put a mailing address and put return address. Now we know where it came from and where its going to. \
IP says that lets go ahead and take that data packet and will add a header on it and its going to have source ip address and destination ip address. Then we can handle it to router and router can use routing protocols to make sure it hops through the network and gets to the right location.

- PDU - Packet
- Packet forwarding, routing
- Addressing
- IP, ICMP, OSPF, RIP, RIPv2, BGP, EGIRP

# 2. Data link layer

The Data link layer is responsible for providing node-to-node data transfer between two directly connected nodes. After a packet enters in a network its DLL responsibilty to transmit it to the host using its MAC address. \

- PDU - Frame
- Encapsulation of network layer data packets into frames
- Frame synchronization
- Frame Relay
- 802.11
- ATM

Data link layer is divided into two sub-layers:

- Logical Link Control (LLC)
- Media Access Control (MAC)

## 2.1 Logical Link Control (LLC)

LLC provides addressing, error and flow control but this addressing is little different. We are talking about MAC (Media Access Control) adresses.

The MAC address of the receiver host is obtained by broadcasting an ARP(Address Resolution Protocol) request onto the network with MAC address FFFF.FFFF.FFFF and destination IP address and the destination host will reply with its MAC address.

- Error control
- Flow Control

## 2.2 Media Access Control (MAC)

Media Access Control determines who is allowed to access the media.

- Physical addressing
- Virtual LANs (VLAN)

# 1. Physical layer

Physical layer contains the information in form of bits. It is reponsible for converting into required bits such as electrical, radio, optical signals. Here the actual physical connection between devices happens. This layer converts the received signal into 0s and 1s.

- PDU - Bits
- Physical topology
- Hardware, electrical and mechanical characteristics
- DSL, ISDN, SONET/SDH, Frame Relay
- Transmission Mode
- Hub, repeater, cable are physical layer devices

### **Note**

Sometimes some potocol might be in multiple layers. \
eg. TCP which is connection oriented communication so it can be seated in layer 5 (Session) too.
