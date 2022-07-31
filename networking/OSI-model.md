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

# 5. Session layer

This layer is responsible for negotiating the parameter and end of the communication. Bringing that session online. So, we can send that information, maintaing the session and tearing the session down once we no longer need them. This layer services include authentication and reconnection after an interruption.

- PDU - Data
- Communication establishment
- Synchronization of data flow
- Acknowledgments of data received during a session

# 4. Transport layer
