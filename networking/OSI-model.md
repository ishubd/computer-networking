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

This layer is all about formatting in a such a way that both parties will be able to read it. Application layer has given the data for network but the data is not in a format that the network can move. This layer is usually a part of an operating system (OS).

- PDU - Data
- Formatting, Data encryption/decryption, Compression/Expansion, Syntax
- Content translation
- System-specific translation
- Its like putting letter into an envelope

# 5. Session layer

This layer is responsible for negotiating the parameter and end of the communication. Bringing that session online. So, we can send that information, maintaing the session and tearing the session down once we no longer need them. This layer services include authentication and reconnection after an interruption.

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
IP says that lets go ahead and take that data packet and will add a header on it and its gonna have source ip address and destination ip address. Then we can handle it to router and router can use routing protocols to make sure it hops through the network and gets to the right location.

- PDU - Packet
- Packet forwarding, routing
- Addressing
- IP, ICMP, OSPF, RIP, RIPv2, BGP, EGIRP
