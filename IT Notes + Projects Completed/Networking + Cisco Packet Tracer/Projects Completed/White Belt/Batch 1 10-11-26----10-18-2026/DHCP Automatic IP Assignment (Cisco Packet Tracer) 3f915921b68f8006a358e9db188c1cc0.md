# DHCP Automatic IP Assignment (Cisco Packet Tracer)

Created: October 14, 2026 10:13 AM
Class: Networking

# Build + Test— DHCP Automatic IP Assignment

**Objective:** Configure a router to automatically assign IPv4 addresses to three office PCs using DHCP.

- **Estimated time:** 45–75 minutes
- **Difficulty:** Beginner
- **Devices:** 1 router, 1 switch, 3 PCs

### Step 1 — Add and Connect Devices

Open Cisco Packet Tracer and add:

- 1 × Cisco 2911 Router (`R1`)
- 1 × Cisco 2960 Switch (`S1`)
- 3 × PCs (`PC-1`, `PC-2`, `PC-3`)

Select **Connections → Copper Straight-Through** and establish these connections:

| Device A | Device B |
| --- | --- |
| R1 — GigabitEthernet0/0 | S1 — GigabitEthernet0/1 |
| PC-1 — FastEthernet0 | S1 — FastEthernet0/2 |
| PC-2 — FastEthernet0 | S1 — FastEthernet0/3 |
| PC-3 — FastEthernet0 | S1 — FastEthernet0/4 |

### Step 2 — Configure the Router

Open `R1` → **CLI** and configure its LAN interface with a static gateway address:

```
enable
configure terminal
interface gigabitEthernet 0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit
```

This assigns the router the address `192.168.1.1/24` and enables the interface connected to the switch.

### Step 3 — Configure DHCP

Continue in the router CLI to create the DHCP address pool:

```
ip dhcp excluded-address 192.168.1.1 192.168.1.20
ip dhcp pool OFFICE-LAN
network 192.168.1.0 255.255.255.0
default-router 192.168.1.1
dns-server 8.8.8.8
end
```

The `OFFICE-LAN` pool defines the network and provides clients with gateway and DNS settings. Addresses `192.168.1.1` through `192.168.1.20` are excluded from automatic assignment.

### Step 4 — Configure the Computers

For each PC, open **Desktop → IP Configuration** and select **DHCP** instead of Static.

The computers will request their network settings automatically from the router. Each should receive a unique IPv4 address, subnet mask `255.255.255.0`, and default gateway `192.168.1.1`.

Example expected assignments:

| Device | Example IPv4 Address | Default Gateway |
| --- | --- | --- |
| PC-1 | 192.168.1.21 | 192.168.1.1 |
| PC-2 | 192.168.1.22 | 192.168.1.1 |
| PC-3 | 192.168.1.23 | 192.168.1.1 |

Actual assignments may differ depending on DHCP lease allocation.

### Initial Build Checkpoint

- [ ]  All five devices are connected.
- [ ]  The router interface is configured and enabled.
- [ ]  The DHCP pool and excluded address range are configured.
- [ ]  All three PCs are set to obtain addresses automatically.

# Screenshots Taken

![image.png](image.png)

![image.png](image%201.png)

![image.png](image%202.png)

![image.png](image%203.png)

# Conclusion

Successfully configured a router to automatically assign IPv4 addresses to three PCs using DHCP in Cisco Packet Tracer. Verified the DHCP leases, network configurations, and device connectivity using router commands, `ipconfig`, and `ping`. This project demonstrates practical skills in DHCP configuration, IPv4 networking, network verification, and basic troubleshooting relevant to entry-level IT Support and Networking roles.
