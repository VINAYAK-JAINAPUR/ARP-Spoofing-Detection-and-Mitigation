# ARP Spoofing Detection and Mitigation in SDN Environments

## Overview
This project presents a robust framework for detecting and mitigating ARP spoofing attacks within Software-Defined Networking (SDN) environments. By leveraging Mininet for network emulation and Ettercap for ARP manipulation, we ensure a proactive defense strategy against ARP spoofing attacks.

## Project Description
The project involves the creation of a Mininet-based virtual network topology that includes multiple hosts, a switch, and a Ryu controller. This setup allows for the simulation and analysis of network behavior to detect and mitigate ARP spoofing attacks.

### Key Features
- **Network Emulation with Mininet:** Created a virtual network topology consisting of four hosts, one switch, and one Ryu controller.
- **ARP Manipulation with Ettercap:** Simulated ARP spoofing attacks to test the robustness of the detection and mitigation framework.
- **Ryu Controller Integration:** Developed applications to monitor ARP traffic, detect spoofing attacks, and block malicious packets in real-time.

## Technologies Used
- **Mininet:** Network emulation tool for creating virtual network topologies.
- **Ryu Controller:** An SDN framework for managing and controlling network flows.
- **Ettercap:** A network security tool used for ARP manipulation.
- **Python:** The programming language used for scripting the Ryu controller applications.

## Implementation Details
1. **Mininet Topology Setup:** Configured a network topology with multiple hosts, a switch, and a Ryu controller.
   ![Topology Setup](images/topology_setup.png)
2. **Event Handling:** Utilized the Ryu controller's event-driven architecture to handle OpenFlow messages and monitor ARP traffic.
3. **ARP Packet Analysis:** Parsed Ethernet frames to extract ARP protocol data and identify ARP replies.
4. **Spoofing Detection and Mitigation:** Maintained IP-to-MAC address mappings and detected discrepancies to identify spoofing attacks. Suspicious ARP packets were dropped to prevent incorrect mappings.
   ![Spoofing Detection](images/spoofing_detection.png)
   ![Mitigation Process](images/mitigation_process.png)

## Achievements
- Successfully implemented real-time ARP spoofing detection and mitigation.
- Ensured network security by maintaining accurate IP-MAC address mappings.
- Demonstrated effective defense strategies against ARP spoofing attacks in a controlled virtual environment.
