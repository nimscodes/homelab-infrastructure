# Architecture overview

Status: Proposed.

The lab separates administration, always-on infrastructure and on-demand compute. The infrastructure node will host lightweight services; the compute node will host resource-intensive VMs and GPU workloads; the management node will administer both.

Design principles: project independence, reproducibility, least privilege, isolation, incremental deployment and recovery testing.

The home router initially provides connectivity. Use DHCP reservations where supported. Future isolated virtual networks will support security and air-gap experiments. Physical VLAN support, backup destinations and storage capacity must be evaluated before finalizing the design.

The single infrastructure node is a potential point of failure. This design is not a highly available production system. Maintain recovery procedures and avoid making household connectivity depend on experimental services until tested.
