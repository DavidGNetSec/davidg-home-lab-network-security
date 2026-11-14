# DavidG Home Lab | Proposed Physical Topology

**Status:** Design proposal, not a verified deployment. Interface assignments, addressing, firewall roles and redundancy will be confirmed during configuration.

```mermaid
flowchart TD
 R[Cisco ISR 4331] --- F1[ASA 5516-X 1]
 F1 --- C[Catalyst 3560-X]
 F2[ASA 5516-X 2 - future security exercises] -. planned .- C
 C --- D1[Catalyst 3750 V2 1]
 C --- D2[Catalyst 3750 V2 2]
 D1 --- A[Catalyst 2960]
 A --- W[Windows analysis workstation]
```

This is a proposed logical arrangement of the seven existing Cisco devices. No failover or redundancy is claimed. Validate cabling and platform capabilities before implementation.
