# traefik
Sets up Traefik v2 on our clusters for each environment. This is where all of our TLS certificates are stored.

## Requirements
- Ansible 2.10+

## Deploy to Docker Swarm
```bash
ansible-playbook deploy.yaml -i inventories/dev/hosts --vault-id ~/.tokens/master_id
```
