# pfSense Setup Guide

This guide outlines the installation and configuration of pfSense for mission-grade firewalling and VPN tunneling.

## Installation
1. Download pfSense ISO from [official site](https://www.pfsense.org/download/).
2. Flash to USB using Rufus or Etcher.
3. Boot target machine and install pfSense.

## Network Segmentation
- Create VLANs for:
  - Mission Control
  - Telemetry
  - Admin
- Assign firewall rules per VLAN.

## VPN Configuration
- Enable OpenVPN or IPsec.
- Generate server and client certificates.
- Enforce MFA for remote access.

## Firewall Rules
- Allow telemetry ports (e.g., 5601 for Kibana).
- Block unauthorized outbound traffic.
- Log all access attempts.

## Final Notes
pfSense provides robust control for aerospace environments. All configurations should be backed up and versioned.
