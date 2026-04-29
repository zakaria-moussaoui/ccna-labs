<img width="609" height="463" alt="Topology" src="https://github.com/user-attachments/assets/2224b6a7-25ad-4a03-af32-7ccc75491fd3" />

## Objectives
- Configure VLANs 10, 20, 30
- Inter-VLAN routing via MLS (Multi-Layer Switch)
- Redundant links between MLS1 & MLS2
- WAN connectivity between R1 and R2

---

## Network Info

| VLAN | Name | Network | Devices |
|------|------|---------|---------|
| 10 | COMP | 192.168.10.0/24 | PC1, PC2, PC3 |
| 20 | HR | 192.168.20.0/24 | PC5, PC6 |
| 30 | INFO | 192.168.30.0/24 | Printer, PC4 |

## WAN Links

| Link | Network |
|------|---------|
| R1 — MLS1 | 10.10.10.0/30 |
| R1 — R2 | 10.10.10.4/30 |
| R2 — MLS2 | 10.10.10.8/30 |

## Test Results
- PC1 ping PC2 (VLAN 10) 
- PC1 ping PC5 (Inter-VLAN) 
- R1 ping R2 (WAN) 
