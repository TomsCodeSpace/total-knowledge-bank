# Practice Lab: Star topology with a server

# Initial Build

### Equipment and Cabling

The network was constructed in Cisco Packet Tracer using the following components:

| Quantity | Component | Purpose |
| --- | --- | --- |
| 4 | PC-PT | Client workstations |
| 1 | Server-PT (`SRV1`) | Centralized server |
| 1 | Cisco 2960 (`SW1`) | Layer 2 Ethernet switching |
| 5 | Copper Straight-Through cables | Connect end devices to the switch |

Each workstation and the server were connected to a dedicated port on the central switch, forming a **star topology**.

### IPv4 Addressing Configuration

The network was configured using the private IPv4 subnet `192.168.10.0/24`.

| Device | IPv4 Address | Subnet Mask |
| --- | --- | --- |
| PC1 | `192.168.10.10` | `255.255.255.0` |
| PC2 | `192.168.10.11` | `255.255.255.0` |
| PC3 | `192.168.10.12` | `255.255.255.0` |
| PC4 | `192.168.10.13` | `255.255.255.0` |
| SRV1 | `192.168.10.100` | `255.255.255.0` |

**Configuration procedure:**

1. Open each end device in Cisco Packet Tracer.
2. Navigate to **Desktop → IP Configuration**.
3. Select **Static** addressing.
4. Enter the corresponding IPv4 address and subnet mask.
5. Leave the default gateway and DNS server fields blank because neither is required for this initial same-subnet connectivity test.

### Connectivity Testing and Verification

Connectivity was tested using ICMP Echo Requests through the `ping` command.

| Test | Destination | Purpose |
| --- | --- | --- |
| Server connectivity | `192.168.10.100` | Verify communication between a client workstation and the centralized server. |
| Client connectivity | `192.168.10.12` | Verify communication with the workstation configured at this address (PC3, if the addressing table was followed). |

**Verification procedure:**

1. Open the source device's **Desktop → Command Prompt**.
2. Execute `ping` followed by the destination IPv4 address.
3. Review the responses to determine whether packets were successfully received.
4. Record the results and capture screenshots for project documentation.

### Topology Diagram

Insert the completed Cisco Packet Tracer topology screenshot below.

**Figure 1.** Star topology with four client workstations and one centralized server connected through a Cisco 2960 switch.

![image.png](image.png)

![image.png](image%201.png)

# Troubleshoot Scenario

### Overall Scenario

I and other employees have a small office network of 4 computers and a server. I’m from `PC0` and I’m disconnected from the server `SRV1` . The server is in an old janitor closet that’s locked and the business owner is the only one with a  key to it and went early to lunch.

## From `PC0` (PC)

- I have determined The PC is still on
    
    ![image.png](image%202.png)
    
- I pinged `Laptop0`  at 192.168.10.11 | Output: Both Computers are and talking to each other

![image.png](image%203.png)

- We pinged the other 2 computers on the network `PC1` and `Laptop1`

![image.png](image%204.png)

## From `SW1` (Switch)

We realize we still have access to the switch. We’re at the switch now.

We tested the switch with this command:

```
show interfaces status
```

This is the output:

- Only 4 devices are connected

![image.png](image%205.png)

We pinged all of the computers again this time CLI open on the switch simultaneously (with the below command) and by matching the ports with the mac addresses with the computers we just now pinged. It’s actually the server that’s disconnected and we call the business owner for the key to the sever.

![image.png](image%206.png)

## From `SRV1` (Server)

We later get access to the server and realize it’s turned off and turn it back on.

![image.png](image%207.png)

We use `PC0`  to ping the server again to see if it works again.

![image.png](image%208.png)

The sever is now greened up again and works.

![image.png](image%209.png)

## What we learned

We can’t ping an IP address from a switch 

A Cisco 2960 is a Layer 2 switch, meaning its primary job is to forward Ethernet frames between devices using MAC addresses, not IP addresses.

![image.png](image%2010.png)