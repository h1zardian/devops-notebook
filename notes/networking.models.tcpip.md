---
id: e84z4c3d83c7y1r01xtk5to
title: TCP/IP
desc: ''
updated: 1678741279619
created: 1678740488534
---

Layers | Protocols
---| --- |
Application | HTTP, FTP, SMTP, DNS
Transport | TCP, UDP
Internet | IP,ICMP, IGMP, ARP
Link | Ethernet, Wi-Fi, PPP

### Key architectural principles

- TCP/IP follows the end-to-end principle, which means that most of the intelligence and functionality is placed at the edge of the network, in the end nodes (the devices that send and receive data). The network itself only provides a basic service of delivering packets from one node to another, without guaranteeing reliability or quality. This makes the network simple and flexible, and allows different types of devices and applications to communicate over it.
- TCP/IP does not strictly follow a layered model, but rather emphasizes on architectural principles. There are four abstraction layers: application, transport, internet, and link. However, these layers are not rigid or fixed, and different protocols can operate across multiple layers or within a single layer. For example, some protocols like ICMP or OSPF are considered to be part of the application layer, even though they are used for network management or routing.
- TCP/IP supports interoperability and scalability, which means that it can work with different types of networks and devices, and can accommodate changes in size and complexity. TCP/IP uses a common addressing scheme (IP addresses) and a common packet format (IP datagrams) to enable communication across different networks. TCP/IP also uses protocols like ARP and DHCP to dynamically assign addresses and resolve them to physical addresses. TCP/IP also uses protocols like TCP and UDP to provide different types of services to applications, such as reliable or unreliable data transmission.
