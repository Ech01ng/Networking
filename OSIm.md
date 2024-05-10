<h1>OSI Model</h1>

The OSI (Open Systems Interconnection) model is a conceptual framework that standardizes the functions of a communication system into seven different layers. Each layer has a specific set of responsibilities and interacts with the layers above and below it. The layers of the OSI model are as follows:

## 1. Physical Layer

The physical layer is responsible for the transmission and reception of raw data bits over a physical medium. It deals with the electrical, mechanical, and physical aspects of the communication.

## 2. Data Link Layer

The data link layer provides reliable and error-free transmission of data frames between two adjacent nodes on a network. It handles framing, error detection and correction, and flow control.

## 3. Network Layer

The network layer is responsible for the delivery of packets from the source to the destination across multiple networks. It deals with routing, logical addressing, and congestion control.

## 4. Transport Layer

The transport layer ensures reliable and efficient end-to-end delivery of data between hosts. It provides services such as segmentation, error control, and flow control.

### Segmentation:

Segmentation in the transport layer involves breaking down a large data stream into smaller segments. This is done to improve efficiency and reliability during transmission. Each segment is assigned a sequence number for proper reassembly at the receiving end.

### Error Control:

When pieces of data never arrive to it's destination, it uses <b>Automatic Repeat Requests</b> to retransmit the lost or corrupted data. A group of pairs called <b>Checksum</b> is added to each segment by the transport layer to check for corrupted data.

### Flow Control:

When a device (like a server) is transmitting data to another device (like a phone) it allows to send a signal to regulate the traffic. If the server can transfer data at 100mbp/s but the phone can only recieve 20mbp/s, the phone will send a signal to decrease the transfer rate to minimize lost data, likewise if it needs to increase transfer rate to maintain device efficiency.

Learning till Here for exam ^

---

## 5. Session Layer

The session layer establishes, manages, and terminates communication sessions between applications. It handles session setup, synchronization, and checkpointing.

## 6. Presentation Layer

The presentation layer is responsible for the formatting and representation of data exchanged between applications. It deals with data encryption, compression, and protocol conversion.

## 7. Application Layer

The application layer provides services directly to the end-user applications. It includes protocols for specific applications such as HTTP, FTP, SMTP, etc.
