# TCP / IP

TCP (Transmission Control Protocol) is a communication protocol to ensure data is sent and received accurately between devices.

It's a list of rules/standards which are divided into layers.

## Protocols Layers

| Layer Number | Protocol       | What it concerns                                                                 |
| :-----------:|:--------------:|:--------------------------------------------------------------------------------:|
| Layer 4      | Application    | End-user softaware: web browsers, email clients, etc.                            |
| Layer 3      | Transport      | Ports: TCP (80 (HTTP), 443 (HTTPS), 25 (SMTP)), UDP (53 (DNS), 67 (DHCP))        |
| Layer 2      | Internet       | IP Adressing and routing                                                         |
| Layer 1      | Physical       | Physical transmission of data: eg. via Ethernet cables                           |

## LAN

A LAN (Local Area Network) and had a network of devices talking to each others within a limited range.

For eg. your home network has multiples devices talking to each others, like the PC to the printer.

## IP

IP (Internet Protocol) is the logical address of a device in the network allocated by a router.

It helps identifie and locate a device on a LAN. It also allows devices to communicate with each others.

Each device has its unique IP address:
- IPv4 (32-bit): eg. *192.168.1.1*
- IPv6 (128 bit): eg. *2001:0db8:85a3:0000:0000:8a2e:0370:7334*

### IPv4
The IPv4 is seperated between 4 octets:

| 192. 168. 1.     | 1.           |
|:----------------:|:------------:|
| Network Portion  | Host Portion |

### Host
A host is a device like a phone or a computer for eg.
It will always be assigned a usable IP address.

### Network IP Addresses
There are always 2 IP addresses reserved in a network:
1. Network Address (first IP of the network)  
	**192.168.1.0**
2. Broadcast Address (last IP of the network)  
	**192.168.1.255**

Usable IP range:
192.168.1.**1** - 192.168.1.**254**

Here is an example of a LAN:  

![lan example](./img/LAN.png)

# Subnet

A subnet, or subnetwork, is a logical subdivision of an IP network.

The practice of dividing a network into two or more networks is called subnetting.

It is represented by a CIDR notation (subnet mask), like so:  
192.168.1.0 **/24**

## Subnet Mask

A subnet mask is a 32-bit number used in IPv4 networking that helps divide an IP address into two components: the network portion and the host portion.

It determines which part of the IP address identifies the network and which part identifies the device (host) on that network. This concept is key to organizing and securing IP networks.

In decimal:
| 255. 255. 255.   | 0.           |
|:----------------:|:------------:|
| Network Portion  | Host Portion |

Or in binary:
| 11111111. 11111111. 11111111.   | 00000000.           |
|:-------------------------------:|:-------------------:|
| Network Portion                 | Host Portion        |

It is useful to be able to convert to bits and vice-versa in network configuration.
