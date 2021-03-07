[![Build Status](https://drone-ci.hopto.org/api/badges/Diesel-Net/traefik/status.svg)](https://drone-ci.hopto.org/Diesel-Net/traefik)

# traefik
Sets up [Traefik v2.4](https://doc.traefik.io/traefik) for each environment on our clusters.

## Requirements
- Ansible 2.10+

## Installing Dependencies
```bash
ansible-galaxy install -r roles/requirements.yaml -p ./roles --force
```

## Deploy to Docker Swarm
```bash
ansible-playbook deploy.yaml -i inventories/development/hosts --vault-id ~/.tokens/master_id
```
