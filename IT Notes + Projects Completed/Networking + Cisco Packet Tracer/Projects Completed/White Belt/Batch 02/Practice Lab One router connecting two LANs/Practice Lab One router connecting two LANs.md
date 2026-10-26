# Practice Lab:  One router connecting two LANs

# Initial Build — Two Subnets, One Router

**Difficulty:** White Belt

**Estimated Time:** 25–35 minutes

### Objective

Build a small network with two separate IPv4 subnets connected through a single router. Configure device addressing and verify communication between both LANs.

### 1. Equipment and Cabling

**Required Equipment**

- 4 × PC-PT
- 2 × Cisco 2960 switches (`SW1`, `SW2`)
- 1 × Cisco 1941 router (`R1`)
- 6 × Copper Straight-Through Ethernet cables

**Topology Connections**

| Device A | Device B |
| --- | --- |
| PC1 Fa0 | SW1 Fa0/1 |
| PC2 Fa0 | SW1 Fa0/2 |
| SW1 Fa0/24 | R1 G0/0 |
| R1 G0/1 | SW2 Fa0/24 |
| PC3 Fa0 | SW2 Fa0/1 |
| PC4 Fa0 | SW2 Fa0/2 |

### 2. IPv4 Address Configuration

Configure each PC through **Desktop → IP Configuration → Static**.

| Device | IPv4 Address | Subnet Mask | Default Gateway |
| --- | --- | --- | --- |
| PC0 | `192.168.10.10` | `255.255.255.0` | `192.168.10.1` |
| PC1 | `192.168.10.11` | `255.255.255.0` | `192.168.10.1` |
| PC2 | `192.168.20.10` | `255.255.255.0` | `192.168.20.1` |
| PC3 | `192.168.20.11` | `255.255.255.0` | `192.168.20.1` |

### 3. Initial Router Configuration

Open `R1` → **CLI**. If the initial configuration dialog appears, enter `no`.

```
enable
configure terminal
hostname R1

interface gigabitEthernet 0/0
description LAN_A
ip address 192.168.10.1 255.255.255.0
no shutdown
exit

interface gigabitEthernet 0/1
description LAN_B
ip address 192.168.20.1 255.255.255.0
no shutdown
exit

end
show ip interface brief
show ip route
```

**Expected Results**

- Both router interfaces eventually display `up/up`.
- The routing table contains connected routes for `192.168.10.0/24` and `192.168.20.0/24`.

### 4. Initial Connectivity Test

From PC1, open **Desktop → Command Prompt** and run:

```
ping 192.168.10.1
ping 192.168.20.10
ping 192.168.20.11
```

- **First ping:** Verifies connectivity to the local default gateway.
- **Second and third pings:** Verify communication with PCs on the remote subnet through R1.

*Note: The first ping may time out while ARP resolves device addresses. Repeat the test if necessary.*

### 5. Troubleshooting Checklist

- Verify Ethernet connections and interface status.
- Confirm both router interfaces have the correct IP addresses and `no shutdown` is configured.
- Check each PC's IPv4 address, subnet mask, and default gateway.
- Run `show ip route` on R1 to confirm both networks appear as directly connected.
- Remember: **No static routes are required** because both LANs connect directly to R1.

### Completion Criteria

- [ ]  All six Ethernet connections are established.
- [ ]  All four PCs have the correct IPv4 settings.
- [ ]  Both router interfaces display `up/up`.
- [ ]  PC1 can ping its gateway and both PCs on the second subnet.
- [ ]  The routing table contains both connected networks.

**Save the Packet Tracer project as:** `B8-One-Router-Two-LANs.pkt`

# Me Breaking The System

- On `PC3`  we changed the subnet mask to `255.255.255.123`
- We got a warning for invalid subnet address and the subnet and IPV4 box went empty.
- To Test that it’s broke, we pinged `PC1`  at `192.168.10.10`

![image.png](image.png)

![image.png](image%201.png)

# Troubleshooting scenario

## Scenario Description

Customer states their computer cannot connect to the router

## Testing the device itself, first

- We pinged `PC2`  at `192.168.20.11`  and we’re at 100% packet loss
- we move onto ip configuration
- we see the IP configuration boxes are blank for IPV4 and subnet mask and re-enter the IPV4 for designated PC which is `PC3`
- We pinged `PC2`  at `192.168.20.11`  again and all of our packets were sent back the device is now fixed

# Screenshots

![image.png](image%202.png)

![image.png](image%203.png)

![image.png](image%204.png)