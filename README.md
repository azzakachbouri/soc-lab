# soc-lab: mini-SOC and detection engineering lab

A small home SOC built with Wazuh to learn detection engineering: simulate
attacks, read the alerts, and write my own detection rules mapped to MITRE ATT&CK.

All attack simulations run only on my own isolated lab VMs.

## Lab

| Machine                            | Role                                     | Address        |
| ---------------------------------- | ---------------------------------------- | -------------- |
| Windows PC (VirtualBox host)       | attacker / admin workstation             | 192.168.56.1   |
| Wazuh-Server (Ubuntu Server 22.04) | Wazuh 4.10.5 manager, indexer, dashboard | 192.168.56.101 |
| agent-ubuntu (Ubuntu)              | monitored endpoint with the Wazuh agent  | 192.168.56.102 |

## Progress

| Phase                                       | Status  |
| ------------------------------------------- | ------- |
| 1. Lab setup                                | done    |
| 2. Attack simulation (Atomic Red Team)      | next    |
| 3. Own detection rules mapped to ATT&CK     | planned |
| 4. Integrate my TCP-proxy monitoring logs   | planned |
| 5. Incident report and architecture diagram | planned |
| 6. Cloud log extension (optional)           | planned |

## Documentation

- [01 Lab setup](docs/01-lab-setup.md)
- [02 Troubleshooting](docs/02-troubleshooting.md)
- [03 First alerts](docs/03-first-alerts.md)

## Security note

No passwords, keys or VM files are stored in this repository (see `.gitignore`).
