# Lab 03 — Examine NAT on a Wireless Router

**Platform:** Cisco Packet Tracer  
**Course:** Networking Basics — Cisco NetAcad  
**Status:** ✅ Complete

## What This Lab Covers
- Connecting 4 PCs to a wireless router and configuring DHCP on all clients
- Examining the router's WAN (public) IP assigned by the ISP
- Examining the router's LAN (private) IP and DHCP pool
- Using Simulation mode to generate HTTP traffic to a web server
- Observing NAT translation by examining inbound and outbound packet headers
- Confirming source IP changes as packets cross the router boundary

## Key Insight
NAT (Network Address Translation) replaces a device's private source IP
with the router's public IP as packets leave the network — and reverses
this on the return trip. This is why billions of devices sharing a small
pool of public IPs can all access the internet simultaneously. Importantly,
NAT is an address conservation mechanism, not a security tool.

## NAT Translation Summary
| Direction | Source IP | What Happens |
|-----------|-----------|-------------|
| PC → Router | 192.168.0.x (private) | Private IP leaves the PC |
| Router → Internet | ISP Public IP | NAT replaces private with public |
| Internet → Router | ciscolearn.nat.com | Response arrives at public IP |
| Router → PC | 192.168.0.x (private) | Router translates back to private |

## Files
| File | Description |
|------|-------------|
| `Lab03_NAT_Wireless_Router_Writeup.docx` | Full write-up with packet analysis and reflection |
| `Examine_NAT_on_a_Wireless_Router_Instructions.pka` | Completed Packet Tracer file |
| `Examine_NAT_on_a_Wireless_Router_Instructions.html` | Original Cisco NetAcad instruction manual |

## Screenshot
<img width="1438" height="696" alt="Screenshot 2026-06-29 at 1 20 34 AM" src="https://github.com/user-attachments/assets/2ed2eebe-7e78-4c21-890f-41b78f649e4d" />
