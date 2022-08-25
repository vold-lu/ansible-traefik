# Ansible playbook for Dolibarr

This playbook allows easy setup of [Traefik](https://traefik.io/traefik/) using [Ansible](https://www.ansible.com).
The playbook will install Traefik version 2.8.3.

## How to use it?

```bash
# Clone the repository
git clone https://github.com/vold-lu/ansible-traefik.git
cd ansible-traefik

# Create the inventory file (replace 127.0.0.1 by your host IP address)
echo '127.0.0.1' >> .inventory

# Run the playbook against the inventory
ansible-playbook -i .inventory --ask-become-pass traefik.yaml
```
