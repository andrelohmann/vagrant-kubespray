# vagrant-kubespray

 (c) Andre Lohmann (and others) 2022

## Maintainer Contact
  * Andre Lohmann
    <lohmann.andre (at) gmail (dot) com>
  * Westhand
    <martinsmartformer (at) gmail (dot) com>

## Content

Install Kubernetes on a bare metal machine.

Server (Bare Metal) -> Vagrant K8s Cluster

### Prerequisites

  * Ubuntu Server minimized installed to the server
  * User k8s is created and has sudo permissions without password
  * Add your public key for remote access
  * Install ansible

```
apt update && apt install python3-pip git -yqq
# Ansible Version 2.11 is important for kubespray
pip install --upgrade ansible-core~=2.11.0
```

### Installation

  * login as k8s
  * Clone the repository

```
git clone https://github.com/andrelohmann/vagrant-kubespray.git
```

  * run the local deployment

```
cd vagrant-kubespace/localhost
ansible-galaxy install -r requirements.yml
ansible-playbook playbook.yml
```
