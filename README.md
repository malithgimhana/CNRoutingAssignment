# Router Configuration and Routing Protocols using Cisco Packet Tracer


* **Module:** Computer Networks
* **Student Name:** P.D.M. Gimhana
* **Student ID:** 39330

---

## Project Overview
This repository contains the practical implementation files (.pkt) for the Cisco Packet Tracer routing configuration assignment. The assignment is divided into three core components tracking basic configuration, manual static routing setup, and dynamic routing protocol implementations (RIPv2 and EIGRP).

## Repository Files
The repository includes three separate Cisco Packet Tracer files matching the assignment requirements:
1. `Task1_BasicConfiguration.pkt` - Initial router initialization and security setups.
2. `Task2_StaticRouting.pkt` - Three-router triangular network topology with manual static paths.
3. `Task3_PartA_RIP.pkt` - Three-router linear topology using Routing Information Protocol version 2.
4. `Task3_PartB_EIGRP.pkt` - Three-router linear topology configured with Enhanced Interior Gateway Routing Protocol.

---

## Topology Descriptions & Implementation Details

### Task 1: Router Basic Configuration
* **Objective:** Establish baseline device identification and management line security constraints.
* **Device:** KandyNSBM_39330 (Cisco 2911 Router)
* **Configurations:**
  * Modified system prompt identity to reflect center name and student registration.
  * Secured the local hardware management connection channel using password authentication matching strict institutional directives.

### Task 2: Static Routing Configuration
* **Topology:** A three-router triangular loop architecture establishing high-availability links between distinct departments.
* **Nodes & Networks:**
  * **ComputingRouter:** Serving LAN subnet `192.168.1.0/24`
  * **BusinessRouter:** Serving LAN subnet `192.168.2.0/24`
  * **ScienceRouter:** Serving LAN subnet `192.168.3.0/24`
  * **Inter-Router WAN Links:** Point-to-point subnets `12.0.0.0/30`, `10.0.0.0/30`, and `11.0.0.0/30`.
* **Routing Logic:** Manually injected static route paths onto each independent routing engine table, explicitly specifying the incoming physical neighbor IP as the next-hop for all non-directly connected transit domains.

### Task 3: Dynamic Routing Configuration
* **Topology:** A segmented linear chain topology spanning separate geographic regional zones across a central distribution line.
* **Nodes & Networks:**
  * **KandyNSBM:** Edge domain serving LAN subnet `172.16.0.0/16`
  * **ColomboNSBM:** Central transit node joining core links.
  * **GalleNSBM:** Edge domain serving LAN subnet `173.16.0.0/16`
  * **Inter-Router WAN Links:** Point-to-point transit blocks `14.0.0.0/30` and `15.0.0.0/30`.

#### Part A: RIPv2 Setup
* Classless distance-vector routing logic activated globally.
* Directly attached subnets designated onto the local dynamic routing engine to automate inter-network map exchanges.

#### Part B: EIGRP Setup
* Pre-existing RIP routing processes completely dissolved from running memory.
* Enhanced Interior Gateway Routing Protocol activated using an assigned Autonomous System boundary identifier (`AS 10`).
* Directly connected networks re-advertised, allowing advanced diffusing update calculations to converge fast end-to-end paths across all network boundaries.

---

## Verification
All topologies have been validated for network layer end-to-end reliability. ICMP connection tests confirm consistent delivery with zero packet drops across all transit legs.
