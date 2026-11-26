# 01 - Wazuh Server Installation

## Environment
- Host: MacBook (Apple Silicon), UTM virtualization
- VM: Ubuntu Server 24.04 ARM64, 4 GB RAM, 2 CPU cores, 50 GB disk
- Wazuh version: 4.14.11 (all-in-one: indexer, server, dashboard)

## Install
```
curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh
sudo bash wazuh-install.sh -a
```

## Result
Dashboard reachable at https://<server-ip>. Screenshot: ../wazuh-dashboard.png

## Notes
- First install attempt failed at the dashboard step and the script rolled back; a retry succeeded.
- Admin credentials are stored locally and never committed to this repo.
