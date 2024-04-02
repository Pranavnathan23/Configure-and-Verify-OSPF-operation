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

## Steps

### 1. Topology Description
- Design a network topology using Packet Tracer, depicting three interconnected networks (A, B, and C) connected via routers.
- Specify the IP addresses and subnet IDs for each network:
  - Network A: 192.168.1.0/24
  - Network B: 192.168.5.0/24
  - Network C: 192.168.3.0/24
 <br />
<img width="1280" alt="Capture" src="https://github.com/Pranavnathan23/Configure-and-Verify-OSPF-operation/assets/163876627/e2811dd8-3fe9-4e7e-85af-004b02484727">



  
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

<img width="1280" alt="Capture1" src="https://github.com/Pranavnathan23/Configure-and-Verify-OSPF-operation/assets/163876627/699d4e12-6628-49fb-879c-56ef93846252">


<br />
<br />

### 4. Neighbor Configuration
- Set OSPF router ID to influence OSPF operation using the `router-id` command.
- Adjust OSPF neighbor priority to change roles (DR/BDR) and influence routing behavior using the `ip ospf priority` command.
  
<br />

<img width="1280" alt="Capture2" src="https://github.com/Pranavnathan23/Configure-and-Verify-OSPF-operation/assets/163876627/05d032e6-079b-486e-bb8b-5fec589d2bca">




<br />
<br />

- Verify neighbor configurations and ensure changes are applied using the `show ip ospf neighbor` command.
<br />

<img width="1280" alt="Capture5" src="https://github.com/Pranavnathan23/Configure-and-Verify-OSPF-operation/assets/163876627/6dcc92b9-fcfb-44ad-bb8b-d019048d9179">



<br />
<br />

### 5. Load Balancing Configuration
- Verify OSPF routing table to identify existing routes and associated costs using the `show ip route` command.
- Configure unequal cost load balancing to distribute traffic across multiple paths using the `ip ospf cost` command.
- Verify load balancing configurations and test traffic simulation to ensure proper operation.
<br />

<img width="1280" alt="Capture7" src="https://github.com/Pranavnathan23/Configure-and-Verify-OSPF-operation/assets/163876627/b5045c8d-d92d-4257-af27-7cbef6fdbc68">


<br />
<br />

### 6. OSPF Verification
- Access the router's CLI and enter exec mode.
- Use commands like `show ip ospf neighbor` to verify OSPF neighborship.
- Verify OSPF processes and area information using `show ip ospf`.
  
<br />
  <img width="1280" alt="Capture8" src="https://github.com/Pranavnathan23/Configure-and-Verify-OSPF-operation/assets/163876627/17806ac2-cfba-421b-988a-de2c3c73cdca">
  <br />
<br />

- To display OSPF interface information on a Cisco router, use the command `show ip ospf interfaces`. This command provides detailed information about OSPF-enabled interfaces on the router, including IP addresses, OSPF process IDs, and interface costs.
<br />

<img width="1280" alt="Capture9" src="https://github.com/Pranavnathan23/Configure-and-Verify-OSPF-operation/assets/163876627/55319fe2-75b8-4525-a22c-083846478417">


<br />
<br />

- View OSPF database details with `show ip ospf database`.
- Check OSPF-specific routing table entries using `show ip route ospf`.

<br />

  <img width="1280" alt="Capture10" src="https://github.com/Pranavnathan23/Configure-and-Verify-OSPF-operation/assets/163876627/56709ba0-6dd3-4ae3-8694-b3d635c22781">

<br />
<br />

### Conclusion
This project provides a hands-on learning experience for configuring and verifying OSPF in a Cisco networking environment. By following these detailed steps, users can gain practical knowledge and skills in OSPF configuration, optimization, and troubleshooting, essential for network administrators and engineers.
