# Lab Report (Small Office Network Setup) (Cisco Packet Tracer)

Created: October 12, 2026 10:39 AM
Class: Networking

# Build + Test — Small Office Network

**Objective:** Build a small office network consisting of one router, one switch, and four PCs.

- **Estimated time:** 20–30 minutes
- **Difficulty:** Beginner
- **Devices:** 1 router, 1 switch, 4 PCs

### Step 1 — Add the network devices

Open Cisco Packet Tracer and place the following devices in a blank workspace:

- 1 × Cisco 1941 Router (`R1`)
- 1 × Cisco 2960 Switch (`S1`)
- 4 × PCs (`PC1`–`PC4`)

Arrange the router at the top, the switch beneath it, and the four PCs along the bottom.

### Step 2 — Connect the devices

Select **Connections → Copper Straight-Through** and establish these five connections:

| Device A | Device B |
| --- | --- |
| R1 — GigabitEthernet0/0 | S1 — FastEthernet0/1 |
| PC1 — FastEthernet0 | S1 — FastEthernet0/2 |
| PC2 — FastEthernet0 | S1 — FastEthernet0/3 |
| PC3 — FastEthernet0 | S1 — FastEthernet0/4 |
| PC4 — FastEthernet0 | S1 — FastEthernet0/5 |

Wait for the switch ports to initialize. Green link indicators generally indicate active connections.

### Step 3 — Configure the router

Open `R1` → **CLI** and enter the following commands:

```
enable
configure terminal
hostname R1
interface gigabitEthernet 0/0
description LAN connection to S1
ip address 192.168.10.1 255.255.255.0
no shutdown
end
```

This assigns the router its LAN gateway address and enables the interface. No switch configuration is required for this basic network.

### Step 4 — Configure the four PCs

For each PC, open **Desktop → IP Configuration**, select **Static**, and enter the appropriate IPv4 address, subnet mask, and default gateway.

| Device | IPv4 Address | Subnet Mask | Default Gateway |
| --- | --- | --- | --- |
| PC1 | 192.168.10.11 | 255.255.255.0 | 192.168.10.1 |
| PC2 | 192.168.10.12 | 255.255.255.0 | 192.168.10.1 |
| PC3 | 192.168.10.13 | 255.255.255.0 | 192.168.10.1 |
| PC4 | 192.168.10.14 | 255.255.255.0 | 192.168.10.1 |

All four PCs use the same `/24` subnet. Each receives a unique IP address, while `192.168.10.1` serves as the default gateway.

### Step 5 — Initial build checkpoint

Before proceeding, confirm that:

- All six devices are present and connected.
- The router has been assigned `192.168.10.1/24`.
- The four PCs have their assigned static IPv4 configurations.
- The router interface has been enabled.

**Next:** Verify the configurations and test connectivity using `ipconfig`, `show ip interface brief`, and `ping`.

# Evidence Taken Verifying that It works

![image.png](image.png)

![image.png](image%201.png)

![image.png](image%202.png)

![image.png](image%203.png)

# Conclusion

Successfully built and configured a small office network in Cisco Packet Tracer using one router, one switch, and four PCs. Assigned static IPv4 addresses, configured the router's default gateway interface, and tested connectivity using `ping`. This project demonstrates foundational networking skills in device configuration, IPv4 addressing, network connectivity, and basic troubleshooting relevant to entry-level IT Specialist and Help Desk roles.
