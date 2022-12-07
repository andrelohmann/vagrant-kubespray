# vagrant-kubespray

 (c) Andre Lohmann (and others) 2022

## Maintainer Contact
  * Andre Lohmann
    <lohmann.andre (at) gmail (dot) com>
  * Westhand
    <martin-alpers (at) web (dot) de>

## Content

Install Kubernetes on a bare metal machine.

Workstation -> Vagrant Machine (provisioner) -> Server (Bare Metal) -> Vagrant K8s Cluster

### Prerequisites

  * Vagrant + VirtualBox installed on the Workstation (ideally latest versions from official vagrant and virtualbox repos)
  * Ubuntu Server minimized installed to the server

### Installation

  * Add your public key to the Server
  * Set the sudoers file to not request a password
  * Create a provisioner Vagrant Machine on your workbook (Linux Laptop, Mac, Whatever)
  * ...
