# [[2023-01-10.pdf]]
![[Pasted image 20241119171143.png]]
Congestion at the Transport layer means  
that there is too much Traffic for the  
receiver to handle. It can cause packet loss  
which means that data which is supposed  
to arrive doesn’t, it lowers the bandwidth,  
increases latency and decreases the  
reliability.  

**To avoid this TCP uses these techniques:**  

- **Flow control:** Uses a window size to send packets with, this window size is determined  by the receiver. Sender sends packet with a determined window size and waits for a updated window size from the receiver.

- **Buffering:** The receiver has a buffer with a Size. This buffer stores packets so the receiver can handle these later.  

- **Acknowledgement (ACK):** The sender waits to send more packets Until it has received an “ACK” from the receiver to send more data  

- **“Slow Start”:** Sender starts by sending small amount of data and then increase it untill congestion occurs, it then reduces amount Sent.
# [[2023-08-25.pdf]]
![[Pasted image 20241119171212.png]]

# [[2024-04-03.pdf]]
![[Pasted image 20241119171231.png]]
# [[2024-08-22.pdf]]
![[Pasted image 20241119171247.png]]