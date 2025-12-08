<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Access S3 from a VPC

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-s3)

**Author:** Joel Mfunga  
**Email:** joelmfunga6@gmail.com

---

## Access S3 from a VPC

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-s3_3e1e79a2)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is my isolated network and it is useful because it allow me to have my own network inside of AWS.

### How I used Amazon VPC in this project

In today's project, I used Amazon VPC to to create subnet, routes etc.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was troubleshooting.

### This project took me...

This project took me 1h.

---

## In the first part of my project...

### Step 1 - Architecture set up

In this step, I will Create a VPC from scratch!
Launch an EC2 instance into your VPC.

### Step 2 - Connect to my EC2 instance

In this step, I will Connect directly to your EC2 instance.

### Step 3 - Set up access keys

In this step, I will Give your EC2 instance access to your AWS environment.

---

## Architecture set up

I started my project by launching my EC2 Server.

I also set up S3 and upload files in the bucket.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-s3_4334d777)

---

## Running CLI commands

AWS CLI is a command-line tool that allows you to manage AWS services from your terminal. I have access to AWS CLI because my AWS account and credentials are properly configured on my machine.

The first command I ran was aws s3 ls This command is used to access S3.

The second command I ran was aws configure This command is used to log into AWS and talk to your AWS services/resources.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-s3_e7fa8776)

---

## Access keys

### Credentials

To set up my EC2 instance to interact with my AWS environment.

Access keys, which are what we're learning about now, are credentials for your applications and other servers to log into AWS and talk to your AWS services/resources.

The secret access key is like the password that pairs with your access key ID (your username). You need both to access AWS services.

### Best practice

Although I'm using access keys in this project, a best practice alternative is to use IAM roles, which provide temporary credentials managed automatically by AWS and eliminate the need to store long-term access keys.

---

## In the second part of my project...

### Step 4 - Set up an S3 bucket

In this step, I will Launch a bucket in Amazon S3.

### Step 5 - Connecting to my S3 bucket

In this step, I will Head back to your EC2 instance.
Get your EC2 instance to interact with your S3 bucket.

---

## Connecting to my S3 bucket

The first command I ran was aws s3 ls This command is used to access S3.

When I ran the command aws s3 ls again, the terminal responded with the best resultatThis indicated it worked.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-s3_4334d778)

---

## Connecting to my S3 bucket

aws s3 ls s3://jmech-vpc-project

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-s3_4334d779)

---

## Uploading objects to S3

To upload a new file to my bucket, I first ran the command aws s3 cp /tmp/test.txt s3://jmech-vpc-project. This command creates a text file.

The second command I ran was 
sudo touch /tmp/test.txt

The third command I ran was aws s3 cp /tmp/test.txt s3://jmech-vpc-project/


![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-networks-s3_3e1e79a2)

---

---
