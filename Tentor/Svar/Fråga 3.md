# [[2023-01-10.pdf]]
![[Pasted image 20241119171008.png]]

![[Pasted image 20250107123944.png]]
# [[2023-08-25.pdf]]
![[Pasted image 20241119171027.png]]

# [[2024-04-03.pdf]]
![[Pasted image 20241119171052.png]]
- **Link state:**
  Link state is a centrelized aproach where the whole network is known when setting up the weights/costs
  Example protocol: OSPF
- **Distance vector:**
  Distance vector on the other hand is when network nodes only are aware of its neighbors
  Example protocol: GPG

- **Static routing:**
  Is when you manually sets up a network connections/weights. This could be preferred if the network is small and you know that it wont change.
- **Dynamic routing:**
  Dynamic routing algorithms automatically set up the networks connections/weights and can switch the routs of one path is overloaded. This also means it easy to add new nodes to the network.
  This is preferred in bigger networks where changes often happen
# [[2024-08-22.pdf]]
![[Pasted image 20241119171113.png]]
- To easily recognize packets
- To equaly divide resources

*Sequence numbers* are introduced to ensure data order and identify duplicate packets, while *timers* are used to manage timeouts and retransmissions for unacknowledged packets.

```
First of RDT stands for realiable data transfer, meaning how do we make sure the reciver gets what the sender sent?

- We introduce sequence numbers to make a "failsafe" incase the NAK or ACK response from the reciver is corrupted. if we didnt have sequance number we would not know what package to send again

- The timer gets introduced to not have to deal with a NAK answer. instead we will only recive a ACK once the package is delivered uncurropted and if we recive nothing the timer will run out and the package will be sent again.
  
  ```
