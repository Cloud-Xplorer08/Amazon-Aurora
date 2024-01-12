# Introduction to Amazon Aurora
## Overview

This lab introduces you to Amazon Aurora and provides you with a basic understanding of how to use Aurora. You will follow the steps to create an Aurora instance and then connect to it.

## Introducing the technologies
### Amazon Aurora

Aurora is a fully managed, MySQL-compatible, relational database engine that combines the performance and reliability of high-end commercial databases with the simplicity and cost-effectiveness of open-source databases. It delivers up to five times the performance of MySQL without requiring changes to most of your existing applications that use MySQL databases.

### Amazon Elastic Compute Cloud (Amazon EC2)

Amazon EC2 is a web service that provides resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. Amazon EC2 reduces the time required to provision new server instances to minutes, giving you the ability to quickly scale capacity, both up and down, as your computing requirements change.

### Amazon Relational Database Service (Amazon RDS)

Amazon RDS makes it easy to set up, operate, and scale a relational database in the cloud. It provides cost-efficient and resizable capacity while managing time-consuming database administration tasks, freeing you up to focus on your applications and business. Amazon RDS provides you with six database engines to choose from, including Aurora, Oracle, Microsoft SQL Server, PostgreSQL, MySQL, and MariaDB.

## Task 1: Create an Aurora instance
In this task, we will create an Aurora database (DB) instance.

![create database](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/5a64e940-939f-4d32-936e-a53e6e759a70)

![template and setting](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/afc325e4-db4a-4c28-aa84-5f48bed14694)

![instance config, avail, durability](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/0429785f-1b73-44a0-9e98-7e3956e1d923)

![connectivity](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/18e92378-c614-4e20-80f2-902bb97905e3)

![additional config](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/7283e6af-82b1-4b52-a2c7-f558bb1eaf11)

![database created](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/6a55cf18-87d0-4b6a-8f93-b0a64e0de9b3)


Your Aurora DB instance is in the process of launching and can take up to 5 minutes to launch.

While creating if error occured just select the older versions of your Aurora

## Task 2: Connect to an Amazon EC2 Linux instance

In this task, we log into to your Amazon EC2 Linux instance. This instance was launched for you when you started your lab using CloudFormation.

![ec2 instance created](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/1a0191c7-1249-4de4-a418-d7a0207deaac)

![session manager](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/e45f33bb-facf-454b-8fb8-edd85408b5f2)


## Task 3: Configure the Amazon EC2 Linux instance to connect to Aurora
In this task, we configure the Amazon EC2 Linux instance to connect to Aurora.

![install maridb command](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/a66f49c1-12be-48d8-8a7f-a7958b93bf2e)

### - sudo yum install mariadb -y
![writer instance endpoint](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/85758c6c-75dd-44af-9498-5f088713ddd3)

Replace <endpoint_goes_here> with the endpoint that you copied
### - mysql -u admin --password='admin123' -h <endpoint_goes_here>
![user pass endpoint](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/5a987af3-75a7-4fc0-a176-b7237f481df9)


## Task 4: Create a table and insert and query records
In this task, we learn how to create a table in a database, load data, and run a query.

![table created](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/0a3de491-765a-4d86-ad92-8c8b77641d21)

![new record inserted](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/8cf0d471-9b16-49c5-bf3c-884228e3389a)

![select statement used](https://github.com/Cloud-Xplorer08/Amazon-Aurora/assets/71820244/0b459374-b4e8-459d-b1df-22cd92e4aea3)







