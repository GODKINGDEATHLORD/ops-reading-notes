# Reading Class 07: Network Connectivity

## [SSH Protocol](https://www.ssh.com/academy/ssh/protocol#how-does-the-ssh-protocol-work)

1. **What is the Secure Shell (SSH) Protocol?**
Its a way to safely tap in to one computer from another 
2. What are the typical uses of the SSH protocol?
- *providing secure access for the users and the process*
- *file transfers*
- *issuing remote commands*
- *managing a network*
3. **How does the SSH protocol work?**
  
  **This next part might seem lazy, but I utilized chat gpt to find an analogy for ssh protocol and I cant explain it any better :**

"*Imagine you're sending a letter, but you want to make sure it doesn't get intercepted by anyone. So, you put your letter inside a special, super-secure envelope that only you and the recipient can open. You also create a secret code that only you and the recipient know to unlock the envelope.*

*Now, you send this envelope through a public postal system (the internet). Even if someone tries to open it along the way, they can't because it's in that special, secure envelope with your secret code.*"

SSH is where you set up a secure connection between two computers, and make sure all the data sent back, and forth is secure, and protected.


![SSH PROTOCOL ](https://www.ssh.com/hs-fs/hubfs/SSH_Client_Server.png?width=556&name=SSH_Client_Server.png)
  
4. **How is the data kept safe when transmitted between the SSH client and server?**

  ### Strong encryptions such as:
- **Public Keys**~ Ex:*CAC & PIV cards*
  - **Passwords**~*This is the most common*

5. **What is SFTP?**

   SFTP= SSH File Transfer protocol, is the most popular file transfer protocol
------------------------------------------------------------------------------------------------------------------------------------------
## [What is RDP? And how to use it](https://www.comparitech.com/net-admin/what-is-rdp/)

1. **What is Windows Remote Desktop Connection?**

  It allows you to connect, and control one PCs OS, from another. Its kind've like the virtual machine, except the machine isn't virtual
2. **What is RDP?**

"It allows remote users to see, and use windows on a device in another location"
   
3. **What is the RDP port number?**

   *PORT 3389*
