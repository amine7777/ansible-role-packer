Ansible role: Packer
=========

This role helps to install minikube on your linux machine.


|Travis|GitHub|Quality|Downloads|Version|
|------|------|-------|---------|-------|
|[![travis](https://travis-ci.com/amine7777/ansible-role-minikube.svg?branch=master)](https://travis-ci.com/amine7777/ansible-role-minikube)|[![github](https://github.com/amine7777/ansible-role-minikube/workflows/CI/badge.svg)](https://github.com/amine7777/ansible-role-minikube/actions)|[![quality](https://img.shields.io/ansible/quality/49942)](https://galaxy.ansible.com/amine7777/minikube)|[![downloads](https://img.shields.io/ansible/role/d/49942)](https://galaxy.ansible.com/amine7777/minikube)|[![Version](https://img.shields.io/github/release/amine7777/ansible-role-minikube.svg)](https://github.com/amine7777/ansible-role-minikube/releases/)|

Requirements
------------
- Linux machine
- Ansible 2.9

Role Variables
--------------
These variables helps to manage packer installation.

You can specify your packer version in this variable.
```yaml
packer_version: 1.5.6
packer_arch: amd64
packer_dir_path: /usr/local/bin
```
This is the url where packer will be downloaded.
```ỳaml
packer_download_url: 'https://releases.hashicorp.com/packer/{{ packer_version }}/packer_{{ packer_version }}_linux_{{ packer_arch }}.zip'
```
This is the path where packer binary will be stored.
```yaml
packer_dir_path: /usr/local/bin
```

Example Playbook
----------------

```yaml
- hosts: all
  roles:
     - amine7777.packer
```


Author Information
------------------

- [Amine Kahlaoui](https://github.com/amine7777), DevOps engineer.
