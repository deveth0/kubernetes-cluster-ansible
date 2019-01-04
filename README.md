# Kubernetes-Cluster-Ansible

This repository contains different ansible-playbooks that can be used to setup a Kubernetes Cluster with Ubuntu 18.04 nodes.

## tl;dr
Configure your inventory and run the following commands:

* ansible-playbook -i inventory kube-install-software.yml -K
* ansible-playbook -i inventory kube-setup-cluster.yml -K 
* ansible-playbook -i inventory kube-self-hosted-recovery.yml -K

Afterwards you can use the `kubectl` command using the kube-master node's `root` account.
