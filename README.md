# wsl-ansible-config

## Complete Workstation Setup

It is currently being used with [Ubuntu](https://ubuntu.com/) 22.04 and may or may not work on other versions or distros.

### Ansible Commands

Run this once after installing the OS and enabling systemd:

    sudo apt update && sudo apt install -y git ansible

Run this to apply the config to your workstation:

    sudo ansible-pull -U https://github.com/lab1702/wsl-ansible-config.git --extra-vars "host_user=$USER"
