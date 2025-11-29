<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Load Data into DynamoDB

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-databases-dynamodb)

**Author:** Joel Mfunga  
**Email:** joelmfunga6@gmail.com

---

## Load Data into a DynamoDB Table

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-databases-dynamodb_b481c730)

---

## Introducing Today's Project!

### What is Amazon DynamoDB?

What is Amazon DynamoDB and why is it useful?

### How I used Amazon DynamoDB in this project

In today's project, I used Amazon DynamoDB to create and items.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project is error

### This project took me...

This project took me 1h33

---

## Create a DynamoDB table

DynamoDB tables organises data using rows and columns, but it's actually quite different from traditional relational databases.

In DynamoDB, an attribute is like a piece of data about an item. In this case, our item is Nikko and the attribute is the number of projects Nikko completed.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-databases-dynamodb_a3cefee0)

---

## Read and Write Capacity

Think of read capacity units (RCUs) as a way to measure how many engines DynamoDB is using to operate. Whereas Write capacity units (WCUs) are just like read capacity units - they give your DynamoDB tables the engines to edit/update/delete data!

Amazon DynamoDB's Free Tier covers 25 RCUS I turned off auto scaling because I dont need to pay

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-databases-dynamodb_ef47dd8f)

---

## Using CLI and CloudShell

AWS CloudShell is AWS CloudShell is shell in your AWS Management Console, which means it's a space for you to run code! The awesome thing about AWS CloudShell is that it already has AWS CLI pre-installed.

AWS CLI is is a software that lets you create, delete and update AWS resources with commands instead of clicking through your console.


I ran a CLI command in AWS CloudShell that created Tables.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-databases-dynamodb_81e0258b)

---

## Loading Data with CLI

I ran a CLI command in AWS CloudShell that ```bash
curl -O https://storage.googleapis.com/nextwork_course_resources/courses/aws/AWS%20Project%20People%20projects/Project%3A%20Query%20Data%20with%20DynamoDB/nextworksampledata.zip

unzip nextworksampledata.zip

cd nextworksampledata

```

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-databases-dynamodb_791c600b)

---

## Observing Item Attributes

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-databases-dynamodb_b481c731)

I checked a ContentCatalog item, which had the following attributes: 
ContenenType etc.

I checked another ContentCatalog item, which had a different set of attributes.

---

## Benefits of DynamoDB

A benefit of DynamoDB over relational databases is flexibility, because it is schema-less and allows you to store and query data without requiring a predefined structure.

Another benefit over relational databases is speed, because DynamoDB delivers single-digit millisecond response times thanks to its fully managed, in-memory caching and distributed architecture.

![Image](http://learn.nextwork.org/nostalgic_indigo_jolly_prickly_pear/uploads/aws-databases-dynamodb_b481c730)

---

---
