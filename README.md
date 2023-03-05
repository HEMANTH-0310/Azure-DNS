# Azure-DNS
---
page_type: sample
languages:
- azurecli
products:
- azure-load-balancer
description: "Set up a virtual network with two virtual machines and a load balancer."
urlFragment: "https://github.com/whizlabs-learn/Azure-DNS"
---

Set up a load balancer to use in learn module exercise for "Host your domain on Azure DNS". Script creates:
- Virtual network for the VMs
- Network security group
- Two network interfaces
- Availability set
- Two virtual machines from a template
- Public IP address
- Load balancer
- Load balancer probe
- Load balancer rule

The script also:
- Updates the two network interfaces to associate them with the load balancer.
- Displays the IP address for the load balancer.


## Contents


| File/folder       | Description                                |
|-------------------|--------------------------------------------|
| `README.md`       | This README file.                          |
|`cloud-init.txt`             |Cloud-init script to configure the virtual machines     |
|`setup.sh`             | Script to set up and deploy a load balancer in Azure CLI                        |

## Prerequisites

The script is intended to be run from a BASH prompt in Azure Cloud Shell.


## Running the sample

To run the set-up script, run the following commands in Azure Cloud Shell:

  ```bash
  cd Azure-DNS  
  chmod +x setup.sh  
  ./setup.sh
  ```
