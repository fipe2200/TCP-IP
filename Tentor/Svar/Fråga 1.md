# [[2023-01-10.pdf]]
![[Pasted image 20241119170216.png]]
- ## Wireless vs wired 
	- **Speed**: wired is usually faster as it is directly connected and is not affected by obstacles and other disturbenes.
	- **Distance**: Wireless can cover more distance, bigger areas but connection is easily affected
	- **Reliability:** Ethernet is usually rare reliable as no other factors than the cable can affect the transmission, less risk for packet loss.
	
- ## The hidden node problem:
	   Occurs when three and more devices are connected, but not every router is connected to each other. For example, lets say we have routers A,B and C:
	  ![[Pasted image 20241121184403.png]]
	  A is connected to both A and C. 
	  But B and C are not connected to each other.
	  B can not know if C is transmitting,
	  C can not know if B is transmitting.
	  Now if both B and C transmits at the same time, a collision occurs.
	  Solution to eliminate the problem is Multiple Access Protocols
- Collision detection:
	  Is used when devices are connected with physical links. In wireless networks devices doesn't have physical links and cannot detect if there was a collision.
	  Instead WLAN'S uses Collision Avoidance, this works by devices listening if the cannel is occupied. 
	  The devices sends a RTS(Request To Send) to the receiver and if they get a CRS(Clear To Send) back, the device occupies the channel and transmits data.
# [[2023-08-25.pdf]]
![[Pasted image 20241119170333.png]]


# [[2024-04-03.pdf]]
![[Pasted image 20241119170429.png]]

# [[2024-08-22.pdf]]
![[Pasted image 20241119170555.png]]
- Error detection and error correction is fundamental for:
		  - Data integrity
		  - Due to unreliable media communication detection and correction is crutial.
		  - Don't affect performance and latency.
	 Ex of error detection is:
		 - Use of bytes
		 - Check sum
		 
- false
- A switch connects multiple devices to a network
  A router connects multiple switches, and their respective networks, to form an even larger network.