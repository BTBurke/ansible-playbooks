Vagrant Playbooks
===
This directory contains playbooks for setting up a Vagrant development environment.

Includes:
* An example Vagrantfile for calling Ansible for provisioning
* A vagranthosts inventory file that works with a VM on localhost
* A playbook for setting up a generic Ubuntu server environment (updating packages)
* A playbook (vboxguestadditions.yaml) that detects mismatches between the Virtualbox version on the host and the Guest Additions version on the VM.  It will install the correct Guest Additions version to eliminate errors with shared folders, etc.

Notes:

1. The shell scripts in the `scripts/` directory are necessary for the vboxguestadditions playbook.  They contain some command line ninjitsu to figure out which version of Vbox is installed on the host and Guest Additions version on the VM.