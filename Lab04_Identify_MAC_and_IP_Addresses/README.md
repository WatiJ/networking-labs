# Lab 04 — Identify MAC and IP Addresses

**Platform:** Cisco Packet Tracer  
**Course:** Networking Basics — Cisco NetAcad  
**Status:** ✅ Complete

## What This Lab Covers
- Observing PDU header information during local network communication
- Observing PDU header information during remote network communication
- Understanding why MAC addresses change at each hop while IP addresses remain constant

## Key Insight
IP addresses are end-to-end — they never change for the entire journey.
MAC addresses are hop-to-hop — they are rewritten at every router boundary.
Switches operate at Layer 2 only and have no awareness of IP addressing.
When a destination is remote, the first hop destination MAC is the router's
interface — not the final device.

## PDU Observations (Remote Communication)
| At Device | Src MAC | Dst MAC | Src IP | Dst IP |
|-----------|---------|---------|--------|--------|
| 172.16.31.3 | 00D0.D311.C788 | 00D0.BA8E.741A | 172.16.31.3 | 10.10.10.2 |
| Switch 2 | 0060.7036.2849 | 00D0.BA8E.741A | N/A | N/A |
| Router (in) | 0060.7036.2849 | 00D0.BA8E.741A | 172.16.31.3 | 10.10.10.2 |
| Router (out) | 00D0.588C.2401 | 0060.2F84.4AB6 | 172.16.31.3 | 10.10.10.2 |
| 10.10.10.2 | 0060.2F84.4AB6 | 00D0.588C.2401 | 10.10.10.2 | 172.16.31.3 |

## Files
| File | Description |
|------|-------------|
| `Lab04_Identify_MAC_and_IP_Addresses_Writeup.docx` | Full write-up with PDU tables and key learning |
| `Identify_MAC_and_IP_Addresses.pka` | Completed Packet Tracer file |

## Screenshot
<img width="1104" height="636" alt="Screenshot 2026-06-30 at 9 47 38 PM" src="https://github.com/user-attachments/assets/dd84be50-a053-4665-9565-12055d4cba5d" />
