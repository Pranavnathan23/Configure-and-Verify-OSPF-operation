# OSPF Configuration and Verification in Cisco Packet Tracer

## Introduction
This project aims to demonstrate the configuration and verification of OSPF (Open Shortest Path First) routing protocol on Cisco routers. Through a series of guided steps, users will learn how to configure OSPF, influence OSPF behavior using router ID and priority settings, implement load balancing, and verify OSPF operation and connectivity.
<br />
<br />

## Objectives

- Set up OSPF (Open Shortest Path First) on Cisco routers.
- Configure OSPF router ID and priority.
- Implement unequal cost load balancing with OSPF.
- Verify OSPF configuration and operation.
  <br />
<br />

### Steps

### 1. Topology Description
- Describe the network topology using Packet Tracer, depicting three interconnected networks (A, B, and C) connected via routers.
- Specify the IP addresses and subnet IDs for each network:
  - Network A: 192.168.1.0/24
  - Network B: 192.168.5.0/24
  - Network C: 192.168.3.0/24
<br />
<br />

### 2. Initial Network Traffic Simulation
- Simulate network traffic between a host on Network A and a laptop on Network B using Packet Tracer.
- Observe the packet flow and identify any routing issues, such as packet drops due to lack of routing information.
<br />
<br />

### 3. OSPF Configuration
- Access the routers' command-line interface (CLI) and enter global configuration mode.
- Configure OSPF routing protocol with a chosen process ID (e.g., OSPF process ID 1).
- Identify and include the directly connected networks (A, B, and inter-router links) in OSPF advertisements.
- Assign area zero (backbone area) to the specified networks using the `network` command.
- Verify OSPF routing table to ensure successful network learning using the `show ip route` command.
<br />
<br />

### 4. Neighbor Configuration
- Set OSPF router ID to influence OSPF operation using the `router-id` command.
- Adjust OSPF neighbor priority to change roles (DR/BDR) and influence routing behavior using the `ip ospf priority` command.
- Verify neighbor configurations and ensure changes are applied using the `show ip ospf neighbor` command.
<br />
<br />

### 5. Load Balancing Configuration
- Verify OSPF routing table to identify existing routes and associated costs using the `show ip route` command.
- Configure unequal cost load balancing to distribute traffic across multiple paths using the `ip ospf cost` command.
- Verify load balancing configurations and test traffic simulation to ensure proper operation.
<br />
<br />

### 6. OSPF Verification
- Access the router's CLI and enter exec mode.
- Use commands like `show ip ospf neighbor` to verify OSPF neighborship.
- Verify OSPF processes and area information using `show ip ospf`.
- Display OSPF interface information with `show ip ospf interfaces`.
- View OSPF database details with `show ip ospf database`.
- Check OSPF-specific routing table entries using `show ip route ospf`.
<br />
<br />

### Conclusion
This project provides a hands-on learning experience for configuring and verifying OSPF in a Cisco networking environment. By following these detailed steps, users can gain practical knowledge and skills in OSPF configuration, optimization, and troubleshooting, essential for network administrators and engineers.
