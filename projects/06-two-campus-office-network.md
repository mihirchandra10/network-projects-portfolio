# 06 · Two-Campus Office Network with Zone-Based Security

**Customer:** Government mapping agency, Bangladesh (two office campuses)
**Role:** Design and implementation

## Scope
- Built the L2 and L3 office network at **two campuses**
- Configured zone-based security policies, ACLs and UTM
- Set up a **site-to-site IPsec VPN** between the two campuses

## Design (simplified)

```mermaid
flowchart LR
  subgraph A["Campus A"]
    FA[SRX-220] --- CA[EX-4300 / Brocade VDX-6740]
    CA --- AA[EX-2200 / HP 1920-48G access]
  end
  subgraph B["Campus B"]
    FB[SRX-220] --- CB[EX-4300]
    CB --- AB[EX-2200 access]
  end
  FA <-- "site-to-site IPsec" --> FB
```

## Technologies
Juniper SRX-220, EX-2200, EX-4300 · Brocade VDX-6740 · HP 1920-48G · security zones · ACL · UTM · IPsec VPN
