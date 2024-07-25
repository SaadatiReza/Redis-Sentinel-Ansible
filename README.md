# Redis Sentinel Ansible Automation

This project automates the setup of a Redis cluster with Sentinel using Ansible. It includes tasks to install and configure Redis, set up Sentinel for high availability, and ensure proper replication and monitoring.

## Prerequisites

- Ansible 2.9+
- Three or more servers for the Redis cluster
- SSH access to all servers

## Inventory

Create an `inventory.ini` file with your server details: (change the IP addresses based on your environment)

```ini
[redis]
redis1 ansible_host=192.168.5.101
redis2 ansible_host=192.168.5.102
redis3 ansible_host=192.168.5.103
```
## Change Redis Password
change your redis password in the `group_vars/all.yml` to make your redis more secure. 

## Usage
Run the playbook with:
```bash
ansible-playbook -i inventory.ini playbook.yml
```
