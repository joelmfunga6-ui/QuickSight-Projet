<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Build a Virtual Private Cloud

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-vpc)

**Author:** Joel Mfunga  
**Email:** joelmfunga6@gmail.com

---

## Build a Virtual Private Cloud (VPC)

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-vpc_2facf927)

---

## Introducing Today's Project!

In this project, I will demonstrate how to create an Amazon VPC, A public subnet and internet gateway to allow instances to have internet connection. I'm doing this project to learn and understand VPC and its componets.

### What is Amazon VPC?

Amazon VPC is a network you create in AWS, and it is useful because it allows you to control IP addressing, subnets, routing, security, and how your resources connect to the internet or to your on-premises network.

In today's project, I used Amazon VPC to create subnet and internet gateway.

### Personal reflection

This project took 30min.

In this project nothing bad happen.

---

## Virtual Private Clouds (VPCs)

### What I did in this step

In this step, I will access the VPC console in AWS.
Create a VPC.

### How VPCs work

A VPC (Virtual Private Cloud) is your own private network inside a cloud provider like AWS.

### Why there is a default VPC in AWS accounts

This is because to deploy some services.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-vpc_2facf927)

### Defining IPv4 CIDR blocks

To set up my VPC, I had to define an IPv4 CIDR block, which is is a way to assign a whole block of IP addresses, kind of like creating a zone/area in a city.

---

## Subnets

### What I did in this step

In this step, I will launch a subnet inside my VPC.

### Creating and configuring subnets

subnets are like different neighborhoods inside your city. You use subnets to group resources with similar access rules and restrictions. Some subnets might be public areas that all resources can access (public subnets) while others are private areas with limited access (private subnets).

### Public vs private subnets

The difference between public and private subnet are public subnet are that a public subnet is connected to the internet and private subnet is for internal resources that don’t need to be publicly accessible.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-vpc_157c4219)

### Auto-assigning public IPv4 addresses

By default, my resources already have private IP addresss, but this only allows internal communication within your VPC.To access the internet or be accessible from the internet, the instance would need a public IP address.

---

## Internet gateways

### What I did in this step

In this step, I will connect my VPC to the internet using a internet gateway so that my EC2 in public subnet may have internet access

### Setting up internet gateways

An internet gateway connects my city (VPC) and the outside world (internet).

Internet gateways are key to making applications available on the internet. By attaching an internet gateway, your instances can access the internet and be accessible to external users.

Attaching an internet gateway means resources in your VPC can now access the internet. The EC2 instances with public IP addresses also become accessible to users, so your applications hosted on those servers become public too.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-vpc_4ae90410)

---

## Using the AWS CLI

### What I'm doing in this extension

In this project extension, I will Open a handy tool (called AWS CoudShell) to run commands.
Run AWS CLI commands to set up a VPC, subnet and internet gateway.
Showcase your secret mission in your project documentation.

### Exploring CloudShell and CLI

AWS CloudShell is shell in your AWS Management Console, which means it's a space for you to run code. The awesome thing about AWS CloudShell is that it already has AWS CLI pre-installed.

### Debugging my setup

Because CLI cannot create the subnet because it doesn’t know which IP addresses to allocate for it.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-vpc_9b2465411)

### Comparing CloudShell vs AWS Console

An advantage of using commands (AWS CLI) is that you can automate tasks, work faster, and repeat the same operation consistently.
With commands, you can script deployments, manage multiple resources at once, and avoid human errors that can happen when clicking through the Console.

---

---
