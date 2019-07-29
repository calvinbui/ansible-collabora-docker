[![Build Status](https://travis-ci.com/calvinbui/ansible-collabora-docker.svg?branch=master)](https://travis-ci.com/calvinbui/ansible-collabora-docker)
![GitHub release](https://img.shields.io/github/release/calvinbui/ansible-collabora-docker.svg)
![Ansible Quality Score](https://img.shields.io/ansible/quality/42298.svg)
![Ansible Role](https://img.shields.io/ansible/role/d/42298.svg)

# Ansible Collabora

Collabora in Docker

##  Requirements

N/A

## Role Variables

`collabora_name`: Name of container

`collabora_image`: Docker image to use

`collabora_ports`: List of ports to expose

`collabora_logs_directory`: Directory to store log files

`collabora_certificates_directory`: Directory to cert files

`collabora_environment_variables`: Docker environmental variables. Find more at https://www.collaboraoffice.com/code/docker/

`collabora_docker_additional_options`: [Additional parameters](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html) to add to docker container

## Dependencies

N/A

## Example Playbook

```yaml
- hosts: servers
  become: true
  roles:
   - role: calvinbui.ansible_collabora_docker
```

## License

GPLv3

## Author Information

http://calvin.me
