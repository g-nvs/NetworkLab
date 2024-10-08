# Home Network Lab

## Objective

The Home Network Lab aimed to build the "fundations" for the next projects I had in mind and also helped gain in-depth understanding of network operations and security.
The primary objective was to build a secured-by-design network with segmentation and isolation with a mix of virtualization and physical hardware.

### Skills Learned

- Advanced understanding of Networking concepts and practical application on FW and Switch.
- Investigation and troubleshooting on Network configuration, issues or performance.
- Firewall and System logs understanding and analysis.
- Better understanding of Network Virtualization through Proxmox.
- Overall problem-solving skills on Linux and Proxmox.

### Tools Used

- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- OPNSense to monitor, block and route network traffic.
- PiHole to configure a local DNS for the Homelab, as well as a DNS forward over dns.eu Servers. Added a DCHP on top of it to provide IP assignment to Laptops and IoT devices.
- Prometheus and Grafana Monitoring stack to keep track of both Proxmox and Server's health. (Next step would be to enable some automatic notifications in case of warnings)

## Steps

![home_v2 drawio](https://github.com/user-attachments/assets/fbd1bd2f-9798-4b68-a727-4dea47267120)
</br>
*Ref 1: Architecture Diagram overview*

1. Proxmox Installation on a physical appliance.
2. Proxmox Network configuration. (VLANs, Network Bridges)
3. Proxmox Server Hardening.
4. Network Addressing and Segmentation.
5. Physical Switch configuration. (VLANs, Ports)
6. OPNSense virtualized over Proxmox.
7. OPNSense Interfaces, VLANs, Rule Policies and Global Configuration.
8. Added Automated feed of Malicious IP Blocking.
9. Added GeoIP Blocking with Maxmind integration on OPNSense.
10. DNS virtualized over Proxmox. (pihole)
11. DNS Configuration along with DCHP for VLAN User.
12. Prometheus and Grafana Installation on a spare RPI4.
13. Node-Exporter installation and configuration on Assets.
14. ZenArmor installation and configuration on OPNSense.
