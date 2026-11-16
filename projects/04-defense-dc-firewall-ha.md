# 04 · Data Center Firewall High Availability

**Customer:** Defense organisation, Bangladesh (central data center)
**Role:** Planning, design and implementation

## Scope
- Planned, designed and implemented **active/passive high availability** between two **Palo Alto PA-3060** firewalls protecting the data center

## Approach
- Dedicated HA1 (control) and HA2 (session sync) links, with heartbeat backup
- Link and path monitoring so the pair fails over automatically when an uplink or the upstream gateway is lost
- Session synchronisation so existing connections survive a failover
- Controlled failover tests before handover

## Technologies
Palo Alto PA-3060 · PAN-OS HA (active/passive) · link and path monitoring · session synchronisation
