# What is Networking?
- In computing, networking is connection of devices such as workstations, smart phones etc.. Networks can be formed from 2 devices to 1 billion. Networking helps devices to communicate, transfer data and 
share resources.
- There are two types of networks, Private(small networks) and Public networks(networks connecting small networks).

# What is Internet?
- It is a giant network that consists of many and many snall networks. 

# How are devices Indentified on a Network?
- Devices can be identified on a network by 2 kinds of addresses that are as follows:
	1. IP (Internet Protocol) Address
	2. MAC (Media Access Control) Address

##1. IP Address:
- IP address can used to identify a device on a network for a short period of time, after which the same IP address can be associated with another device on the same network.
- It is important to know that IP may change from device to device in a network but it cannot be simultaneously active on more than one device.
- The IP address is divided into four octets.
	*192.168.1.12*
- Look at the above example, here '192' is octet 1; '168' is octet 2 and so on till octet 4. 
- IP address for private network will differ from other devices in the same network. If I wan't to connect a laptop with printer and they are both in the private network, the IP address of both differ.
- IP address used for public network will be the same for devices in the same private network. If I am to send data to the internet from 2 devices from my home networkm, then the IP address for both would 
be seen the same.
- IP address can be calculated by the method known as IP addressing or subnetting.

##2. MAC Address:
- Every device has it's own unique MAC address.
- It is embedded into the motherboard.
- It is 12 character hexadecimal number.
	*a4:c3:f0:85:ac:2d*
- Look at the above example of MAC address. the first 6 characters (a4:c3:f0) represent the vendor name who produced the network interface (intel) and the next 6 characters are unique address of network 
interface.
- So from this, we can say that a person cannot hide his MAC address or he cannot fake it. But no.
- The MAC address can be faked or 'spoofed' via the process known as 'spoofing'. By this, the device pretends to identify as another device using it's MAC address. 
- This can be proved harmful for weak security designs and can result in security breaches.

# Ping:
- It is the most fundamental tools in networking and by default comes with the operating system like linux or windows.
- It uses ICMP (Internet Control Message Protocol) to identify the performance of connection between devices.
- The syntax to do simple ping is *ping (IP address or Website)*.

# What confused me?
- At first I was confused how ping actually works in background. And after some research that the ping sends ICMP Echo request to target IP address and then sends a ICMP Echo Reply to measure network latency.
