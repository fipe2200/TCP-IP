![[Fråga 3#2024-08-22.pdf]]

---

![[Pasted image 20241227115420.png]]
![Lightbox](https://media.geeksforgeeks.org/wp-content/uploads/20220818183806/s15.png)

---

![[Pasted image 20241227115807.png]]

- IMAP is **stateful** because it maintains a session state, keeping track of the client's mailbox and email interactions.
	1. A client issues the `LOGIN` command to authenticate and start a session.
	2. The client sends the `SELECT` command to open a mailbox.
	3. Subsequent commands, like `FETCH`, are performed within the context of the selected mailbox, and the server keeps track of this state until the session ends.
	
- SMTP is generally **stateless**, as it does not retain information about the client or previous transactions after an email delivery session ends.
	1. A client connects to an SMTP server to send an email.
	2. The client issues the `MAIL FROM`, `RCPT TO`, and `DATA` commands to transmit the email.
	3. Once the email is accepted and the session ends (via the `QUIT` command), the server does not retain any session state related to the client.

---

![[Pasted image 20241227115821.png]]

Yes, reliable data transfer over UDP is possible by implementing reliability at the application layer. This is achieved using techniques like:

C A S E

1. **Custom Protocols**: Protocols like QUIC provide reliability on top of UDP.
2. **Acknowledgments and Retransmissions**: The receiver confirms packet delivery, and lost packets are resent.
3. **Sequence Numbers**: Ensure packets are received and reordered correctly.
4. **Error Detection**: Checksums detect corruption, prompting retransmission.

---


![[Fråga 5#2024-08-22.pdf]]

---


![[Fråga 4#2023-01-10.pdf]]

---


![[Fråga 7#2024-08-22.pdf]]

---


![[Fråga 7#2023-01-10.pdf]]

---

![[Fråga 10#2024-08-22.pdf]]

---


![[Fråga 10#2024-04-03.pdf]]