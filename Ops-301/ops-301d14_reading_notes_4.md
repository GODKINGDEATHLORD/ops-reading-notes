
[Routing](https://www.nakivo.com/blog/virtualbox-network-setting-guide/)

1. **Which network mode in VirtualBox can be used to emulate unplugging the Ethernet cable from the network?**
 "Not attached: A virtual network adapter is installed in a VM, but the network connection is missing, much like when you unplug the Ethernet network cable when using a physical network adapter."

2. **Which network mode would be best if you wanted to run a server on a VM that could be fully accessible from your physical local area network?**
"Bridged Adapter: This mode is used for connecting the virtual network adapter of a VM to a physical network to which a physical network adapter of the VirtualBox host machine is connected."

3. **What are the three options of promiscuous mode and what does each do?**

"There are three options of using the promiscuous mode: Deny, Allow VMs, Allow All. Deny: Any traffic that is not intended to the virtual network adapter of the VM is hidden from the VM. Allow VMs: All traffic is hidden from the VM network adapter except the traffic transmitted to and from other VMs. Allow All: There are no restrictions in this mode. A VM network adapter can see all incoming and outgoing traffic."

4. **What is Port Forwarding?**
"Port forwarding is a process of intercepting traffic addressed to the appropriate IP address and port in addition to redirecting that traffic to a different IP address and/or port."

