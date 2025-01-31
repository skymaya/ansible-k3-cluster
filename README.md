Install Kubernetes K3s Cluster with Ansible

This Ansible playbook will install kubernetes K3s on a small test cluster consisting of one server (controller) and two agents.

Development was done on VirtualBox VMs running Ubuntu 24.04.

Prerequisites

1. The server and agent VMs already provisioned with Ubuntu 24.04
3. Each VM has openssh-server installed and running
2. A VM (or host machine) running Ansible that can SSH to the server and agent VMs as root

Run

ansible-playbook -i hosts playbook.yml

or

ansible-playbook -i hosts playbook.yml --tags kubernetes
