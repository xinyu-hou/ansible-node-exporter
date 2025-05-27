# Ansible Role: Node Exporter Setup

This repository contains an Ansible role and example playbooks to install and configure [Prometheus Node Exporter](https://github.com/prometheus/node_exporter) on Linux systems.

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/xinyu-hou/ansible-node-exporter.git
cd ansible-node-exporter
```

### Set Your Inventory
Create or modify your inventory file (e.g., `inventory.ini`):

```ini
[exporters]
target-host.example.com ansible_ssh_private_key_file=~/.ssh/id_rsa
```
Notes:

- Replace `target-host.example.com` with your target host's IP address or DNS name (hostname or CNAME).
- Replace `~/.ssh/id_rsa` with the path to your SSH private key if it’s not the default.
- You can also specify `ansible_user=<your_ssh_user>` if it’s different from your local username.

### Run the Playbook

```bash
ansible-playbook -i inventories/inventory.ini playbooks/start_node_exporter.yml
```
