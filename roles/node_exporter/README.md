Role node_exporter
=========

An Ansible role to install and configure Node Exporter on Linux hosts.  
It downloads the official Node Exporter binary, installs it to `/usr/local/bin`, creates a dedicated system user, and sets up a systemd service to manage the Node Exporter daemon.

Role Variables
--------------

All variables can be found and customized in `defaults/main.yml`.

Dependencies
------------

This role has no external dependencies.

Example Playbook
----------------

Example playbook can be found in `playbooks/start_node_exporter.yml`.
