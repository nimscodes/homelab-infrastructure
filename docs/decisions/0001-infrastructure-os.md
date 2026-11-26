# ADR 0001: Ubuntu Server for the infrastructure node

Status: Accepted; implementation pending.

## Context
The Infrastructure node has 8 GB RAM and is available as a dedicated server. Core services should remain independent of the dual-boot workstation.

## Decision
Install Ubuntu Server 24.04 LTS directly on the infrastructure node. Begin with lightweight services and containers rather than multiple virtual machines.

## Alternatives
Retain Windows, use Rocky Linux, or install Proxmox. These remain valid alternatives for other nodes or future requirements.

## Consequences
Windows will be erased after backups and recovery preparation. Linux administration will be primarily remote. Battery condition, ventilation, lid behavior and power recovery must be checked before continuous operation.
