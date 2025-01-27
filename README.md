# Lab-Mechanica -- WIP

Infrastructure as Code repository for home lab management and automation.

## Repository Structure

```
Lab-Mechanica/
├── cluster/                      # Raspberry Pi cluster configuration
│   ├── kubernetes/              # Kubernetes manifests and helm charts
│   ├── ansible/                 # Ansible playbooks for cluster management
│   └── monitoring/              # Cluster monitoring configurations
│
├── networking/                  # Network infrastructure
│   ├── ubiquiti/               # UniFi configurations and backups
│   ├── vlans/                  # VLAN definitions and documentation
│   └── dns/                    # DNS configurations including Pi-hole
│
├── services/                   # Core services configurations
│   ├── homeassistant/         # Home Assistant configuration and automations
│   ├── registry/              # Docker registry setup and maintenance
│   ├── grafana/               # Grafana dashboards and configurations
│   └── monitoring/            # General monitoring configurations
│
├── storage/                   # Storage system configurations
│   ├── unraid/               # Unraid system configurations
│   └── backup/               # Backup strategies and scripts
│
├── media/                    # Media server configurations
│   ├── plex/                # Plex server setup and maintenance
│   └── automation/          # Media management automation
│
├── docs/                    # Documentation
│   ├── setup/              # Initial setup instructions
│   ├── maintenance/        # Maintenance procedures
│   ├── network/           # Network architecture documentation
│   └── disaster-recovery/ # Disaster recovery procedures
│
├── scripts/                # Utility scripts
│   ├── maintenance/       # Maintenance scripts
│   └── monitoring/        # Monitoring scripts
│
└── terraform/             # Infrastructure as Code
    ├── modules/          # Reusable Terraform modules
    └── environments/     # Environment-specific configurations
```

## Key Components

### Cluster Management
- Kubernetes configurations for the Raspberry Pi cluster
- Ansible playbooks for automation and maintenance
- Cluster monitoring and alerting setup

### Networking
- UniFi configuration backups and restoration procedures
- VLAN definitions and documentation
- Pi-hole DNS configurations and adlists

### Core Services
- Home Assistant automation configurations
- Private Docker registry setup
- Grafana dashboards and data sources
- Monitoring stack configurations

### Storage & Media
- Unraid system configurations and share settings
- Plex media server setup and optimizations
- Backup strategies and verification procedures

### Documentation
- Complete setup instructions for rebuilding from scratch
- Regular maintenance procedures
- Network architecture documentation
- Disaster recovery procedures

## Getting Started

1. Clone this repository
2. Follow the setup instructions in `docs/setup/`
3. Configure environment variables according to `docs/setup/environment.md`
4. Run the initial setup script: `scripts/setup/init.sh`

## Maintenance Procedures

Regular maintenance tasks are documented in `docs/maintenance/` and automated via scripts in `scripts/maintenance/`.

## Monitoring

The monitoring stack includes:
- Grafana dashboards for system metrics
- AlertManager for notifications
- Prometheus for metrics collection
- Custom scripts for specific monitoring tasks

## License

See LICENSE file for details
