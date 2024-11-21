# 1.2.1 Olika nätverk i hem

# 1.2.2 Fysiska medier

## Twisted-Pair Copper Wire
- kostar lite
- 10 Mbps till 10 Gbps
## Unshielded twisted pair (UTP)
[![Unshielded Twisted Pair (UTP) is a ubiquitous type of copper cabling](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTCXg2zolucQGWFTL5wOy3Aoh0cSqjxfJTF5Q&s)

## Coaxial Cable
[![What is a coaxial cable? A definition from WhatIs.com](https://www.techtarget.com/rms/onlineImages/networking-coaixal_cable_01_mobile.jpg)

## Fiber Optics
- Immune to electromagnetic interference
- A single optical fiber can support tremendous bit rates
[![Top 10 Advantages of Fiber Optic Internet Connections | HP® Tech Takes](https://store.hp.com/app/assets/images/uploads/prod/top-10-advantages-of-fiber-topic-internet-connections-hero1566844551360542.jpg)

## Terrestrial Radio Channels
- no physical wire to be installed
- can penetrate walls
- can carry a signal for long distances

3 kategorier:
1. Short distance
2. Local areas
3. Wide areas

[![Terrestrial Network - an overview | ScienceDirect Topics](https://ars.els-cdn.com/content/image/3-s2.0-B9780128239780000101-f06-05-9780128239780.jpg)

## Satellite Radio Channels
A communication satellite links two or more Earth-based microwave transmitter/ receivers, known as ground stations. The satellite receives transmissions on one frequency band, regenerates the signal using a repeater 
### 1. Geostationary satellites
- Fast på 1 ställe i atmosfären
- Hög hastighet, används i ställen där kabel internet inte finns.
### 2. LEO satellites
- Åker runt jorden
- kommunicerar med andra satellites




# 1.3 The Network Core

# 1.5 Protocol Layers and Their Service Models
![[Pasted image 20241121125152.png]]

*A*ll *P*eople *S*eem *T*o *N*eed *D*ata *P*rocessing
## Application Layer
- Message/Data
- SMTP(Email), HTTP
## Transport Layer
- Segment
- Provides logical communication between processes, offering services like reliable data transfer (TCP) or connectionless communication (UDP).
- Port Numbers
## Network Layer
- Datagram
- Handles routing and forwarding of datagrams across networks, using IP for addressing and routing protocols like OSPF and BGP.
## Data Link
- Frames
- MAC address
- Switches
- Ensures data transfer between neighboring network nodes, including error detection and handling using protocols like Ethernet and Wi-Fi.
##  Physical
- Deals with the physical transmission of bits over a medium like copper wires, fiber optics, or wireless channels
## Questions:
### **R22**: If two end-systems are connected through multiple routers and the data-link level between them ensures reliable data delivery, is a transport protocol offering reliable data delivery between these two end-systems necessary? Why?
```
Yes, a transport protocol offering reliable data delivery is still necessary. The data-link layer ensures reliable delivery only on a hop-by-hop basis between adjacent nodes. It does not guarantee end-to-end reliability across multiple routers. A transport protocol like TCP provides end-to-end reliability, ensuring proper sequencing, retransmission of lost packets, and congestion control, which the data-link layer cannot handle on a global scale​
```
### ### **R24**: What do encapsulation and de-encapsulation mean? Why are they needed in a layered protocol stack?
```
- **Encapsulation**: At the sender's end, data from a higher layer is wrapped with protocol-specific headers or trailers at the lower layer. For example, an application-layer message is encapsulated into a transport-layer segment, which is then encapsulated into a network-layer datagram, and so on.
- 
- **De-encapsulation**: At the receiver's end, each layer processes and removes its headers or trailers to extract the payload for the higher layer.
- **Importance**: Encapsulation ensures modularity and abstraction in networking, enabling each layer to add its own control information. This layered approach simplifies networking tasks and promotes interoperability across different hardware and software​
```

### R25: Layers Processed by Different Devices
- **Router**: Processes layers 1 (Physical), 2 (Link), and 3 (Network).
- **Link-layer Switch**: Processes layers 1 (Physical) and 2 (Link).
- **Host**: Processes all five layers (Physical, Link, Network, Transport, and Application)​

# 1.7 History

