# Project Description: Advanced Static Routing Implementation with Redundancy and Failover Testing

This project involved the comprehensive design, configuration, and validation of a static routing topology in a multi-router network environment. Conducted as part of a university-level networking module, the project aimed to demonstrate mastery of static routing principles, redundancy mechanisms, and real-world troubleshooting in a controlled lab setting.

## Key Objectives:
- Implement static routing across a complex network topology with multiple LANs and inter-router links.
- Configure default routes for Internet access via an ISP router.
- Integrate floating static routes to ensure redundancy and failover capability.
- Validate connectivity and resilience through structured testing scenarios, including failure simulation and path verification.

## Network Topology Overview:
The topology consisted of:
- **Five routers** (R1 to R5) and one ISP router.
- **Three LANs:** Left LAN (192.168.10.0/24), Right LAN (192.168.20.0/24), and Server LAN (192.168.100.0/24).
- **Multiple WAN links** (Ethernet and Serial) with primary and backup paths.
- **Redundant connections** between routers to ensure path diversity and high availability.

## Technical Implementation:
- **Static Routing Configuration:** Manual configuration of routing tables on all routers using Cisco IOS commands.
- **Floating Static Routes:** Backup routes configured with higher Administrative Distances (AD) to ensure automatic failover.
- **Default Routing:** Gateway of last resort configured to direct Internet-bound traffic toward the ISP.
- **Hierarchical Routing:** Routes prioritized using AD values to control path selection.

## Testing & Validation:
A systematic testing approach was conducted across five scenarios:
1. **Basic Connectivity:** Successful ping and traceroute tests between all LANs and to the ISP.
2. **Internet Access:** Verified from all endpoints, confirming correct default route propagation.
3. **Link Failover (R1–R3):** Simulated single and multiple failures to validate redundancy mechanisms.
4. **Link Failover (R2–R4):** Confirmed symmetrical redundancy behavior.
5. **Multi-Failure Scenarios:** Tested extreme failure conditions to assess network resilience and routing consistency.

## Key Findings & Insights:
- Static routing proved reliable and predictable for stable, moderate-sized networks.
- Floating static routes successfully provided failover capability, though with limitations in dynamic convergence.
- Asymmetric routing issues were observed during partial failures, affecting diagnostic tools like traceroute while user connectivity (ping) remained intact.
- The project highlighted the importance of meticulous planning, thorough documentation, and proactive failure scenario anticipation in static routing environments.

## Conclusion:
This project successfully demonstrated the practical application of static routing in a redundant, multi-subnet environment. It reinforced essential networking skills—topology analysis, route planning, configuration management, and methodical troubleshooting—while providing valuable insights into the strengths and limitations of static routing in modern network design.
