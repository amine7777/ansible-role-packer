# Install Packer [![amine7777](https://circleci.com/gh/amine7777/install_packer.svg?style=svg)](https://circleci.com/gh/amine7777/install_packer)
--------------------------------------------------------------------------------------


![](packer.png)

This playbook is an easy way to install Packer with just adding the last version.

You need to have a Linux OS. You need to have Ansible already installed.

Please copy and paste these commands

```bash
git clone https://github.com/amine7777/install_packer
cd install_packer
ansible-playbook deploy_packer.yaml -e "packer_version=1.5.6"
```
