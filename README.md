# klondike

klondike will deploy and manage a Kubernetes cluster using AWS CloudFormation and Ansible.
klondike can send metrics to Datadog, aggregate logs via Logstash, and securely manage secrets using Ansible Vault.

This project is opinionated in how it deploys Kubernetes and the related services.
All feedback and code contributions are welcome, but the scope of this project is only intended to reflect one method of deployment.
klondike will not grow to encompass other deployment methodologies.

klondike is licensed under Apache 2.0.
See [LICENSE](LICENSE) for more details.

## Overview

klondike deploys three types of hosts: controllers, workers and a bastion.
The controllers operate the Kubernetes control plane, while the workers run pods scheduled to them via the Kubernetes API.

The bastion is an administrative host that facilitates the management of the klondike cluster.
An operator uses the bastion for initial cluster deployment, as well as on-going cluster management tasks.


## Installation 
There's no quick way to bootstrap this. However our guide is thourough and regularly tested.
[Installation] (INSTALL.md)

## Guides 
There's many users of a cluster. We have tried to be thorough but there is still much to do.
[Guides] (docs/index.md)
