# Understanding-IP-Addresses-and-CIDR-Notation

## IP Addresses and CIDR Notation Demystified: 

## A Comprehensive Guide Description: 

Welcome to the IP Addresses and CIDR Notation Demystified Course, a comprehensive program designed to provide you with a clear understanding of IP addresses and CIDR (Classless Inter-Domain Routing) notation. 

Whether you're a network administrator, IT professional, or simply interested in networking concepts, this course will guide you through the essentials of IP addressing and CIDR notation. 

Tailored for beginners, this course takes you on a step-by-step journey into the world of IP addresses and CIDR notation. You'll learn the fundamentals of IP addressing, including IPv4 and IPv6 address formats, subnetting, and the importance of IP addressing in network communication.
Through practical examples and interactive exercises, you'll gain proficiency in working with CIDR notation, which allows for flexible allocation of IP address ranges. You'll explore CIDR subnet masks, learn how to calculate subnets, and understand how CIDR notation enables efficient address space utilization. As part of the course, you'll delve into advanced topics such as IP routing, network segmentation, and address allocation strategies. You'll gain insights into the hierarchy of IP addressing, IP classes, and the role of CIDR notation in modern network design. Our experienced instructor will provide expert guidance and insights, sharing practical tips and real-world scenarios to enhance your understanding of IP addressing and CIDR notation. You'll have the opportunity to ask questions, engage in discussions, and deepen your knowledge of networking concepts.
By the end of this course, you'll possess a solid understanding of IP addresses and CIDR notation, enabling you to effectively manage and design networks. Whether you're configuring network devices, troubleshooting connectivity issues, or planning network infrastructure, you'll be equipped with the knowledge to make informed decisions and ensure efficient IP address utilization. Journey into the world of IP addresses and CIDR notation, and unlock the potential to navigate networking challenges with confidence. Enroll now and take the first step towards mastering IP addressing and CIDR notation for efficient network management.

# Introduction to IP Addresses

An IP address is a unique address that identifies a device on the internet or a local network. IP stands for "Internet Protocol," which is the set of rules governing the format of data sent via the internet or local network. In essence, IP addresses are the identifier that allows information to be sent between devices on a network: they contain location information and make devices accessible for communication. The internet needs a way to differentiate between different computers, routers, and websites. IP addresses provide a way of doing so and form an essential part of how the internet works.

## What is an IP Address?

An IP address is a string of numbers separated by periods. IP addresses are expressed as a set of four numbers - an example address might be 192.158.1.38. Each number in the set can range from 0 to 255. So, the full IP addressing range goes from 0.0.0.0 to 255.255.255.255. IP addresses are not random. They are mathematically produced and allocated by the Internet Assigned Numbers Authority (IANA), a division of the Internet Corporation for Assigned Names and Numbers (ICANN). ICANN is a non-profit organization that was established in the United States in 1998 to help maintain the security of the internet and allow it to be usable by all. Each time anyone registers a domain on the internet, they go through a domain name registrar, who pays a small fee to ICANN to register the domain.

![ip address](<images/ip address.jpg>)

## Subnetting and Subnet Masks

## What is Subnetting?

Subnetting is the practice of dividing a network into two or smaller networks. It increases routing efficiency, which helps to enhance the security of the network and reduces the size of the broadcast domain.
IP Subnetting designates high-order bits from the host as part of the network prefix. This method divides a network into smaller subnets.
It also helps you to reduce the size of the routing tables, which is stored in routers. This method also helps you to extend the existing IP address base & restructures the IP address.[]

![subnetting](images/subnetting.jpg)

## What is Subnet Mask? 

A subnet mask is a 32 bits address used to distinguish between a network address and a host address in IP address. A subnet mask identifies which part of an IP address is the network address and the host address. They are not shown inside the data packets traversing the Internet. They carry the destination IP address, which a router will match with a subnet.


# CIDR Notation and Address Aggregation

## What is CIDR?

