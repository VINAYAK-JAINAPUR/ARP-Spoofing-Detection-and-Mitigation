# ARP Spoofing Detection and Mitigation in SDN Environments

## Overview
This project presents a robust framework for detecting and mitigating ARP spoofing attacks within Software-Defined Networking (SDN) environments. By leveraging Mininet for network emulation and Ettercap for ARP manipulation, we ensure a proactive defense strategy against ARP spoofing attacks.

## Project Description
The project involves the creation of a Mininet-based virtual network topology that includes multiple hosts, a switch, and a Ryu controller. This setup allows for the simulation and analysis of network behavior to detect and mitigate ARP spoofing attacks.

### Key Features
- **Network Emulation with Mininet:** Created a virtual network topology consisting of four hosts, one switch, and one Ryu controller.
- **ARP Manipulation with Ettercap:** Simulated ARP spoofing attacks to test the robustness of the detection and mitigation framework.
- **Ryu Controller Integration:** Developed applications to monitor ARP traffic, detect spoofing attacks, and block malicious packets in real-time.

## Tools Used
- **Mininet:** Network emulation tool for creating virtual network topologies.
   ![Topology Setup](https://github.com/VINAYAK-JAINAPUR/ARP-Spoofing-Detection-and-Mitigation/blob/main/images/setup.jpeg)
- **Ryu Controller:** An SDN framework for managing and controlling network flows.
- **Ettercap:** A network security tool used for ARP manipulation.
- **Python:** The programming language used for scripting the Ryu controller applications.

## Implementation Details
1. **Mininet Topology Setup:** Configured a network topology with multiple hosts, a switch, and a Ryu controller.
   ![Mininet Topology Setup](https://github.com/VINAYAK-JAINAPUR/ARP-Spoofing-Detection-and-Mitigation/blob/main/images/ryu.jpeg)
2. **Event Handling:** Utilized the Ryu controller's event-driven architecture to handle OpenFlow messages and monitor ARP traffic.
3. **Flowchart:** The following flowchart outlines the process of detecting and mitigating ARP spoofing attacks within the SDN environment:

![Flowchart](https://github.com/VINAYAK-JAINAPUR/ARP-Spoofing-Detection-and-Mitigation/blob/main/images/flowchart_cnet.jpeg)

4. **ARP Packet Analysis:** Parsed Ethernet frames to extract ARP protocol data and identify ARP replies.
5. **Spoofing Detection:** Maintained IP-to-MAC address mappings and detected discrepancies to identify spoofing attacks.
![Spoofing Detection](https://github.com/VINAYAK-JAINAPUR/ARP-Spoofing-Detection-and-Mitigation/blob/main/images/detection.jpeg)
6. **Spoofing Mitigation:** Suspicious ARP packets were dropped to prevent incorrect mappings.
   ![Mitigation Process](https://github.com/VINAYAK-JAINAPUR/ARP-Spoofing-Detection-and-Mitigation/blob/main/images/mitigation.jpeg)
  
 

## Achievements
- Successfully implemented real-time ARP spoofing detection and mitigation.
- Ensured network security by maintaining accurate IP-MAC address mappings.
- Demonstrated effective defense strategies against ARP spoofing attacks in a controlled virtual environment.
