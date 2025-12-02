<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Testing VPC Connectivity

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-connectivity)

**Author:** Joel Mfunga  
**Email:** joelmfunga6@gmail.com

---

## Testing VPC Connectivity

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-connectivity_8ee57662)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC (Virtual Private Cloud) is a logically isolated virtual network that you create inside AWS.
It lets you control your own networking environment — including IP ranges, subnets, route tables, NAT gateways, and security layers.

### How I used Amazon VPC in this project

In today's project, I used Amazon VPC to to create subnet, route table, NACL SG etc.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was troubleshooting.

### This project took me...

This project took me 1h

---

## Connecting to an EC2 Instance

Connectivity is all about how well different parts of your network talk to each other and with external networks

My first connectivity test was whether I could connect to Public EC2. I only erro screen eve though I did not face it.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-connectivity_88727bef)

---

## EC2 Instance Connect

I connected to my EC2 instance using EC2 Instance Connect, which is public.

My first attempt at getting direct access to my public server resulted in an error, because HTTP was not allow inboud and outbound in SG.

I fixed this error by allowing HTTP in and outbound in SG.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-connectivity_1cbb1b88)

---

## Connectivity Between Servers

Ping is a command we use to test connectivity between two devices I used ping to test the connectivity between public server and private server.

The ping command I ran was ping 10.0.1.147

The first ping returned PING 10.0.1.147 (10.0.1.147) 56(84) bytes of data.64 bytes from 10.0.1.147: icmp_seq=1 ttl=127 time=0.782 ms This meant the ping fail.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-connectivity_defghijk)

---

## Troubleshooting Connectivity

I troubleshooted this by allowing ICMP4 in and outbound in NACL and Inbound in Security Group.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-connectivity_4a9e8014)

---

## Connectivity to the Internet

Curl is Just like ping, curl is a tool to test connectivity in a network. Where ping checks if one computer can contact another (and how long messages take to travel back and forwth), curl is used to transfer data to or from a server. That means on top of checking connectivity, you can use curl to grab data from, or upload data into other servers on the internet!



I used curl to test the connectivity between server.

### Ping vs Curl

Ping and curl are different because Checks basic reachability using ICMP and Interacts with web servers and APIs.

---

## Connectivity to the Internet

I ran the curl command curl https://learn.nextwork.org/projects/aws-host-a-website-on-s3.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-connectivity_8ee57662)

---

---
