# Lab 05 — Observe Traffic Flow in a Routed Network

**Platform:** Cisco Packet Tracer  
**Course:** Networking Basics — Cisco NetAcad  
**Status:** ✅ Complete

## What This Lab Covers
- Observing ARP broadcast behaviour in a flat unrouted network
- Reconfiguring department switches to connect directly to router interfaces
- Renewing host IP addresses across new subnets using ipconfig /renew
- Observing how routing contains broadcasts to relevant subnets only
- Understanding performance and security benefits of network segmentation

## Key Insight
In a flat unrouted network every ARP request is processed by every device —
at 150+ devices this creates constant unnecessary overhead. After routing,
an ARP broadcast only reaches devices on the same subnet. Routing creates
broadcast domain boundaries that improve performance, enable security
policies between departments, and make networks scalable as they grow.

## Network Before & After
| | Unrouted | Routed |
|--|---------|--------|
| Accounting | 192.168.1.0/24 (shared) | 192.168.1.0/24 |
| Finance | 192.168.1.0/24 (shared) | 192.168.2.0/24 |
| Sales | 192.168.1.0/24 (shared) | 192.168.3.0/24 |

## Files
| File | Description |
|------|-------------|
| `Lab05_Observe_Traffic_Flow_Routed_Network_Writeup.docx` | Full write-up with comparison tables and key learning |
| `Observe_Traffic_Flow_in_a_Routed_Network.pka` | Completed Packet Tracer file |

## Screenshot
<img width="1440" height="563" alt="Screenshot 2026-06-30 at 11 16 44 PM" src="https://github.com/user-attachments/assets/07095a2f-99b2-4ed3-8248-0b523eb7bfe7" />
