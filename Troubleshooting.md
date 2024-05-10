<h1>Troubleshooting</h1>

## ICMP

ICMP, which stands for Internet Control Message Protocol, is a network protocol used for diagnostic and troubleshooting purposes in computer networks. It operates at the network layer of the TCP/IP protocol suite and is closely associated with the Internet Protocol (IP).

- ICMP works by sending control messages between network devices, such as hosts and routers, to communicate various types of information. These messages are typically used to report errors, provide feedback, or exchange operational information.

Probably should know this ^

---

- Error Reporting: One of the primary functions of ICMP is to report errors. For example, if a network device encounters a problem while trying to deliver an IP packet, it can send an ICMP error message back to the source host. This error message provides information about the issue, such as the type of error and the affected network device.

- Echo Request and Reply: ICMP also supports the "echo request" and "echo reply" messages, commonly known as "ping." When a host sends an ICMP echo request to another host, it expects an ICMP echo reply in return. This mechanism is often used to test network connectivity and measure round-trip time (RTT) between hosts.

- Time Exceeded: ICMP includes a "time exceeded" message that is used when a packet exceeds its time-to-live (TTL) value. This message is sent back to the source host to indicate that the packet was discarded due to reaching its TTL limit. It helps identify network routing issues or loops.

- Redirect: ICMP can also be used to send "redirect" messages. When a router receives a packet that could have been sent on a better route, it can send an ICMP redirect message to the source host, suggesting a more efficient route to reach the destination.
