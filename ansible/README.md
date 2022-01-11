# Ansible

This folder contains ansible playbooks to install and configure ELK stack and other network tools (joy and mercury) verified on Ubuntu Server 21.10.

# Playbooks

- `install-elk`: Installs ELK stack services (Elasticsearch, Logstash and Kibana)
- `configure-elk`: Configures ELK stack, copying files from [elk-stack](../elk-stack/config) directory.
- `install-joy`: Builds and installs [Cisco/joy](https://github.com/cisco/joy)
- `install-mercury`: Builds and installs [Cisco/mercury](https://github.com/cisco/mercury)
- `main`: executes all playbooks in one run.

# Usage

> Please review all the configuration and commands before running an automated script from some random person in the Internet!


- Run all the playbooks:

```
ansible-playbook -i hosts main.yaml
```

- Or run any of them:

```
ansible-playbook -i hosts configure-elk.yaml
```

# References

- [Ansible Documentation](https://docs.ansible.com/)

