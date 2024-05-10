<h1>Device Addressing</h1>

In a LAN (Local Area Network), devices are identified using unique addresses. These addresses can be either physical or logical.

Physical addresses, also known as MAC (Media Access Control) addresses, are assigned to network interface cards (NICs) by the manufacturer. They are globally unique and consist of six pairs of hexadecimal digits.

Logical addresses, such as IP (Internet Protocol) addresses, are assigned to devices by the network administrator. They provide a hierarchical structure for routing and identifying devices on a network.

## Communication on a LAN

Communication on a LAN involves the exchange of messages between devices. This communication can be achieved through various protocols, such as Ethernet.

Ethernet uses a combination of addressing, framing, and error detection mechanisms to ensure reliable data transmission within a LAN.

## Types of Messages

Different types of messages can be exchanged on a LAN. Some common message types include:

- Unicast: A message sent from one device to another specific device.
- Broadcast: A message sent from one device to all devices on the LAN.
- Multicast: A message sent from one device to a specific group of devices on the LAN.

Good to know!! ^

---

## Handling LAN Traffic

Different network devices handle LAN traffic in various ways. Switches, for example, use MAC addresses to forward traffic only to the intended recipient. Routers, on the other hand, use logical addresses to route traffic between different LANs.

## Learning Who's Who

Devices on a LAN learn about each other's addresses through a process called address learning. Switches, for instance, build a MAC address table by examining the source MAC addresses of incoming frames. This table is then used to forward traffic efficiently.

## Challenges of Shared Physical Medium

In a LAN, multiple devices share the same physical medium, which can lead to collisions and congestion. To address these challenges, LAN technologies employ techniques like CSMA/CD (Carrier Sense Multiple Access with Collision Detection) to detect and handle collisions, and switches to segment the LAN into smaller collision domains.

- CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance) is a technique used in wireless LANs to avoid collisions by having devices wait for a clear channel before transmitting. It aims to prevent collisions by avoiding transmission when other devices are already transmitting.

- CSMA/CD (Carrier Sense Multiple Access with Collision Detection) is a protocol used in Ethernet networks to control access to the network medium and handle collisions when multiple devices try to transmit data simultaneously. It detects collisions by listening to the network while transmitting and stops transmission if a collision is detected.

Mainly Know These Ones ^

---

- Token Passing: In this technique, a token is passed around the network, and only the device holding the token is allowed to transmit data. This helps in avoiding collisions and controlling access to the shared medium.

- Polling: In polling, a central device (such as a hub or a switch) controls the access to the shared medium by sequentially polling each device and allowing them to transmit data when it's their turn.

- Reservation-based protocols: These protocols allow devices to reserve a specific time slot for transmitting data, ensuring that collisions are avoided.

- Virtual LANs (VLANs): VLANs allow the logical segmentation of a LAN into multiple virtual LANs, each with its own broadcast domain. This helps in reducing collisions and improving network performance.

## Connectionless

Connectionless refers to the communication mode used by the Internet Protocol (IP). In a connectionless communication mode, each packet is treated as an independent unit and is routed separately based on the destination IP address. There is no established connection or ongoing session between the sender and receiver. Each packet is individually addressed and delivered to its destination without any guarantee of delivery or order.

Could be helpful? ^
