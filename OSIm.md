<h1>OSI Model</h1>

The OSI (Open Systems Interconnection) model is a conceptual framework that standardizes the functions of a communication system into seven different layers. Each layer has a specific set of responsibilities and interacts with the layers above and below it. The layers of the OSI model are as follows:

## 1. Physical Layer

The physical layer is responsible for the transmission and reception of raw data bits over a physical medium. It deals with the electrical, mechanical, and physical aspects of the communication.

## 2. Data Link Layer

The data link layer provides reliable and error-free transmission of data frames between two adjacent nodes on a network. It handles framing, error detection and correction, and flow control.

## 3. Network Layer

From the Transport Layer, it passes segments to the Network Layer

The network layer is responsible for the delivery of packets from the source to the destination across multiple networks (i.e: from one computer to another located in different networks). It deals with routing, logical addressing, and congestion control.

Data units in this layer are called <b>Packets</b>.

Functions for the Network Layer include logical addressing, path determination and routing.

### Logical Addressing:

Ip addressing done in the Network Layer is caleed Logical <b>Addressing</b> (IPv4 & IPv6 + Subnet Mask)

The Network Layer assigns senders and recievers IP addresses to each segment to formulate the packet, IP addressing are assigned in sure so that each data packet can reachthe correct destination.

### Routing:

Is the method of moving the <b>Data Packet</b> from source to destination and it is based on the <b>Logical Addressing</b> format of IPv4 or IPv6.

Let's say from device B a request to access GitHub is sent ot the GitHub server which has a unique IP address, it then replies with the packet being sent to device B's unique IP address to make sure only that device has access to the page. the <b>Network Layer</b> of the server has already assigned a sender and reciever IP address in the packet, let's say the mask is 225.225.225.0, the first combination represents the network and the lst combination represents the device in the network

## 4. Transport Layer

The transport layer ensures reliable and efficient end-to-end delivery of data between hosts. It provides services such as segmentation, error control, flow control, connection and connectionless transmission.

### Segmentation:

Segmentation in the transport layer involves breaking down a large data stream into smaller segments. This is done to improve efficiency and reliability during transmission. Each segment is assigned a sequence number for proper reassembly at the receiving end.

### Error Control:

When pieces of data never arrive to it's destination, it uses <b>Automatic Repeat Requests</b> to retransmit the lost or corrupted data. A group of pairs called <b>Checksum</b> is added to each segment by the transport layer to check for corrupted data.

### Flow Control:

When a device (like a server) is transmitting data to another device (like a phone) it allows to send a signal to regulate the traffic. If the server can transfer data at 100mbp/s but the phone can only recieve 20mbp/s, the phone will send a signal to decrease the transfer rate to minimize lost data, likewise if it needs to increase transfer rate to maintain device efficiency.

### Protocols:

- Connection-oriented Teansmission -> Transmission Control Protocol (TCP)
- Connectionless Transmission -> User Datagram Protocol (UDP)

UDP is slower than TCP as there is no feedback, but due to that lost data can only be trnasmitted in TCP
Hence UDP is used for things that we don't require the full picture like: Streaming, Music, Games, VoiP, DNS.
While TCP is used for when all the information is needed like: WWW, Emails, File Transfer Protocol (FTP).

Learning till Here for exam ^

---

## 5. Session Layer

The session layer establishes, manages, and terminates communication sessions between applications. It handles session setup, synchronization, and checkpointing.

## 6. Presentation Layer

The presentation layer is responsible for the formatting and representation of data exchanged between applications. It deals with data encryption, compression, and protocol conversion.

## 7. Application Layer

The application layer provides services directly to the end-user applications. It includes protocols for specific applications such as HTTP, FTP, SMTP, etc.
