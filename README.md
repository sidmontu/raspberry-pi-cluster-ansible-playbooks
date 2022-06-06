# Ansible playbooks to manage Raspberry Pi clusters

_(this is WIP)_

This repository contains a set of Ansible playbooks that help to set up and manage a Raspberry Pi cluster.

## How to run?

Install Ansible on a control node and define an inventory. Run a playbook as follows:

```bash
ansible-playbook some-playbook.yml --ask-pass
```

## Configuring

Change the target group name (the default is `rpies`) in the **.yml** files before running a playbook if needed.

## Available playbooks

* **ping.yml**: Pings all the machines
* **new-cluster.yml**: Updates the machines and expands their filesystem
* **shutdown.yml**: Shuts down all the machines
* **microk8s-prepare.yml**: Prepares for Kubernetes (Microk8s) installation
* **microk8s-install.yml**: Installs Kubernetes (MicroK8s)
* **microk8s-master.yml**: Generates join tokens in the master node
* **microk8s-workers.yml**: Makes workers join the cluster

## Related articles

* [Setting Up a Dedicated Database Server on Raspberry Pi](https://dzone.com/articles/set-up-a-dedicated-database-server-on-raspberry)
* [Building a 24-Core Raspberry Pi Cluster From Scratch](https://dzone.com/articles/building-a-24-core-raspberry-pi-cluster-from-scrat)
