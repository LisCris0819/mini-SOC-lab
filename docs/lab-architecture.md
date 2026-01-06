# SOC Lab Architecture

## Purpose
This document defines the architecture and scope of a personal SOC lab designed to simulate a small-scale enterprise environment. The lab focuses on controlled log ingestion into Splunk for detection and investigation of common endpoint-based attack techniques.

## Components
- Splunk Server (installed locally on Windows host; Splunk Free license)
- Windows Endpoint virtual machine (primary victim and log source)
- Linux Endpoint virtual machine (attacker and log source)

## Log Sources (Initial)
- Windows Event Logs (Security, System)
- Linux authentication logs (SSH)

## Design Constraints
- Daily ingest limited to 500 MB (Splunk Free)
- Only targeted log sources enabled
- No full packet capture or verbose debug logging
