<h1>Subnetting Summary for IPv4 and IPv6<h1>

## IPv4 Subnetting

IPv4 subnetting is the process of dividing a large network into smaller subnetworks, known as subnets. This allows for efficient utilization of IP addresses and better network management.

### Subnet Mask

A subnet mask is a 32-bit value that is used to divide an IP address into network and host portions. It consists of a series of 1s followed by a series of 0s. The number of 1s in the subnet mask determines the size of the network portion.

Example subnet mask: `255.255.255.0`

### CIDR Notation

CIDR (Classless Inter-Domain Routing) notation is a compact representation of an IP address and its associated subnet mask. It is expressed as `<IP address>/<subnet mask>`.

Example CIDR notation: `192.168.0.0/24`

### Subnetting Example

Let's consider an example where we have the IP address range `192.168.0.0` to `192.168.255.255` and we want to divide it into 4 subnets.

1. Determine the number of bits required for the subnet mask. In this case, we need 2 bits to represent 4 subnets (`2^2 = 4`).

2. Create the subnet mask by setting the required number of bits to 1 and the remaining bits to 0. In this case, the subnet mask would be `255.255.192.0`.

3. Divide the IP address range into subnets based on the subnet mask.

   - Subnet 1: `192.168.0.0/18`
   - Subnet 2: `192.168.64.0/18`
   - Subnet 3: `192.168.128.0/18`
   - Subnet 4: `192.168.192.0/18`

## IPv6 Subnetting

IPv6 subnetting follows a similar concept to IPv4 subnetting, but with some differences due to the larger address space.

### Subnet Prefix

In IPv6, a subnet prefix is used to divide the address space into subnets. It consists of a network prefix followed by a subnet ID.

Example subnet prefix: `2001:0db8:85a3::/48`

### Subnetting Example

Let's consider an example where we have the IPv6 address range `2001:0db8:85a3::/48` and we want to divide it into 8 subnets.

1. Determine the number of bits required for the subnet ID. In this case, we need 3 bits to represent 8 subnets (`2^3 = 8`).

2. Create the subnet prefix by setting the required number of bits for the subnet ID and the remaining bits for the network prefix. In this case, the subnet prefix would be `2001:0db8:85a3:0000::/51`.

3. Divide the IPv6 address range into subnets based on the subnet prefix.

   - Subnet 1: `2001:0db8:85a3:0000::/51`
   - Subnet 2: `2001:0db8:85a3:2000::/51`
   - Subnet 3: `2001:0db8:85a3:4000::/51`
   - Subnet 4: `2001:0db8:85a3:6000::/51`
   - Subnet 5: `2001:0db8:85a3:8000::/51`
   - Subnet 6: `2001:0db8:85a3:a000::/51`
   - Subnet 7: `2001:0db8:85a3:c000::/51`
   - Subnet 8: `2001:0db8:85a3:e000::/51`
