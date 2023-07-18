# AWS Cloud Instances Provisioning with Ansible

This folder contains Ansible playbooks and roles for provisioning cloud instances on AWS.

## Prerequisites

Before using these playbooks, you need to have the following:

- An AWS account
- [Ansible Automation Platform](https://developers.redhat.com/products/ansible/download) is installed on your local machine

## Using the playbook 
When using the create_ec2instance.yml playbook, be sure to specify the variables:
```
---
ec2_instance_name: example
region: us-east-1
instance_type: t3.micro
ami: ami-06640050dc3f556bb
key_name: ansible-demo
vpc_name: ansible-vpc
cidr_block: "10.10.0.0/16"
cidr: "10.10.0.0/24"
```
