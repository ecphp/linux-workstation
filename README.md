# Ubuntu-based development environment - Ansible playbook

## About

NOTE: This project is deprecated and superseded by [ECGALAXY components](https://code.europa.eu/ecgalaxy).

This Ansible playbook installs a development environment on
[Ubuntu 18.04 LTS](http://releases.ubuntu.com/18.04/).

## Usage

First you need to install git and Ansible on the local machine:

```
sudo apt update && sudo apt install git ansible
```

Then, clone this repository, cd into ```linux-workstation``` and execute the playbook using the following command:

```
ansible-playbook -i hosts.localhost site.yml --ask-become-pass
```

## Optional

You can remove 'roles' you do not need by editing the ```site.yml``` file.

You can also limit the playbook execution to a specific role by using its tag, for instance:

```
ansible-playbook -i hosts.localhost -t docker site.yml --ask-become-pass
```