Classless Inter-Domain Routing (CIDR) is an IP address allocation method that improves data routing efficiency on the internet. Every machine, server, and end-user device that connects to the internet has a unique number, called an IP address, associated with it. Devices find and communicate with one another by using these IP addresses. Organizations use CIDR to allocate IP addresses flexibly and efficiently in their networks.

![cidr table](<images/cidr table.jpg>)

## IP Address Aggregator

IP Address Aggregator is a utility developed to automate minimization process and convert bunch of IPv4 addresses into smallest continuous range(s) possible. IP
aggregation is commonly performed by network engineers working with BGP & routers. This utility will help webmasters to configure server firewalls, apache.htaccess files, address masks and so on.

### Basic Usage

IP Address Aggregation Tool accepts various IP address formats for input (scroll to Input Format Examples for more details). Enter IP Address list in a block of text (one IP Address or range per line) into IP Address Ranges input area. Select desired output format and click submit button. It will automatically discard any non-recognized or invalid address text.
Once processed click on Copy To Clipboard button to directly copy results into memory and paste it anywhere else

# IP Address Classes and Private IP Address Ranges

## What is Classful Addressing?

Classful addressing is a network addressing the Internet's architecture from 1981 till Classless Inter-Domain Routing was introduced in 1993.
This addressing method divides the IP address into five separate classes based on four address bits.
Here, classes A, B, C offers addresses for networks of three distinct network sizes. Class D is only used for multicast, and class E reserved exclusively for experimental purposes.

![classes](images/classes.jpg)

Let's see each of the network classes in detail:

## Class A Network

This IP address class is used when there are a large number of hosts. In a Class A type of network, the first 8 bits (also called the first octet) identify the network, and the remaining have 24 bits for the host into that network.
An example of a Class A address is 102.168.212.226. Here, "102" helps you identify the network and 168.212.226 identify the host.
Class A addresses 127.0.0.0 to 127.255.255.255 cannot be used and is reserved for loopback and diagnostic functions.

## Class B Network

In a B class IP address, the binary addresses start with 10. In this IP address, the class decimal number that can be between 128 to 191. The number 127 is reserved for loopback, which is used for internal testing on the local machine. The first 16 bits (known as two octets) help you identify the network. The other remaining 16 bits indicate the host within the network.
An example of Class B IP address is 168.212.226.204, where 168 212 identifies the network and 226.204 helps you identify the Hut network host.
## Class C Network

Class C is a type of IP address that is used for the small network. In this class, three octets are used to indent the network. This IP ranges between 192 to 223.
In this type of network addressing method, the first two bits are set to be 1, and the third bit is set to 0, which makes the first 24 bits of the address them and the remaining bit as the host address. Mostly local area network used Class C IP address to connect with the network.
Example for a Class C IP address:
192.168.178.1

## Class D Network

Class D addresses are only used for multicasting applications. Class D is never used for regular networking operations. This class addresses the first three bits set to "1" and their fourth bit set to use for "0". Class D addresses are 32-bit network addresses. All the values within the range are used to identify multicast groups uniquely. Therefore, there is no requirement to extract the host address from the IP address, so Class D does not have any subnet mask. Example for a Class D IP address: 227.21.6.173

## Class E Network

Class E IP address is defined by including the starting four network address bits as 1, which allows you two to incorporate addresses from 240.0.0.0 to 255.255.255.255. However, E class is reserved, and its usage is never defined. Therefore, many network implementations discard these addresses as undefined or illegal.
Example for a Class E IP address:
243.164.89.28

## Limitations of classful IP addressing

Here are the drawbacks/cons of the classful IP addressing method:

1. Risk of running out of address space soon Class boundaries did not encourage efficient allocation of address space Rules for assigning Network ID: 

1. The network ID will be assigned based on the below-given rules:

1. The network ID cannot start with 127 because 127 belongs to class A address and is reserved for internal loopback functions. 

1. All bits of network ID set to 1 are reserved for use as an IP broadcast address and cannot be used. All bits of network ID are set to 0. They are used to denote a particular host on the local network and should not be routed.
























