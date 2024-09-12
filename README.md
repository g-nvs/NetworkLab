# Home Network Lab

## Objective

The Home Network Lab aimed to build the "fundations" for the next projects I had in mind and also helped gain in-depth understanding of network operations and security.
The primary objective was to build a secured-by-design network with segmentation and isolation with a mix of virtualization and physical hardware.

### Skills Learned

- Advanced understanding of Networking concepts and practical application on FW and Switch.
- Investigation and troubleshooting on Network configuration, issues or performance. Firewall log analysis.
- Better understanding of Network Virtualization through Proxmox.
- 

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- OPNSense to monitor, block or route network traffic.
- PiHole to configure a local DNS for the Homelab, as well as a DNS forward over dns.eu servers. Added a DCHP on top of it to provide IP assignment to Laptops and IoT devices.
- Prometheus and Grafana Monitoring stack to keep track of both Proxmox and Server's health. (Next step would be to enable some automatic notifications in case of warnings)

## Steps

![home_nw drawio](https://github.com/user-attachments/assets/9ef678e7-5f17-47cb-8316-545d4cb67a30)
*Ref 1: Architecture Diagram overview*

1. Proxmox Installation on a physical appliance.
2. Proxmox Network configuration. (VLANs, Network Bridges)
3. Proxmox Server Hardening.
4. Physical Switch configuration. (VLANs, Ports)
5. Network Addressing and Segmentation.
6. OPNSense Installation over Proxmox.
7. OPNSense Interfaces, VLANs, Rule Policies and Global Configuration.
8. Added Automated feed of Malicious IP Blocking.
9. Added GeoIP Blocking with Maxmind integration on OPNSense.
10. DNS Installation over Proxmox. (pihole)
11. DNS Configuration along with DCHP for VLAN User.
12. Prometheus and Grafana Installation on a spare RPI4.
13. Node-Exporter installation and configuration on Assets.
14. ZenArmor installation and configuration over OPNSense.
