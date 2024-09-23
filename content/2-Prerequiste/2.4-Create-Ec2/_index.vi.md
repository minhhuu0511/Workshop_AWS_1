---
title : "Tạo Public Linux EC2"
date :  "`r Sys.Date()`" 
weight : 4
chapter : false
pre : " <b> 2.4 </b> "
---

 Truy cập giao diện quản trị dịch vụ EC2:
![EC2](/images/2.prerequisite/013-createEC2.png)

![EC2](/images/2.prerequisite/076-createEC2.png)
  + Click **Instances**.
  + Click **Launch instances**.

![EC2](/images/2.prerequisite/014-createEC2.png)
  Tại trang **Step 1: Choose an Amazon Machine Image (AMI)**.
  + Click **Select** để lựa chọn AMI **Amazon Linux 2 AMI**.
  
![EC2](/images/2.prerequisite/015-createEC2.png)

 Tại trang **Step 2: Choose an Instance Type**.
 + Click chọn Instance type **t2.micro**.
 + Click **Next: Configure Instance Details**.
 
![EC2](/images/2.prerequisite/016-createEC2.png)
Tại hộp thoại **Key pair**.
  + Click chọn **Create a new key pair**.
  + Tại mục **Key pair name** điền **Web Server**.
  + Tại mục **Key pair type** chọn **RSA**.
  + Tại mục **Private Key format** chọn **.pem**
  + Click **Create Key Pair** và lưu xuống máy tính của bạn.
  
![EC2](/images/2.prerequisite/017-createEC2.png)
  Tại trang **Network setting**
  + Tại mục **VPC** chọn **VPC Main**.
  + Tại mục **Subnet** chọn **Public Subnet 1**.
  + Tại mục **Auto-assign Public IP** chọn **Use subnet setting (Enable)**
 + Chọn **Select an existing security group**.
  + Chọn security group **Web Server SG**.
 


+ Click **Launch Instances** để tạo máy chủ EC2.

