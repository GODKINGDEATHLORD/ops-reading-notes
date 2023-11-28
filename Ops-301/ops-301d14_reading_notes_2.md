# [What is a Port Scanner and How Does it Work?](https://www.varonis.com/blog/port-scanning-techniques/)

1. **What is a port? Describe it with an analogy that would help a family member understand.**
It is a virtual point where a network connection starts and ends. A port is like a house in a large gated couldesac. In the front you have a realator (ip address) and a security guard(firewall) a large majority of the homes are occupied. All of the houses have unique house numbers , and unique residents that live within the house holds 

2. **What does a port scanner send to a port to check the current status?**
It sends a network request to connect to a speciefic tcp or UDP on a computer
3. **When a port scanner sends a request to connect, what are the three possible responses? Describe them.**
- Open = Accepted
- Closed = Not listening
- Filtered = dropped , blocked , silence, will recieve no repsponse 
4. **What is the difference between TCP and UDP?**
Transmission control protocol
"TCP sends each packet in order, complete with error checking, verification, and a 3-way handshake to confirm each packet is successful."
User Diagram Protocol 
"doesn’t have any error checking but tends to be faster,a connectionless protocol, so programs that use UDP just send the data – and if you miss a packet, you will never get it again"
# [Common Ports](https://www.professormesser.com/network-plus/n10-008/n10-008-video/common-ports-n10-008/)
*List and describe the ports used for the following:*

- **Telnet**-Telnet, the telecommunication network protocol, uses TCP port 23. It allows for a console connection to a remote device but lacks encryption, making it less secure​
- **SSH**- Secure shell, SSH operates over TCP port 22, providing a secure method for terminal communication with encryption, making it a safer alternative to Telnet for accessing switches, routers, firewalls, and servers
- **DNS**- Domain Name System , DNS typically uses UDP port 53 for translating domain names to IP addresses. However, in cases of large data transfers, DNS might use TCP, but still on port 53​
- **SMTP**- Simple Mail Transfer Protocol, SMTP, used for sending emails, typically uses TCP port 25 for plaintext communications. For encrypted communications using TLS, TCP port 587 is commonly used
- **HTTP**- Hypertext transfer protocol, HTTP uses TCP port 80 for non-encrypted web communication.
- **HTTPS**- Hypertext transfer protocol secure , uses TCP port 443, which historically used SSL (Secure Sockets Layer) and now often employs TLS (Transport Layer Security) for encryption
- **RDP**- Remote desktop protocol , RDP, used in Windows systems for remote desktop access, operates over TCP port 338
- **Ping**-