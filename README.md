# Kubernetes-Cluster-Ansible

This repository contains different ansible-playbooks that can be used to setup a Kubernetes Cluster with Ubuntu 18.04 nodes.

A detailed description is available in my blog: https://www.dev-eth0.de/2019/01/04/kubernetes-cluster-ansible/

## tl;dr
Configure your inventory and run the following commands:

* `ansible-playbook -i inventory kube-install-software.yml -K`
* `ansible-playbook -i inventory kube-setup-cluster.yml -K `
* `ansible-playbook -i inventory kube-self-hosted-recovery.yml -K`

Afterwards you can use the `kubectl` command using the kube-master node's `root` account.


## Attributions
The ansible files are based on the work of `bsder` published on digitalocean.com:
https://www.digitalocean.com/community/tutorials/how-to-create-a-kubernetes-1-11-cluster-using-kubeadm-on-ubuntu-18-04
