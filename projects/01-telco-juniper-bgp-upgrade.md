# 01 · Juniper Firmware Upgrade & BGP Community Design

**Customer:** Grameenphone (mobile operator, Bangladesh), data security system
**Role:** Planning and implementation lead

## Scope
- Planned and executed a Juniper firmware (Junos) upgrade on the customer's data security platform
- Designed and configured BGP routing that uses **BGP communities** ("colour" tagging) to classify and steer routes

## Approach
1. **Pre-upgrade:** checked target-release compatibility, took configuration and state baselines (routes, BGP sessions, interfaces) and wrote a rollback plan
2. **Maintenance window:** upgraded in stages so that service stayed up throughout
3. **BGP design:** tagged routes with communities by source and purpose, then applied import/export policy based on those tags
4. **Validation:** compared post-upgrade state against the baseline and verified BGP sessions and route counts

## Technologies
Juniper Junos · BGP communities and routing policy · change management and rollback planning

## Related lab
BGP community policy example: [`network-config-templates/juniper/bgp-dual-isp.conf`](https://github.com/mihirchandra10/network-config-templates/blob/main/juniper/bgp-dual-isp.conf)
