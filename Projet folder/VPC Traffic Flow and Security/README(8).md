<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# VPC Traffic Flow and Security

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-security)

**Author:** Joel Mfunga  
**Email:** joelmfunga6@gmail.com

---

## VPC Traffic Flow and Security

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-security_92b0b0b4)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is a virtual network you create in AWS, and it is useful because it gives you full control over your networking environment, including subnets, routing, security, and connectivity to the internet or on-premises networks.

### How I used Amazon VPC in this project

In today's project, I used Amazon VPC to learn Traffic Flow and Security.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was full of details.

### This project took me...

This project took me 1hour

---

## Route tables

Route tables areas a GPS for the resources in your subnet. Just like a GPS helps people get to their destination in a city, a route table is a table of rules, called routes, that decide where the data in your network should go.

Route tables are needed to make a subnet public because they define where the traffic goes, and a subnet becomes public only when its route table sends internet-bound traffic (0.0.0.0/0) to an Internet Gateway.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-security_0a07b191)

---

## Route destination and target

Routes are defined by their destination and target, which means the destination specifies where the traffic is going, and the target specifies how the traffic will get there

The route in my route table that directed internet-bound traffic to my internet gateway had a destination of 0.0.0.0/0 and a target of Internet gateway.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-security_0a07b191)

---

## Security groups

If VPCs are cities and subnets are neighbourhoods, a security group is a security checkpoint, or security guard, at the entrance for each building (resource) in that neighbourhood (subnet).

### Inbound vs Outbound rules

Inbound rules control the data that can enter the resources in your security group I  configured an inbound rule that allow HTTPS Traffics to anywhere

Your server requests data from another service; your app sends out an email notification. Allow all traffic everywhere.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-security_92b0b0b4)

---

## Network ACLs

Network ACLs are stateless firewall rules that control inbound and outbound traffic at the subnet level in a VPC.

### Security groups vs. network ACLs

The difference between a security group and a network ACL is that security groups are stateful and operate at the instance level, while network ACLs are stateless and operate at the subnet level.

---

## Default vs Custom Network ACLs

### Similar to security groups, network ACLs use inbound and outbound rules

By default, a network ACL's inbound and outbound rules will allow all traffic.

In contrast, a custom ACL’s inbound and outbound rules are automatically set to deny all traffic.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-security_4faeb056)

---

## Tracking VPC Resources

---

---
