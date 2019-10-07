# Ubuntu-based PHP development environment - Ansible playbook

## About

This Ansible playbook installs a working PHP development environment on
[Ubuntu 18.04 LTS](http://releases.ubuntu.com/18.04/).

## Usage

First you need to install git and Ansible on the local machine:

```
sudo apt update && sudo apt install git ansible
```

Then, execute the playbook using the following command:

```
ansible-playbook -i hosts.localhost site.yml --ask-become-pass
```
