# cybersecurity-task-4

Objective
The goal of this task was to set up and use a firewall on a Linux system to configure and test basic rules for blocking and allowing network traffic. I used `ufw` (Uncomplicated Firewall) to achieve this.

---

Steps Taken

I performed the following steps to complete the task, documenting the process with screenshots.

1. Blocked Inbound Traffic on Port 23 (Telnet)
   I first checked the status of the firewall and then added a rule to block inbound traffic on TCP port 23, which is used by the insecure Telnet protocol.
    
2.  Tested the Block Rule
    To confirm the rule was working, I attempted to connect to port 23 locally using the `telnet` command. The connection was successfully refused, proving that the firewall rule was active.
    
3.  Allowed SSH Traffic on Port 22
    To demonstrate how to allow specific traffic, I added a rule to permit incoming SSH connections on TCP port 22.

4.  Removed the Test Rule
    Finally, I removed the blocking rule for port 23 to restore the firewall's original configuration.


Summary of How a Firewall Filters Traffic
A firewall acts as a security guard for a network, inspecting incoming and outgoing data packets. It uses a set of rules to decide whether to allow, deny, or drop the packets based on their characteristics, such as the source/destination IP address, port number, and protocol. By controlling this traffic, a firewall prevents unauthorized access and protects the network from malicious activity.
