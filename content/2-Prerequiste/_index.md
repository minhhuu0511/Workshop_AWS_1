---
title : "Chuẩn bị VPC, EC2 và RDS "
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2. </b> "
---

Trong bước này, chúng ta sẽ cần tạo một VPC có 2 subnet public / private. Sau đó tạo 1 EC2 Instance Linux nằm trong public subnet,  1 EC2 Instance Windows nằm trong private subnet.

Tổng quan kiến trúc sau khi các bạn hoàn tất bước này sẽ như sau:

![VPC](/images/6.clean/073-Diagram.png)


### Nội dung
  - [Tạo VPC](2.1-Create-Vpc/)
  - [Tạo Security Group](2.2-Create-Secgroup/)
  - [Tạo DBSubnet Group](2.3-Create-DBSubnetGroup/)
  - [Tạo máy chủ EC2](2.4-Create-Ec2/)
  - [Tạo RDS](2.5-Create-Rds/)