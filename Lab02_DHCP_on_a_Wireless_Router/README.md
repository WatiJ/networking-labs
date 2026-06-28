# Lab 02 — Configure DHCP on a Wireless Router

**Platform:** Cisco Packet Tracer  
**Course:** Networking Basics — Cisco NetAcad  
**Status:** ✅ Complete

## What This Lab Covers
- Connecting 3 PCs to a wireless router via Ethernet
- Observing default DHCP settings and IP addressing
- Changing the router IP address from 192.168.0.1 to 192.168.5.1
- Updating the DHCP pool start address to 192.168.5.126 with max 75 users
- Enabling DHCP on all clients and verifying address assignment
- Verifying connectivity via ping between all devices

## Key Insight
Changing a router's IP mid-session immediately breaks client connectivity
because the clients are still on the old network. You must force a DHCP
renewal on each client before they can reach the router again. This is
a real-world troubleshooting scenario administrators encounter regularly.

## IP Addressing (Final)
| Device | IP Address | Default Gateway |
|--------|-----------|----------------|
| Wireless Router | 192.168.5.1 | ISP Assigned |
| PC0 | 192.168.5.126 | 192.168.5.1 |
| PC1 | 192.168.5.127 | 192.168.5.1 |
| PC2 | 192.168.5.128 | 192.168.5.1 |

## Files
| File | Description |
|------|-------------|
| `Lab02_DHCP_Wireless_Router_Writeup.docx` | Full write-up with config steps and reflection |
| `Configure_DHCP_on_a_Wireless_Router.pka` | Completed Packet Tracer file |
| `Configure_DHCP_on_a_Wireless_Router.html` | Original Cisco NetAcad instruction manual |

## Screenshot
<img width="1439" height="701" alt="Screenshot 2026-06-28 at 7 34 21 PM" src="https://github.com/user-attachments/assets/cca0fa55-3d78-4435-a325-345f31a7e29c" />
