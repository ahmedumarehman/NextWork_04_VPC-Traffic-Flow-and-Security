<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# VPC Traffic Flow and Security

**Project Link:** [View Project](https://nextwork.ai/projects/fe5ed473-5874-57e1-a58f-d9b3d652330c)

**Author:** Ahmed Umar Rehman  
**Email:** ahmedumar475@gmail.com

---

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/fe5ed473-5874-57e1-a58f-d9b3d652330c_92b0b0b4)

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is a logically isolated virtual network in AWS, and it is useful because it allows you to control and secure how your AWS resources communicate with each other and the internet.

### How I used Amazon VPC in this project

In today's project, I used Amazon VPC to create and configure a virtual network with subnets, route tables, an Internet Gateway, Security Groups, and Network ACLs to control and secure network traffic.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was running into IAM permission issues, especially when my IAM user was unable to perform some VPC actions even after permissions were assigned.

### This project took me...

This project took me around 1 hour and 20 minutes

## Route tables

Route tables are rules that determine where network traffic from a subnet should go.

Route tables are needed to make a subnet public because they provide a route to an Internet Gateway, allowing the subnet's resources to communicate with the internet.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/fe5ed473-5874-57e1-a58f-d9b3d652330c_0a07b191)

## Route destination and target

Routes are defined by their destination and target, which mean

Destination = where the traffic is going.
Target = where the traffic should be sent.

The route had a destination of 0.0.0.0/0 and a target of my Internet Gateway.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/fe5ed473-5874-57e1-a58f-d9b3d652330c_0a07b191)

## Security groups

Security groups are virtual firewalls that control inbound and outbound traffic for AWS resources such as EC2 instances.

### Inbound vs Outbound rules

Inbound rules are rules that control what incoming traffic is allowed to reach a resource.

I configured an inbound rule that allows specific incoming traffic to reach my resource.

Outbound rules are rules that control what outgoing traffic is allowed from a resource.

By default, my security group's outbound rule allows all outbound traffic.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/fe5ed473-5874-57e1-a58f-d9b3d652330c_92b0b0b4)

## Network ACLs

Network ACLs (NACLs) are subnet-level firewalls that control inbound and outbound traffic using allow and deny rules.

### Security groups vs. network ACLs

The difference between a security group and a network ACL is that a security group operates at the resource level and is stateful, while a network ACL operates at the subnet level and is stateless.

## Default vs Custom Network ACLs

### Similar to security groups, network ACLs use inbound and outbound rules

By default, a network ACL's inbound and outbound rules will allow all traffic.

In contrast, a custom NACL’s inbound and outbound rules are automatically set to deny all traffic.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/fe5ed473-5874-57e1-a58f-d9b3d652330c_4faeb056)

## Tracking VPC Resources

---

*Built with [NextWork](https://nextwork.ai) - [View this project](https://nextwork.ai/projects/fe5ed473-5874-57e1-a58f-d9b3d652330c)*
